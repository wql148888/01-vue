<template>
<div>
    <div class="nav_wrap">
        <div class="nav_left">
        <div class="nav_left_item" v-for = "(item,index) in list" :key=index>{{item}}</div>
        <!-- <div class="nav_left_item">有品</div> -->
    </div>
    <div class="nav_right">
        <div class="nav_right_login">登录</div>
        <div class="nav_right_register">注册</div>
        <div class="nav_right_car">消息通知</div>
    </div>
    </div>
</div>
</template>

<script>

export default {
  data () {
    return {
    list: ['小米商城','MIUI','loT','云服务','天星数科','有品','小爱开放平台','企业团购','资质证照','协议规则','下载app','Select Location']
}
  },
}
</script>

<style>
.nav_wrap {
    display: flex;
    justify-content: space-between;
    height: 33px;
    line-height: 18px;
    background: #333;
    color: #a4a3a3;
    font-size: 10px;
}
.nav_left,
.nav_right {
    display: flex;
    padding: 0 155px;
}
.nav_left_item {
    padding: 0 10px;
    margin: 8px 0;
    border-right: 1px solid #5f6368;
}
.nav_left_item:hover {
    color: #fff;
}

</style>
