<template>
  <section id="catalog" class="relative w-full min-h-screen bg-black text-white px-4 py-10">
    <!-- Background image if desired -->
    <div class="absolute inset-0 bg-no-repeat bg-cover bg-center opacity-20" :style="{ backgroundImage: `url('/img.png')` }"></div>

    <div class="relative z-10 max-w-6xl mx-auto">
      <!-- Catalog Heading -->
      <h2 class="text-4xl font-semibold mb-8 text-[#A5846C]">КАТАЛОГ</h2>

      <!-- Car Grid -->
      <div class="grid gap-6 sm:grid-cols-2 lg:grid-cols-3">
        <!-- Card 1: HYUNDAI ELANTRA 2018-2020 -->
        <div class="bg-[#1C1C1C] rounded-xl overflow-hidden shadow-lg flex flex-col">
          <img
              src=""
              alt="Hyundai Elantra 2018-2020"
              class="w-full h-48 object-cover"
          >
          <div class="p-4 flex flex-col flex-grow">
            <h3 class="text-xl font-bold text-[#C1A38A] mb-2">HYUNDAI ELANTRA<br>2018-2020 год</h3>
            <p class="flex items-start text-sm text-gray-300 mb-2">
              <svg class="w-5 h-5 inline-block mr-1 mt-1" fill="currentColor" viewBox="0 0 20 20">
                <path d="M11.3,1.046c..."/>
              </svg>
              <ul>
                <li>Объем: 2.5</li>
                <li>Коробка передач: автомат</li>
              </ul>
            </p>
            <p class="text-xl font-semibold text-white mb-4">18 000 тг/сутки</p>
            <button
                class="mt-auto bg-[#A5846C] text-white py-2 px-4 rounded hover:bg-[#8f6f5b] transition"
                @click="showModal = true"
            >
              Арендовать авто
            </button>
          </div>
        </div>

        <!-- Card 2: KIA K3 2022-2023 -->
        <div class="bg-[#1C1C1C] rounded-xl overflow-hidden shadow-lg flex flex-col">
          <img
              src=""
              alt="Kia K3 2022-2023"
              class="w-full h-48 object-cover"
          >
          <div class="p-4 flex flex-col flex-grow">
            <h3 class="text-xl font-bold text-[#C1A38A] mb-2">KIA K3<br>2022-2023 год</h3>
            <p class="flex items-center text-sm text-gray-300 mb-2">
              <svg class="w-5 h-5 inline-block mr-1" fill="currentColor" viewBox="0 0 20 20">
                <path d="M11.3,1.046c..."/>
              </svg> Объем 1.6
            </p>
            <p class="text-xl font-semibold text-white mb-4">23 000 тг/сутки</p>
            <button
                class="mt-auto bg-[#A5846C] text-white py-2 px-4 rounded hover:bg-[#8f6f5b] transition"
                @click="showModal = true"
            >
              Арендовать авто
            </button>
          </div>
        </div>

        <!-- Card 3: HYUNDAI ELANTRA 2022-2024 -->
        <div class="bg-[#1C1C1C] rounded-xl overflow-hidden shadow-lg flex flex-col">
          <img
              src=""
              alt="Hyundai Elantra 2022-2024"
              class="w-full h-48 object-cover"
          >
          <div class="p-4 flex flex-col flex-grow">
            <h3 class="text-xl font-bold text-[#C1A38A] mb-2">HYUNDAI ELANTRA<br>2022-2024 год</h3>
            <p class="flex items-center text-sm text-gray-300 mb-2">
              <svg class="w-5 h-5 inline-block mr-1" fill="currentColor" viewBox="0 0 20 20">
                <path d="M11.3,1.046c..."/>
              </svg> Объем 1.6
            </p>
            <p class="text-xl font-semibold text-white mb-4">25 000 тг/сутки</p>
            <button
                class="mt-auto bg-[#A5846C] text-white py-2 px-4 rounded hover:bg-[#8f6f5b] transition"
                @click="showModal = true"
            >
              Арендовать авто
            </button>
          </div>
        </div>

        <!-- Card 4: HYUNDAI SONATA 2021 -->
        <div class="bg-[#1C1C1C] rounded-xl overflow-hidden shadow-lg flex flex-col">
          <img
              src=""
              alt="Hyundai Sonata 2021"
              class="w-full h-48 object-cover"
          >
          <div class="p-4 flex flex-col flex-grow">
            <h3 class="text-xl font-bold text-[#C1A38A] mb-2">HYUNDAI SONATA<br>2021</h3>
            <p class="flex items-center text-sm text-gray-300 mb-2">
              <svg class="w-5 h-5 inline-block mr-1" fill="currentColor" viewBox="0 0 20 20">
                <path d="M11.3,1.046c..."/>
              </svg> Объем 3.5
            </p>
            <p class="text-xl font-semibold text-white mb-4">35 000 тг/сутки</p>
            <button
                class="mt-auto bg-[#A5846C] text-white py-2 px-4 rounded hover:bg-[#8f6f5b] transition"
                @click="showModal = true"
            >
              Арендовать авто
            </button>
          </div>
        </div>

        <!-- Card 5: TOYOTA CAMRY 75 2024 -->
        <div class="bg-[#1C1C1C] rounded-xl overflow-hidden shadow-lg flex flex-col">
          <img
              src=""
              alt="Toyota Camry 75 2024"
              class="w-full h-48 object-cover"
          >
          <div class="p-4 flex flex-col flex-grow">
            <h3 class="text-xl font-bold text-[#C1A38A] mb-2">TOYOTA CAMRY 75<br>2024 год</h3>
            <p class="flex items-center text-sm text-gray-300 mb-2">
              <svg class="w-5 h-5 inline-block mr-1" fill="currentColor" viewBox="0 0 20 20">
                <path d="M11.3,1.046c..."/>
              </svg> Объем 2.5
            </p>
            <p class="text-xl font-semibold text-white mb-4">40 000 тг/сутки</p>
            <button
                class="mt-auto bg-[#A5846C] text-white py-2 px-4 rounded hover:bg-[#8f6f5b] transition"
                @click="showModal = true"
            >
              Арендовать авто
            </button>
          </div>
        </div>
      </div>
    </div>

    <!-- Modal -->
    <transition name="fade">
      <div
          v-if="showModal"
          @click="showModal = false"
          class="fixed inset-0 z-50 flex items-center justify-center bg-black bg-opacity-70 p-4"
      >
        <div class="relative bg-white text-black w-full max-w-md mx-auto rounded-lg shadow-lg p-8" @click.stop="showModal">

          <!-- Modal Title & Subtitle -->
          <h2 class="text-2xl font-semibold mb-2 text-black">Оставьте ваши данные и мы с вами свяжемся</h2>
          <p class="text-gray-600 mb-6 text-sm">Скидка 10% всем новым клиентам!</p>

          <!-- Form -->
          <form @submit.prevent="handleFormSubmit">
            <!-- Name Input -->
            <label class="block mb-4">
              <input
                  type="text"
                  placeholder="Ваше имя*"
                  v-model="formData.name"
                  class="w-full border border-gray-300 rounded-full py-2 px-4 focus:outline-none focus:border-[#A5846C]"
                  required
              />
            </label>

            <!-- Phone Input -->
            <label class="block mb-1 relative">
              <span class="absolute left-4 top-2 text-xl">🇰🇿</span>
              <input
                  type="tel"
                  placeholder="+7 (999) 999-99-99"
                  v-model="formData.phone"
                  :class="{'border-red-500': !isPhoneValid && formData.phone}"
                  class="w-full border border-gray-300 rounded-full py-2 pl-10 pr-4 focus:outline-none focus:border-[#A5846C]"
                  required
              />
            </label>
            <!-- Error Message -->
            <p v-if="!isPhoneValid && formData.phone" class="text-red-500 text-sm mb-4">Пожалуйста, введите корректный номер в формате: +7 (XXX) XXX-XX-XX</p>

            <!-- Submit Button -->
            <button
                type="submit"
                class="w-full rounded-full py-2 mt-4 text-white font-semibold"
                :style="{ background: 'linear-gradient(to right, #A5846C, #C1A38A)' }"
            >
              Арендовать авто
            </button>
          </form>

          <!-- Footer Note -->
          <p class="text-gray-500 text-xs mt-4 italic">*Не сдаем в аренду под такси</p>
        </div>
      </div>
    </transition>
  </section>
</template>

<script setup>
import { ref, computed } from 'vue'

const showModal = ref(false)
const formData = ref({
  name: '',
  phone: ''
})

// Regex for phone format: +7 (XXX) XXX-XX-XX
// Explanation:
// ^\+7 \( - starts with +7 (
// \d{3} - exactly 3 digits
// \)  - closing parenthesis
// \s - a space
// \d{3} - 3 digits
// -\d{2}-\d{2}$ - a dash, then 2 digits, dash, then 2 digits to the end of the string
const phoneRegex = /^\+7 \(\d{3}\) \d{3}-\d{2}-\d{2}$/

const isPhoneValid = computed(() => {
  if (formData.value.phone === '') return true // If empty, don't show error yet
  return phoneRegex.test(formData.value.phone)
})

function handleFormSubmit() {
  // Validate before submission
  if (!isPhoneValid.value) {
    // If phone is invalid, do not proceed.
    return
  }

  // Handle form submission (e.g., send data to server)
  console.log('Name:', formData.value.name)
  console.log('Phone:', formData.value.phone)

  // Clear form or handle success state, then close modal
  formData.value.name = ''
  formData.value.phone = ''
  showModal.value = false
}
</script>

<style scoped>
.fade-enter-active, .fade-leave-active {
  transition: opacity 0.2s;
}
.fade-enter-from, .fade-leave-to {
  opacity: 0;
}
</style>
