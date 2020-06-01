<template>
  <div id="root">
      <p>{{ originalPrice }}</p>
      <p>{{ doublePrice }}</p>
      <p>{{ triplePrice }}</p>
  </div>
</template>

<script>
import { mapGetters } from 'vuex';
export default {
    computed: {
        ...mapGetters(['originalPrice', 'doublePrice', 'triplePrice'])
    }
    // 위 코드 == 아래 코드: 헬퍼 함수가 주는 간편함~
    // computed: {
    //     originalPrice() {
    //         return this.$store.getters.originalPrice;
    //     },
    //     doublePrice() {
    //         return this.$store.getters.doublePrice;
    //     },
    //     triplePrice() {
    //         return this.$store.getters.triplePrice;
    //     }
    // }
}
</script>

<style>

</style>