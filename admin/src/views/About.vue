<template>
  <div class="orderItem">
    <div class="oderNumber">11</div>
    <div class="Right">
      <div class="orderRight">
        <div class="oderName">姓 名：果冻</div>
        <div class="oderPhone">电话号码：15770550320</div>
        <div class="oderAddess">收货地址：address</div>
        <div class="oderTime">发布时间：2019-11-08</div>
      </div>
      <div class="orderBtn">接单</div>
    </div>
  </div>
</template>



<script>
export default {
  name: 'About',
  data() {
    return {}
  }
}
</script>


<style>
.orderItem {
  font-size: 1rem;
  display: flex;
  justify-content: space-between;
}
.oderNumber {
  border: 1px solid blue;
  width: 10px;
  height: 10px;
  padding: 2px;
  border-radius: 50%;
  background: red;
}
.orderRight {
  border: 1px solid red;
}
.orderBtn {
  height: 50px;
  border: 1px solid yellow;
  display: flex;
  align-items: center;
}
.Right {
  display: flex;
  align-items: center;
}
</style>
