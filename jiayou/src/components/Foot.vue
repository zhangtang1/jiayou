<template>
    <ul class="box">
        <li>1. 每个微信号仅能为好友加油1次</li>
        <li>2. 300元抵现券：适用 6个月及以上的省心计划、爱融租 爱保理、爱收藏专享</li>
        <li>3. 适用 6个月及以上的省心计划、爱融租、爱保理</li>

        <img src="../assets/buchong.png" alt="">
    </ul>
</template>

<script>
    export default {
        data: function (){  
            return {

            }
        }
    }
</script>

<style lang="scss" scoped>
    .box {
        position: relative;
        background-color: #e4d5c0;
        text-align: left;
        padding: 4%;
        padding-top: 20%;
        padding-bottom: 8%;
        font-size: .875rem;
        color: #702200;
        line-height: 1.6;

        &:before {
            content: '';
            height: 1px;
            width: 100%;
            position: absolute;
            left: 0;
            top: 4%;
            background-color: #c6b091;
        }

        img {
            width: 60%;
            position: absolute;
            top: -4%;
            left: 50%;
            transform: translateX(-50%);
        }
    }
</style>

