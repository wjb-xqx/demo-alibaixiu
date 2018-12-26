<template>
    <div class="header  clearfix">
        <div class="logo">
            <a href="/" title="发现生活，发现美">
                <!-- <img src="@/assets/logo.png" alt=""> -->
            </a>
        </div>
        <ul class="nav clearfix">
            <router-link to="/list" tag="li"><span class="iconfont icon-icon-test"></span> 奇趣事</router-link>
            <li><span class="iconfont icon-dianhua"></span>潮科技</li>
            <li><span class="iconfont icon-shenghuoyongshui"></span>会生活</li>
            <li><span class="iconfont icon-liwu"></span>美奇迹</li>
        </ul>
        <form action="">
            <input type="text" placeholder="请输入关键字" class="form-control">
            <input type="submit" value="" class="icon iconfont btn">
        </form>
    </div>
</template>

<script>
export default {
    name:"comHeader"
}
</script>

<style lang="less" scoped>
.header{
    position: fixed;
    top: 0;
    bottom: 0;
    width: 190px;
    z-index: 99;
    height: 397px;
    background-color: #f6f6f6;
    >.logo{
        width: 190px;
        height: 120px;
        >a{
            display: block;
            width: 100%;
            height: 100%;
            background-color: #428bca;
            >img{
                 width: 100%;
                 height: 100%;
            }
        }
    }
    >.nav{
        width: 100%;
        margin: 20px 0;
        >li{
            font-size: 16px;
            height: 44px;
            line-height: 44px;
            padding-left: 35px;
            cursor: pointer;
            &:hover{
                background-color: #fff;
            }
            >span{
                padding-right: 8px;
            }
        }
    }
    >form{
        height: 44px;
        width: 160px;
        position: relative;
        margin: 0 auto;
        >.form-control{
            width: 115px;
            height:34px;
            border: 1px solid #ccc;
            padding-left: 5px;
        }
        >.btn{
            width: 48px;
            height: 34px;
            position: absolute;
            right: 0;
            top: 0;
            background-color: #428bca;
            color:#fff;
        }
    }
}
</style>



