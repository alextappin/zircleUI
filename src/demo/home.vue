<template>
  <z-view style="border-width: 8px;">
    WELCOME TO ZIRCLE UI
    <div slot='extension'>
      <z-spot
        :angle='45'
        to-view='docs'
        class='accent'
        label='Docs'>
        <i class='fas fa-book'></i>
      </z-spot>
      <z-spot
        button
        :angle='135'
        class='accent'
        label='Github'
        @click.native="openUrl">
        <i class='fab fa-github'></i>
      </z-spot>
    </div>
  </z-view>
</template>
<script>
export default {
  methods: {
    openUrl () {
      window.open('https://github.com/zircleUI/zircleUI', '_blank')
    }
  }
}
</script>
