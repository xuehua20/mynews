<template>
  <div class="list">
    <ul>
      <li @click="data.add">
        <p>{{ data.name }}</p>
        <p>{{ data.user }}</p>
        <i class="iconfont iconjiantou1"></i>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  //接收父组件传的值
  props: ["data", "index"]
};
</script>
<style lang="less" scoped>
.list {
  ul {
    font-size: 0.253333rem;
    li {
      display: flex;
      height: 0.8rem;
      line-height: 0.8rem;
      border-bottom: 0.013333rem solid #e4e4e4;
      p {
        flex: 1;
        margin-bottom: 0rem;
      }
      :nth-child(2) {
        text-align: right;
      }
      i {
        font-size: 0.333333rem;
        padding-left: 0.333333rem;
      }
    }
  }
}
</style>
