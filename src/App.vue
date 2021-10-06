<script lang="ts">
import { defineComponent, h } from 'vue';
import catImg from '@/assets/images/cat.jpg';

export default defineComponent({
  render() {
    const vnode = h(
      'div',
      { class: 'circle' },
      [h('img', { src: catImg })],
    );
    return vnode;
  },
});
</script>

<style scoped>
.circle {
  background: #000;
  width: 100px;
  height: 100px;
  border-radius: 100%;
}
</style>