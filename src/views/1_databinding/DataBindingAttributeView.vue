<template>
  <div>
    <input type="text" v-model="userId" readonly /> <br />
    <input type="text" v-bind:value="userId" readonly /> <br />
    <input type="text" :value="userId" readonly /> <br />
    <img :src="imgSrc" alt="" style="width: 100; height: auto" /> <br />
    <input type="search" name="" id="" v-model="txt1" />
    <button :disabled="txt1 === ''">조회</button>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      userId: 'dad',
      imgSrc:
        'https://search.pstatic.net/sunny/?src=https%3A%2F%2Fi.pinimg.com%2Foriginals%2F42%2F91%2Ff0%2F4291f0c3635094ebff28555bfbeee23b.jpg&type=a340',
      txt1: ''
    }
  },
  setup() {},
  created() {},
  mounted() {},
  unmounted() {},
  methods: {}
}
</script>
