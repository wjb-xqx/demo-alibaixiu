<template> 
    <div class="comAside clearfix">
        <!-- 搜索 -->
        <div class="widgets clearfix">
            <h4>搜索</h4>
            <div class="body">
                <form action="">
                    <input type="text" placeholder="输入关键字" class="keys">
                    <input type="submit" value="搜索" class="btn">
                </form>
            </div>
        </div>
        <!-- 随机推荐 -->
        <div class="widgets clearfix">
            <h4>随机推荐</h4>
            <div class="body random clearfix">
                <ul>
                    <li>
                        <div class="left">
                            <p class="title">废灯泡的14种玩法 妹子见了都会心动</p>
                            <p class="reading">阅读(819)</p>
                        </div>
                        <div class="rightImg">
                            <img src="@/assets/images/widget_2.jpg" alt="">
                        </div>
                    </li>
                    <li>
                        <div class="left">
                            <p class="title">废灯泡的14种玩法 妹子见了都会心动</p>
                            <p class="reading">阅读(819)</p>
                        </div>
                        <div class="rightImg">
                            <img src="@/assets/images/widget_2.jpg" alt="">
                        </div>
                    </li>
                    <li>
                        <div class="left">
                            <p class="title">废灯泡的14种玩法 妹子见了都会心动</p>
                            <p class="reading">阅读(819)</p>
                        </div>
                        <div class="rightImg">
                            <img src="@/assets/images/widget_2.jpg" alt="">
                        </div>
                    </li>
                    <li>
                        <div class="left">
                            <p class="title">废灯泡的14种玩法 妹子见了都会心动</p>
                            <p class="reading">阅读(819)</p>
                        </div>
                        <div class="rightImg">
                            <img src="@/assets/images/widget_2.jpg" alt="">
                        </div>
                    </li>
                    <li>
                        <div class="left">
                            <p class="title">废灯泡的14种玩法 妹子见了都会心动</p>
                            <p class="reading">阅读(819)</p>
                        </div>
                        <div class="rightImg">
                            <img src="@/assets/images/widget_2.jpg" alt="">
                        </div>
                    </li>
                </ul>
            </div>
        </div>
        <!-- 最新评价 -->
        <div class="widgets clearfix">
            <h4>最新评价</h4>
            <div class="body discuz clearfix">
                <ul>
                    <li>
                        <div class="avatar">
                            <img src="@/assets/images/avatar_1.jpg" alt="">
                        </div>
                        <div class="text">
                            <p><span>鲜活</span>9个月前(08-14)说:</p>
                            <p>挺会挺会玩的挺会玩的挺会玩的挺会玩的玩的</p>
                        </div>
                    </li>
                    <li>
                        <div class="avatar">
                            <img src="@/assets/images/avatar_1.jpg" alt="">
                        </div>
                        <div class="text">
                            <p><span>鲜活</span>9个月前(08-14)说:</p>
                            <p>挺会挺会玩的挺会玩的挺会玩的挺会玩的玩的</p>
                        </div>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:"comAside",
    data(){
        return{
            
        }
    },
    mounted () {
        // window.addEventListener('scroll', this.handleScroll, true);  
         // 监听（绑定）滚轮 滚动事件
    },
    methods:{
         handleScroll(){
            // var scrollTop = window.pageYOffset || document.documentElement.scrollTop 
            // || document.body.scrollTop
            //  var offsetTop = this.$refs.widgets.offsetTop
            //  if (scrollTop > offsetTop) {
            //    this.searchBarFixed = true
            //  } else {
            //    this.searchBarFixed = false
            //  }
        }
    }
}
</script>

<style lang="less" scoped>
.comAside{
    float: left;
    margin-left: -320px;
    width: 300px;
    height: 500px;
    position: relative;
    // background-color: #fff;
    padding: 20px 0 20px 20px;
    >.widgets{
        padding: 15px 20px;
        background-color: #fff;
        overflow: hidden;
        >h4{
            margin-bottom: 5px;
            font-size: 20px;
            border-bottom: 2px solid #ff5e52;
            display: inline-block;
            }
        >.body{
            margin-top: 10px;
                >form{
                    width: 100%;
                    display: inline-block;
                    height: 34px;
                    position: relative;
                     >.keys{
                         width: 190px;
                         height: 34px;
                         border: 2px solid #ccc;
                         border-right: 0 none;
                         outline: none;
                         float: left;
                         overflow: hidden;
                         padding-left: 5px;
                     }
                     >.btn{
                         position: absolute;
                         top: 0;
                         right: 0;
                         width: 70px;
                         height: 34px;
                         text-align: center;
                         color: #fff;
                         border: 0 none;
                         background-color: #ff5e52;
                         opacity: 0.85;
                     }
                 }
        }
        >.random{
            >ul{
                height: 100%;
                >li{
                    height: 80px;
                    display: flex;
                    border-bottom: 1px solid #ccc;
                     padding: 10px 0;
                     cursor: pointer;
                    >.left{
                        flex:1;
                        >.title{
                            width: 160px;
                             font-size: 14px;
                             color: #444;
                        }
                        >.reading{
                            font-size: 12px;
                            color: #999;     
                        }
                    }
                    >.rightImg{
                        width: 70px;
                        >img{
                            width: 100%;
                            height: 53px;
                        }
                    }
                    &:hover{
                        .title{
                            color:red;
                        }
                    }
                }
            }
        }
        >.discuz{
            >ul{
                height: 100%;
                >li{
                    height: 60px;
                    padding: 10px 0;
                    border-bottom: 1px solid #ccc;
                    cursor: pointer;
                    >.avatar{
                        width: 40px;
                        height: 40px;
                        border-radius: 20px;
                        overflow: hidden;
                        float: left;
                        >img{
                            width: 100%;
                            height: 100%;
                        }
                    }
                    >.text{
                        float: right;
                        padding-left: 5px;
                        width: 200px;
                        span{
                            color: #666;
                             margin-right: 5px;
                        }
                        >p{
                            overflow: hidden;
                            text-overflow:ellipsis;
                            white-space: nowrap;
                        }
                    }
                }
            }
        }
    }
}
</style>
