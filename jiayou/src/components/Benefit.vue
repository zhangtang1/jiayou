<template>
    <div class="box">
        <img src="../assets/introduce.png" alt="">

        <div class="cnt">
            <p>好友（非爱投资用户）打开您分享的链接“加油”后，可获得10元~2017元随机现金，现金将放入Ta的爱投资账户余额，可随时投资或提现。</p>
            <p>好友“加油”随机现金奖共10万元，送完活动结束。</p>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'benefit',

        data: function () {  
            return {

            }
        }
    }
</script>

<style lang="scss" scoped>
    .box {
        position: relative;
        margin-bottom: 10%;
    }

    img {
        width: 92%;
    }

    .cnt {
        font-size: .875rem;
        position: absolute;
        top: 27%;
        left: 50%;
        width: 80%;
        transform: translateX(-50%);
        padding: 20px;
        text-align: left;
        line-height: 1.6;

        p {
            margin-bottom: .6rem;
            color: #873917;
        }
    }
</style>
