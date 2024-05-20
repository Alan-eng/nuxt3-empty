<template>
	<div>
    Тест VK Bridge
		<NuxtWelcome />
	</div>
</template>

<script setup>
import bridge from "@vkontakte/vk-bridge"

onMounted(() => {
  console.log("onMounted")

  // Отправляет событие инициализации нативному клиенту
  bridge.send("VKWebAppInit")
})
</script>

<style></style>
