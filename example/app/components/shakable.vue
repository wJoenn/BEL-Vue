<template>
  <div class="bg-[#181818] min-h-screen text-white">
    <p class="fixed top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 text-[200px]">{{ diceRoll }}</p>

    <div class="fixed bottom-0 p-8 flex items-center justify-center inset-x-0">
      <p class="text-slate-500">Shake your device to roll a D100</p>
    </div>
  </div>
</template>

<script setup lang="ts">
  import { Motion, type AccelListenerEvent } from "@capacitor/motion"

  const diceRoll = ref<number>()

  const rollDice = async ({ acceleration: { x, y, z } }: AccelListenerEvent) => {
    if ([x, y, z].every(accel => accel < 30)) { return }

    for (let i = 0; i < rand({ max: 20, min: 10 }); i++) {
      diceRoll.value = rand({ max: 100 })
      await sleep(30)
    }
  }

  const rand = ({ max, min = 0 }: { max: number, min?: number }) => Math.ceil(Math.random() * (max - min)) + min
  const sleep = (duration: number) => new Promise(resolve => setTimeout(resolve, duration))

  onMounted(() => {
    Motion.addListener('accel', rollDice)
  })
</script>
