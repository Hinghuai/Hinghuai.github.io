<template>
<div class="center">
  <el-input class="search" v-model="search" placeholder="模糊搜索"></el-input>
  <div class="box">
    <list :search='search'></list>
  </div>
</div>
</template>

<script>
import List from '@/components/list'

export default {
  data: () => {
    return {
      search: '',
    }
  },
  components: {
    List,
  },
}
</script>

<style scoped>
.box {
  margin: 20px;
  box-shadow: 0 2px 12px 0 rgba(0, 0, 0, 0.1);
}

.search {
  margin: 20px;
  width: 80%;
}

.center {
  text-align: center;
}
</style>