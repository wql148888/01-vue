<template>
<div>
    <div class="category_wrap">
        <div class="category_left_pic ">
            <span class="iconfont icon-icon-xiaomiguishu"></span>
        </div>
        <div class="category_middle_list">
            <div class="category_middle_list_item" v-for="(item,index) in list" :key=index>{{item}}</div>
            <!-- <div class="category_middle_list_item">红米手机</div> -->
        </div>
        <div class="category_right">
            <input type="text" name="" placeholder="冰箱"><button class="iconfont icon-sousuo" ></button>
        </div>
    </div>
</div>
</template>

<script>

export default {
  data () {
    return {
    list: ['Xiaomi手机','Redmi红米','电视','笔记本','家电','路由器','服务','社区']
}
  },
}
</script>

<style>
    .category_wrap {
        display: flex;
        height: 100px;
        /* background: pink; */
    }
    .category_left_pic {
        position: relative;
        flex: 3;
        /* padding: 0 0 0 10px; */
        color: #ff6a00;
        /* background: pink; */
    }
    .category_left_pic span {
        /* margin: 0 10px 0 10px; */
        position: absolute;
        left: 176px;
        top: 28px;
        font-size: 53px;
    }
    .category_middle_list {
        display: flex;
        flex: 8;
        padding: 0 74px;
        height: 100%;
        line-height: 100px;
        /* text-align: center; */
        /* background: yellow; */
    }
    .category_middle_list_item {
        padding: 0 10px;
    }
    .category_right {
        position: relative;
        flex: 4;
        padding: 26px 0;
        /* background: orange; */
    }
    .category_right input {
        padding: 5px 8px;
        height: 31px;
        width: 225px;
    }
    .category_right button {
        position: absolute;
        top: 26px;
        left: 244px;
        height: 45px;
        width: 50px;
        line-height: 8px;
        text-align: center;
        background: #fff;
        border: 1px solid #333;
    }
</style>
