<template>
  <el-table :data="tableData" border stripe show-summary style="width: 600px;background-color: #252525;"  height="750">
    <el-table-column prop="date" label="日期" width="200px">
    </el-table-column>
    <el-table-column prop="exchange" label="交易所" width="200px">
    </el-table-column>
    <el-table-column prop="money" label="收支金额(￥)" width="200px">
    </el-table-column>
  </el-table>
</template>

<script>
  import Vue from 'vue'
  import {
    Table,
    TableColumn
  } from 'element-ui'
  import tableData from '@/assets/json/tableData.js'
  Vue.use(Table)
  Vue.use(TableColumn)
  export default {
    name: 'HomePage',
    data() {
      return {
        tableData
      }
    },
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h1,
  h2 {
    font-weight: normal;
  }

  ul {
    list-style-type: none;
    padding: 0;
  }

  li {
    display: inline-block;
    margin: 0 10px;
  }

  a {
    color: #42b983;
  }

</style>
