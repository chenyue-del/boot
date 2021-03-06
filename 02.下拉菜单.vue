<template>
  <div>
    <el-select v-model="svalue" filterable>
      <el-input placeholder="搜索" prefix-icon="el-icon-search" size="mini" > </el-input>
      
      <el-option
        v-for="item in options"
        :key="item.value"
        :label="item.label"
        :value="item.value">
        <input type="checkbox">
      </el-option>
    </el-select>
  </div>
</template>

<script>
  export default {
  data() {
    return {
      selectedArray: [],
      options: [
        { name: '1', label: '变更中' },
        { name: '2', label: '未生效' },
        { name: '3', label: '作废' },
        { name: '4', label: '正常' },
        { name: '5', label: '审核中' }
      ]
    }
  }
}
</script>

<style>

</style>