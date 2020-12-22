<template>
  <div>
    <div class="container">
      <div class="item" v-for="(item , index) in itemList" :key="index">
        {{item.title}}
      </div>
    </div>
  </div>
</template>


<script>
export default {
  data() {
    return {
      itemList: [
        {title: '测试'},
        {title: '测试'},
        {title: '测试'},
        {title: '测试'},
        {title: '测试'},
      ]
    }
  }
};
</script>

<style lang="scss" scoped>
.container {
  display: flex;
  align-items: center;
  padding: 0 .24rem;
  flex-wrap: wrap;
  justify-content: space-between;
  .item {
    width: .9rem;
    height: .9rem;
    background-color: pink;
    font-size: .16rem;
  }
}
</style>