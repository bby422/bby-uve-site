<template>
  <a class="btn-default" v-bind:href="href" v-bind:title="title" @click="taClick" v-bind:rel="rel">{{text}}{{rel}}</a>
</template>
<script>
export default {
  name: 'cbutton',
  props: ['text', 'rel'],
  data() {
    return {
      href: '#',
      title: ''
    }
  },
  methods: {
    taClick: function(e) {
      e.preventDefault()
      this.text = 'OK'
    }
  }
}

</script>
