<template>
  <div>
    <el-form-item label="提示语：">
      <el-input v-if="inputForm.rules" v-model="inputForm.options.placeholder" />
    </el-form-item>
    <el-form-item label="数据校验：">
      <el-checkbox v-model="inputForm.checked">必须从组织结构人员里选择</el-checkbox>
    </el-form-item>
  </div>
</template>
<script>

export default {
  props: {
    inputForm: {
      type: Object,
      default: () => {}
    }
  },
  data() {
    return {}
  }
}
</script>
<style scoped></style>
