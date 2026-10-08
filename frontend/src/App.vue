<script setup{% if language == "typescript" %} lang="ts"{% endif %}>
const message{% if language == "typescript" %}: string{% endif %} = "Hello from Kurogane + Vue";
</script>

<template>
  <h1>{% raw %}{{ message }}{% endraw %}</h1>
</template>
