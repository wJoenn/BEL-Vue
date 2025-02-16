---
background: '#181818'
colorSchema: dark
layout: center
---

<div class="flex gap-8 max-w-full">
  <div class="min-w-0 space-y-8">
    <div>
      <h1>Louis Ramos</h1>
      <h2>Fullstack Vue/Rails developer at Leexi</h2>
    </div>
    <ul v-click="1">
      <li>AI-notetaker B2B SaaS</li>
      <li>Invite our bot in your online video calls or integrate with your VoIP</li>
      <li>Or record yourself and upload it to Leexi</li>
      <li>Get insights and statistics from your calls automatically</li>
    </ul>
    <p v-click="1">
      🔗
      <a href="https://www.leexi.ai/">leexi.ai</a>
    </p>
  </div>

  <div class="relative shrink-0 w-60">
    <img class="rounded-xl" src="/images/pp.webp" />
    <img v-click="1" class="absolute w-20 -bottom-10 -left-10 bg-white px-3 py-3.5 rounded-xl" src="/images/leexi.png" />
  </div>
</div>

---
layout: center
transition: slide-left
---

<div class="flex gap-8 max-w-full">
  <div class="min-w-0 space-y-8">
    <div>
      <h1>Louis Ramos</h1>
      <h2>Fullstack Vue/Rails developer at Leexi</h2>
    </div>
    <ul>
      <li>AI-notetaker B2B SaaS</li>
      <li>Invite our bot in your online video calls or integrate with your VoIP</li>
      <li class="text-[#80eec0]">Or record yourself and upload it to Leexi</li>
      <li>Get insights and statistics from your calls automatically</li>
    </ul>
    <p>
      🔗
      <a href="https://www.leexi.ai/">leexi.ai</a>
    </p>
  </div>

  <div class="relative shrink-0 w-60">
    <img class="rounded-xl" src="/images/pp.webp" />
    <img class="absolute w-20 -bottom-10 -left-10 bg-white px-3 py-3.5 rounded-xl" src="/images/leexi.png" />
  </div>
</div>

---
transition: slide-left
---

<h1>Why Capacitor ?</h1>
<div class="grid grid-cols-3 gap-8">
  <div class="bg-[#222222] rounded p-4 space-y-8">
    <div class="flex gap-4 justify-between items-center">
      <h2 class="!text-2xl">Native</h2>
        <div class="flex gap-2">
          <img class="h-8" src="/images/java.png" />
          <img class="h-8" src="/images/kotlin.png" />
          <img class="h-8" src="/images/swift.png" />
      </div>
    </div>
    <div class="bg-[#181818] p-4 rounded">
      <p class="!m-0">Pros</p>
      <ul>
        <li>Battle tested</li>
        <li>Community</li>
      </ul>
    </div>
    <div class="bg-[#181818] p-4 rounded">
      <p class="!m-0">Cons</p>
      <ul>
        <li>New languages</li>
        <li>Native UI library</li>
        <li>Different applications</li>
      </ul>
    </div>
  </div>
  <div v-click="1" class="bg-[#222222] rounded p-4 space-y-4">
    <h2 class="!text-2xl">Hybrid</h2>
    <div class="bg-[#181818] px-4 py-2 rounded">
      <div class="flex items-center gap-2">
        <img class="h-4" src="/images/flutter.png" />
        <h3 class="!text-lg">Flutter</h3>
      </div>
      <p class="!m-0 text-sm">Pros</p>
      <ul class="text-xs">
        <li>2 in 1</li>
        <li>Wider UI library</li>
      </ul>
      <p class="!m-0 text-sm">Cons</p>
      <ul class="text-xs">
        <li>Yet another language</li>
      </ul>
    </div>
    <div v-click="2" class="bg-[#181818] px-4 py-2 rounded">
      <div class="flex items-center gap-2">
        <img class="h-4" src="/images/react.png" />
        <h3 class="!text-lg">React Native</h3>
      </div>
      <p class="!m-0 text-sm">Pros</p>
      <ul class="text-xs">
        <li>JavaScript & popular</li>
      </ul>
      <p class="!m-0 text-sm">Cons</p>
      <ul class="text-xs">
        <li>Not Vue</li>
        <li>Native UI library</li>
      </ul>
    </div>
  </div>
  <div v-click="3" class="bg-[#222222] rounded p-4 space-y-4">
    <div>
      <h2 class="!text-2xl">Web Views</h2>
      <p class="text-sm !m-0">Web-based so can be designed in any way, usable on both platforms.</p>
      <p class="text-sm !m-0">Supposedly less performant and niche community.</p>
    </div>
    <div v-click="4" class="bg-[#181818] px-4 py-2 rounded">
      <div class="flex items-center gap-2">
        <img class="h-4" src="/images/capacitor.png" />
        <h3 class="!text-lg">Capacitor</h3>
      </div>
      <p class="!m-0 text-xs">Compatible with any framework</p>
    </div>
    <div v-click="4" class="bg-[#181818] px-4 py-2 rounded">
      <div class="flex items-center gap-2">
        <img class="h-4" src="/images/nativescript.png" />
        <h3 class="!text-lg">Native Script</h3>
      </div>
      <p class="!m-0 text-xs">No official support for Vue 3 yet</p>
    </div>
    <div v-click="4" class="bg-[#181818] px-4 py-2 rounded">
      <div class="flex items-center gap-2">
        <img class="h-4" src="/images/tauri.png" />
        <h3 class="!text-lg">Tauri</h3>
      </div>
      <p class="!m-0 text-xs">Rust-based</p>
    </div>
  </div>
</div>

---
transition: slide-left
---

# What is Capacitor ?

<div class="space-y-16 my-16">
  <div class="flex gap-8 items-center">
    <img class="h-24 shrink-0" src="/images/capacitor.png" />
    <div class="bg-[#222222] rounded grow p-4">
      <ul>
        <li>An Open source cross-platform native runtime for web apps.</li>
        <li>Includes many core native plugins such as Camera, File system, Geolocation etc</li>
        <div class="flex gap-16">
          <li>Framework agnostic</li>
          <li>440k weekly download on NPM</li>
        </div>
      </ul>
    </div>
  </div>
  <div class="bg-[#222222] rounded flex gap-8 p-4">
    <div class="flex flex-col bg-[#80eec020] border-[#80eec0] border border-dashed p-4 pt-2 gap-2">
      <p class="!m-0">Web View</p>
      <div class="flex gap-8">
        <div class="bg-[#9370db20] border border-dashed border-[#9370db] p-4">
          <p class="!m-0">Web App</p>
        </div>
        <div class="bg-[#119eff20] border border-dashed border-[#119eff] p-4">
          <p class="!m-0">Capacitor Bridge</p>
        </div>
      </div>
    </div>
    <div class="border border-dashed p-4 pt-2 gap-2 flex-col flex">
      <p class="!m-0">Native runtime</p>
      <div class="flex gap-8">
        <div class="bg-[#f9674320] border border-dashed border-[#f96743] p-4">
          <p class="!m-0">Camera</p>
        </div>
        <div class="bg-[#f9674320] border border-dashed border-[#f96743] p-4">
          <p class="!m-0">File system</p>
        </div>
        <div class="bg-[#f9674320] border border-dashed border-[#f96743] p-4">
          <p class="!m-0">Geolocation</p>
        </div>
      </div>
    </div>
  </div>
</div>

---
layout: center
transition: slide-left
---

# Let's have a demo

---
transition: slide-left
---

# Benefits && Drawbacks

<div class="grid grid-cols-2 gap-8 mt-16">
  <div class="space-y-8">
    <div v-click="1" class="bg-[#80eec020] border border-dashed border-[#80eec0] p-4">
      <p class="!m-0">Compatible with any JavaScript framework</p>
    </div>
    <div v-click="3" class="bg-[#80eec020] border border-dashed border-[#80eec0] p-4">
      <p class="!m-0">Integrates around your application, not the opposite</p>
    </div>
    <div v-click="4" class="bg-[#80eec020] border border-dashed border-[#80eec0] p-4 max-w-full">
      <p class="!m-0">Many existing plugins from the Capacitor team, the Capacitor-community company and other open source developers</p>
    </div>
  </div>
  <div class="space-y-8">
    <div v-click="2" class="bg-[#f9674320] border border-dashed border-[#f96743] p-4">
      <p class="!m-0">Not exactly "web development"</p>
    </div>
    <div v-click="5" class="bg-[#f9674320] border border-dashed border-[#f96743] p-4">
      <p class="!m-0">Smaller community compared to native solutions</p>
    </div>
    <div v-click="6" class="bg-[#f9674320] border border-dashed border-[#f96743] p-4">
      <p class="!m-0">You might still need to write some native code</p>
    </div>
  </div>
</div>

---
transition: slide-left
---

# Capacitor Voice Recorder

<div>
  <p>Capacitor voice recorder is a plugin to... <span v-click="1">record audio with your mobile device</span></p>
  <img v-click="[2, 3]" class="fixed bottom-5 left-1/2 -translate-x-1/2 h-96" src="/images/capacitor-voice-recorder/base.png">
  <img v-click="[3, 4]" class="fixed bottom-5 left-1/2 -translate-x-1/2 h-96" src="/images/capacitor-voice-recorder/send-file.png">
  <img v-click="[4, 5]" class="fixed bottom-5 left-1/2 -translate-x-1/2 h-96" src="/images/capacitor-voice-recorder/chunk.png">
  <img v-click="5" class="fixed bottom-5 left-1/2 -translate-x-1/2 h-96" src="/images/capacitor-voice-recorder/save-file.png">
</div>

---
layout: center
---

# Questions ?
