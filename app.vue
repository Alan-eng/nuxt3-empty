<template>
	<div>
    Тест VK Bridge
		<NuxtWelcome />
	</div>
</template>

<script>
import bridge from "@vkontakte/vk-bridge"

console.log("Перед VKWebAppInit")

// Отправляет событие инициализации нативному клиенту
bridge.send("VKWebAppInit")
</script>

<style></style>
