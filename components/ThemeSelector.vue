<template>
  <div>
    <button @click="setColorTheme('light')">Light</button>
    <button @click="setColorTheme('dark')">Dark</button>
  </div>
</template>

<script setup>
const colorMode = useColorMode()

function setColorTheme(theme) {
  colorMode.preference = theme
}
</script>
