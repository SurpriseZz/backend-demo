<template>
  <div>
    <el-dialog v-model="showComponent" @open="onOpen">111111</el-dialog>
  </div>
</template>
<script setup>
import { ElDialog } from "element-plus";
import { ref } from "vue";
const showComponent = ref(false)
const name = ref("customModal");
const show = () => {
  showComponent.value = true
}
defineExpose({
  name,
  show,
});
</script>
  