<template>
    <div>
        <img v-if="url" src="../assets/redbar.png" alt="">

        <p v-for="(item, index) in wordArr">
            {{ item }}
        </p>
    </div>
</template>

<script>
    export default {
        name: 'Line',

        data: function () {  
            return {
                wordArr: [
                    '点击“开始集油”按钮，每获1位好友“加油”，下方抵现券起用金额立减1000元(最高可减至20000元)需满足3个及以上好友加油后，才可领取。',
                ],

                url: '../assets/redbar.png',
            }
        },
    }
</script>

<style scoped>
    div {
        font-size: 1rem;
        color: #702200;
        padding: 3% 3% 0 3%;
        line-height: 1.5;
        position: relative;
    }

    img {
        width: 66%;
        position: absolute;
        left: 50%;
        top: -4%; 
        transform: translate(-50%, -50%);
    }

    p {
        margin: 1rem 0;
    }
</style>

