<template>
	<a class="btn-default" v-bind:href="href" v-bind:title="title" @click="taClick">{{text}}</a>
</template>
<script>
export default {
  name: 'cbutton',
  data () {
    return {
      href: '#',
      title: '',
      text: '确定'
    }
  },
  methods: {
    taClick: function (e) {
      e.preventDefault()
       this.text = 'OK'
    }
  }
}
</script>