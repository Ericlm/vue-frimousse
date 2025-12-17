<script setup lang="ts">
import { default as EmojiPicker } from 'vue-frimousse'
import type { EmojiPickerEmoji } from 'vue-frimousse/src/packages/types.js';


const onEmojiClick = (emoji: EmojiPickerEmoji) => {
  console.log('Selected emoji:', emoji)
}
</script>

<template>
  <EmojiPicker.Root :onEmojiSelect="onEmojiClick">
    <EmojiPicker.Search placeholder="Search..." />
    <EmojiPicker.Viewport>
      <EmojiPicker.List />
    </EmojiPicker.Viewport>
  </EmojiPicker.Root>
</template>

