<template>
    <div class="box">
        <img src="../assets/youtong.png" alt="">
        
        <div class="cnt">
            <div class="quan">
                <img src="../assets/quanbg.png" alt="">
                <div class="cnt">
                    <div>￥{{ quan }}</div>
                    <div>
                        <h3>{{ qiyong }}</h3>
                        <button class="btn">立即领券</button>
                    </div>
                </div>
            </div>

            <div class="tip">
                <div class="banner">
                    <p>已收到 <b>3</b> 位好友加油</p>
                    <p>起用金额降至 <b>37000</b> 元</p>
                </div>
            </div>

            <div class="staff">
                <div class="leftBox">
                    <div>
                        <p>集邮</p>
                        <p>进度</p>
                    </div>

                    <div>
                        <p>起用</p>
                        <p>金钱</p>
                    </div>
                </div>

                <img src="../assets/staff.png" alt="">

                <div class="info">
                    <div class="item" v-for="i in 20" :class="{ show: i==num }">
                        <div v-if="i<=num"></div>
                    </div>
                </div>
            </div>
        </div>

        <img src="../assets/share.png" alt="">
    </div>
</template>

<script>
    export default {
        data: function () { 
            return {
                
            }
        },

        props: ['quan', 'qiyong', 'num'],
    }
</script>


<style lang="scss" scoped>
    div {
        box-sizing: border-box;
    }
    .box {
        font-size: 0;
        position: relative;
        padding-bottom: 20%;

        >img:first-child {
            width: 92%;
        }
        >img:last-child {
            width: 84%;
            position: absolute;
            z-index: 10;
            bottom: 3.7%;
            left: 50%;
            transform: translateX(-50%);

            &:active {
                opacity: .5;
            }
        }

        .cnt {
            position: absolute;
            top: 0;
            left: 0;

            .quan {
                margin-top: 23%;
                position: relative;
                                
                img {
                    width: 84%;
                }

                .cnt {
                    position: absolute;
                    display: flex;
                    font-size: 20px;
                    height: 100%;
                    width: 84%;
                    left: 50%;
                    transform: translateX(-50%);
                    // justify-content: center;
                    align-items: center;

                    >:first-child {
                        width: 61.5%;
                        color: #e74f44;
                        font-size: 2.4rem;
                        font-weight: bold;
                        padding-right: 7%;
                        padding-top: 5%;
                    }
                    >:last-child {
                        width: 30%;
                        flex: 1 1 auto;
                        color: #862b03;

                        h3 {
                            margin-top: 10%;
                            margin-bottom: 10%;
                        }

                        .btn {
                            border: 1px solid #862b03;
                            font-size: .875rem;
                            color: #862b03;
                            box-sizing: border-box;
                            padding: 3px 16px;
                            height: 1.6rem;
                            background-color: #ffd732;
                            border-radius: 1rem;
                            display: flex;
                            align-items: center;
                            margin: 0 auto;
                            outline: none;

                            &:active {
                                opacity: .5;
                            }
                        }
                    }
                }
            }

            .tip {
                font-size: 1rem;
                width: 92%;
                margin: 6% auto 0 auto;
                
                .banner {
                    padding: 10px;
                    display: inline-block;
                    background-color: rgba(255, 255, 255, .4);
                    color: #fff;
                    border-radius: 4px;

                    p {
                        margin: 0;
                        line-height: 1.5rem;
                    }
                }
            }

            .staff {
                font-size: 1rem;
                display: flex;
                align-items: center;
                width: 92%;
                margin: 4% auto 0 auto;
                position: relative;

                img {
                    width: 78%;
                }

                .leftBox {
                    flex: 0 0 16%;
                    font-size: .875rem;
                    color: #c02d25;
                    font-weight: bold;

                    p {
                        margin: 0;
                    }
                }

                .info {
                    position: absolute;
                    right: 10%;
                    top: 7%;
                    color: #fff;
                    display: flex;
                    width: 70%;
                    height: 36.5%;
                    align-items: center;

                    .item {
                        height: 80%;
                        flex: 0 0 4%;
                        margin-left: 1%;
                        background-color: #cacaca;
                        border-radius: 2px;
                        position: relative;

                        &:first-child {
                            margin-left: 0;
                        }

                        &:before {
                            content: '';
                            position: absolute;
                            border: 6px solid transparent;
                            border-top: 6px solid rgba(255, 255, 255, .4);
                            width: 0;
                            top: -102%;
                            display: none;
                        }

                        div {
                            position: absolute;
                            top: 0;
                            left: 0;
                            right: 0;
                            bottom: 0;
                            background-color: #e9ac0e;
                            border-radius: 2px;
                        }
                    }

                    .show {
                        &:before {
                            display: block;
                        }
                    }
                }
            }
        }
    }
</style>

