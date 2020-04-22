<template>
    <div class='header'>
        <div class="nav-topbar">
            <div class="container">
                <div class="top-menu">
                    <a href="javascript:;">小米商城</a>   <!-- javascript:;防止页面刷新   -->
                    <a href="javascript:;">MUI</a>
                    <a href="javascript:;">云服务</a>
                    <a href="javascript:;">协议规则</a>
                </div>
                <div class="topbar-user">
                    <a href="javascript:;">登录</a>   <!-- javascript:;防止页面刷新   -->
                    <a href="javascript:;">注册</a>
                    <a href="javascript:;" class="my-cart"><span class="icon-cart"></span>购物车</a>
                </div>
            </div>
        </div>
        <div class="nav-header"></div>

    </div>
</template>

<script>
export default {
    name:'nav-header',
}
</script>

<style lang='scss'>
    .header{
        .nav-topbar{
            height: 39px;
            line-height: 39px;
            background-color: #333333;
            color: #B0B0B0;
            .container{
                width: 1226px;
                margin-right: auto;   //margin-right 和 margin-left 都自动，居中设置
                margin-left: auto ;
                //定义布局方式：flex布局
                display: flex;
                // 水平方向居中
                justify-content: space-between;
                // 垂直方向居中
                align-items: center;
                // a标签的样式优先于class样式，所以上面 .nav-topbar的color样式没有显示，需要在a中自定义
                a{
                    display: inline-block;
                    color:#B0B0B0;
                    margin-right: 17px;
                }
                .my-cart{
                    width: 110px;
                    background-color: #FF6600;
                    text-align: center;
                    color:#ffffff;
                    .icon-cart{
                        display: inline-block;
                        width: 16px;
                        height: 12px;
                        background:url('/imgs/icon-cart-checked.png') no-repeat center;
                        background-size: contain;
                        margin-right: 4px;

                    }

                }


            }
        
        }
    }

</style>