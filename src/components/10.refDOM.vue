<template>
  <div>
    <h3 ref="h3Ref">啊啊啊啊，。五环</h3>
  </div>
</template>

<script>
import { ref, onMounted } from "@vue/composition-api";

export default {
  setup() {
    const h3Ref = ref(null);

    onMounted(() => {
      console.log(h3Ref.value);
      h3Ref.value.style.color = "red";
    });

    return {
      h3Ref
    };
  }
};
</script>