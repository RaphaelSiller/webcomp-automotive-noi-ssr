<!--
SPDX-FileCopyrightText: NOI Techpark <digital@noi.bz.it>

SPDX-License-Identifier: AGPL-3.0-or-later
-->

<template>
  <label :for="text"> {{ text }} <sup v-if="required" class="text-red">*</sup> </label>
</template>

<script>
export default {
  props: {
    text: {
      type: String,
      default: ''
    },
    required: {
      type: Boolean,
      default: false
    }
  }
}
</script>

<style lang="postcss" scoped>
label {
  @apply block text-sm text-black mb-1;
}
</style>
