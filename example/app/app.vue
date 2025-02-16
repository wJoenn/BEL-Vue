<template>
  <div class="bg-[#181818] min-h-screen text-white">
    <p class="fixed top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 text-[200px]">{{ diceRoll }}</p>

    <div class="fixed bottom-0 p-8 flex items-center justify-center inset-x-0">
      <button
        class="bg-[#222222] px-5 py-3 rounded text-xl"
        @click="rollDice"
      >
        Roll a D100
      </button>
    </div>
  </div>
</template>

<script setup>
  const diceRoll = ref()

  const rollDice = async () => {
    for (let i = 0; i < rand({ max: 20, min: 10 }); i++) {
      diceRoll.value = rand({ max: 100 })
      await sleep(30)
    }
  }

  const rand = ({ max, min = 0 }) => Math.ceil(Math.random() * (max - min)) + min
  const sleep = duration => new Promise(resolve => setTimeout(resolve, duration))
</script>
