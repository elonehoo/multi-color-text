<script setup lang="ts">

</script>

<template>
  <div style="width: 500px;margin: auto;">
    <div class="multiColor">
      <p style="font-size: 15vh;">multi color text</p>
    </div>
  </div>
</template>

<style>

:root{
  --color1: #01579B;
  --color2: #00838F;
  --color3: #FFD600;
  --color4: #FF4081;
  --color5: #F44336;
}

.multiColor {
  background:linear-gradient(225deg,
    var(--color1) 0%, var(--color1) 9%,
    transparent 9%, transparent 10%,
    var(--color2) 10%, var(--color2) 19%,
    transparent 19%, transparent 20%,
    var(--color3) 20%, var(--color3) 29%,
    transparent 29%, transparent 30%,
    var(--color4) 30%, var(--color4) 39%,
    transparent 39%, transparent 40%,
    var(--color5) 40%, var(--color5) 49%,
    transparent 49%, transparent 50%,
    var(--color1) 50%, var(--color1) 59%,
    transparent 59%, transparent 60%,
    var(--color2) 60%, var(--color2) 69%,
    transparent 69%, transparent 70%,
    var(--color3) 70%, var(--color3) 79%,
    transparent 79%, transparent 80%,
    var(--color4) 80%, var(--color4) 89%,
    transparent 89%, transparent 90%,
    var(--color5) 90%, var(--color5) 99%,
    transparent 99%
  );
  background-clip: text;
  -webkit-background-clip: text;
  background-size: 200% 200%;
  color: transparent;
  animation: move 4s linear infinite;
}

@keyframes move {
  0%{
    background-position: 0px 100%;
  }
  100%{
    background-position: 100% 0px;
  }
}
</style>
