<template>
  <router-view />
</template>

<script lang="ts">
import { io } from "socket.io-client";
const socket = io("ws://localhost:3000", {
  transports: ["websocket", "polling", "flashsocket"]
})
export default {
  
}
</script>