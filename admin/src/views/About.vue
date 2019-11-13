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
      <svg width="0" height="0" style="display: none">
                <filter id="filter">
                    <feTurbulence type="fractalNoise" baseFrequency=".01" numOctaves="4" />
                    <feDisplacementMap in="SourceGraphic" scale="100" />
                </filter>
        </svg>
        <div class="button-box">
                <div class="back"></div>
            <span class="text">hover</span>
        
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





:root {
            --height: 100px;
            --width: 200px;
        }
.button-box {
            width: 200px;
            height: 70px;
            box-shadow: 2px 2px 5px #ccc;
            text-align: center;
            line-height: 70px;
            cursor: pointer;
            position: relative;
            overflow: hidden;
        }

        .button-box .text {
            color: rgb(15, 240, 221);
            text-transform: uppercase;
            font-weight: bold;
            font-size: 23px;
            position: relative;
            z-index: 5;
            transition: all 2.5s cubic-bezier(0.1, 0.22, 0.3, 1);
        }
        .button-box:hover .text{
            color: white;
        }
        .button-box .back {
            position: absolute;
            left: -50%;
            bottom: -50%;
            width: 0;
            height: 0;
            filter: url(#filter);
            border-radius: 50%;
            z-index: 5;
            transition: all 2.5s cubic-bezier(0.1, 0.22, 0.3, 1);
            background: #0dbb55;
        }

        .button-box:hover .back {
            width: calc(2 * var(--width)) !important;
            height: calc(2 * var(--height)) !important;
        }
</style>
