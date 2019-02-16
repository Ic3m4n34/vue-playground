<template>
  <div class="child-component"><slot :useMe="data" /></div>
</template>

<script>
import AnotherComponent from '@/components/another-component';

export default {
  name: 'ChildComponent',
  components: {
    AnotherComponent
  },
  data() {
    return {
      data: 'Child Components Data'
    };
  }
};
</script>

<style lang="scss" scoped>
.child-component {
  background: grey;
}
</style>
