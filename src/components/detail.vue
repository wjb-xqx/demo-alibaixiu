<template>
    <div class="detail">
        <div class="container clearfix">
            <com-header></com-header>
            <div class="content-wrap">
                <div class="content">
                    <div class="article-header">
                        <div class="breadcrumbs">
                            <span>当前位置：</span>
                            <a href="#">wjb</a>
                            &nbsp;>&nbsp;
                            <a href="#">生活馆</a>&nbsp;>&nbsp;
                            <span>正文</span>
                        </div>
                        <div class="article-title">
                            <h1>关于指甲的10个健康知识 你知道几个？</h1>
                        </div>
                        <ul class="article-meta">
                            <li>alibaixiu 发布于 2015-11-23</li>
                            <li>分类：<a href="#">生活馆</a></li>
                            <li>阅读(2645)</li>
                            <li>评论(1)<a href="#">知道日报</a></li>
                        </ul>
                    </div>
                    <!-- 内容 -->
                    <div class="article-content">
                            <p><img src="@/assets/images/115249j8p27p3jps9h05pw.jpg" alt=""></p>
                            <p>11月12日起，100元人民币将换新颜。昨日，南都记者从广州市内多家银行了解到，根据中国人民银行安排，2015年版第五套人民币100元纸币12日正式发行。新版百元纸币主色调、主图案、尺寸规格不变，主要是提升防伪性和印刷质量，首次采用国际钞票防伪领域公认的前沿防伪技术———光彩光变技术。正因该技术可将纸币上的面值数字和安全线的颜色随光线角度不同发生变化，业界还称此类纸币为“会发光的钞票”。</p>
                            <p class="post-copyright">未经允许不得转载：wjb</p>

                    </div>
                    <div class="article-social">
                        <a href="JavaScript:;">
                            <i class="icon iconfont icon-zan"></i> 
                            赞 (<span>10</span>) 
                        </a>
                    </div>
                    <!-- 相关推荐 -->
                    <div class="hot clearfix">
                        <h3>相关推荐</h3>
                        <ul>
                            <li>
                                <a href="#">
                                    <img src="@/assets/images/hots_4.jpg" alt="">
                                    <span>星球大战:原力觉醒视频演示 电影票68</span>
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    <img src="@/assets/images/hots_4.jpg" alt="">
                                    <span>星球大战:原力觉醒视频演示 电影票68</span>
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    <img src="@/assets/images/hots_4.jpg" alt="">
                                    <span>星球大战:原力觉醒视频演示 电影票68</span>
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    <img src="@/assets/images/hots_4.jpg" alt="">
                                    <span>星球大战:原力觉醒视频演示 电影票68</span>
                                </a>
                            </li>
                        </ul>
                    </div>
                    <!-- 评论 -->
                    <h3 class="title"><strong>评论</strong><b>0</b> </h3>
                    <div class="no_webshot">
                        <form action="">
                            <div class="comt-title">
                                <img src="@/assets/images/avatar_1.jpg" alt="">
                            </div>
                            <div class="comt">
                                <div class="comt-box">
                                    <textarea placeholder="你的评论可以一针见血" cols="100%" rows="3" tabindex="1">
                                    </textarea>
                                    <div class="comt-ctrl">
                                        <button> 提交评论</button>
                                    </div>
                                </div>
                            </div>
                        </form>
                    </div>
                    <div class="comt-comterinfo">
                        <ul>
                            <li>
                                <label for="author"></label>
                                <input type="text" placeholder="昵称">
                                <span>昵称 (必填)</span>
                            </li>
                            <li>
                                <label for="author"></label>
                                <input type="text" placeholder="邮箱">
                                <span>邮箱 (必填)</span>
                            </li>
                            <li>
                                <label for="author"></label>
                                <input type="text" placeholder="网址">
                                <span>网址</span>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
            <com-aside></com-aside>
        </div>
    </div>
</template>

<script>
import comHeader from './common/comHeader'
import comAside from './common/comAside'
export default {
    name:"detail",
    components:{
        comHeader,
        comAside
    }
}
</script>

<style lang="less" scoped>
.content-wrap{
    width: 100%;
    float: left;
    .content{
        margin-right: 320px;
        margin-left: 190px;
        padding: 20px 25px 0;
        min-height: 800px;
        overflow: hidden;
        background-color: #fff;
    }
    // 头部
    .article-header{
        padding: 0 0 12px;
        border-bottom: 1px solid #eee;
        margin-bottom: 20px;  
        >.breadcrumbs{
            padding: 5px 0 10px;
            font-size: 12px;
            text-align: left;
            >span{
                 font-size: 12px;
                  margin-bottom: 0;
             }
        }
        >.article-title{
            font-size: 26px;
            margin-top: 5px;
            line-height: 1.2;
         }
         >.article-meta{
             overflow: hidden;
             color: #999;
             font-size: 12px;
             margin-top: 10px;
             >li{
                 float: left;
                 margin-right: 20px;
             }
         }
    }
    .article-content{
        margin: 20px 0;
        font-size: 15px;
        >p{
            margin-bottom: 20px;
            >img{
                width: 400px;
                height: 266px;
                display: block;
                margin: 0 auto;
                text-align: center;
            }
        }
        >.post-copyright{
            background-color: #f2f2f2;
            font-size: 12px;
            color: #999;
            padding: 6px 15px 5px;
            border-radius: 2px;
            text-align: center;
            margin-top: 10px;
        }
    }
    .article-social{
        padding: 30px 0;
        text-align: center;
        >a{
            display: inline-block;
            background-color: #FF5E52;
            padding: 12px 25px;
            display: inline-block;
            border-radius: 2px;
            color: #fff;
            box-shadow: 0 0 2px rgba(0,0,0,.12);
        }
    }
    .title{
        position: relative;
        margin: 0;
        line-height: 32px;
        font-size: 20px;
        border-bottom: 2px solid #eee;
        >strong{
            border-bottom: 2px solid #FF5E52;
            display: inline-block;
            position: relative;
            bottom: -2px;
            font-weight: normal;
            margin-right: 3px;
        }
        >b{
            color: #429ad9;
            font-weight: normal;
        }
    }
    .no_webshot{
        background-color: #fff;
        >form{
            margin-bottom: 20px;
            padding-left: 60px;
            >.comt-title{
                width: 50px;
                float: left;
                margin-left: -60px;
                >img{
                    border-radius: 2px;
                    width: 50px;
                    height: 50px;
                }
            }
            >.comt{
                position: relative;
                >.comt-box{
                    border: 2px solid #CCD4D9;
                    border-radius: 2px;
                    padding: 4px;
                    >textarea{
                        width: 100%;
                        resize: none;
                        overflow-x: hidden;
                        overflow-y: auto;
                        border: none;
                        line-height: 22px;
                        font-size: 14px;
                        outline: 0;
                        margin-bottom: 2px;
                        height: 48px;
                        
                    }
                    >.comt-ctrl{
                        position: relative;
                        height: 34px;
                        background-color: #FAFAFA;
                        border-top: 1px solid #E6EAED;
                        margin: 0 -4px -4px -4px;
                        >button{
                            position: absolute;
                            right: -2px;
                            bottom: -2px;
                            border: none;
                            background: #429ad9;
                            border-right: 2px solid #429ad9;
                            border-bottom: 2px solid #429ad9;
                            padding: 0px 20px;
                            height: 36px;
                            color: #fff;
                            outline: 0;
                            border-radius: 0 0 2px 0;
                        }
                    }
                }
            }
        }
    }
    .comt-comterinfo{
            padding: 20px 0 0;
            color: #444;
            text-align: center;
            margin-bottom: 80px;
            >ul{
                width: 350px;
                text-align: left;
                margin: 0 auto;
                >li{
                    margin-bottom: 10px;
                    >label{
                        margin-bottom: 5px;
                        font-weight: bold;
                    }
                    >input{
                        margin-right: 10px;
                        position: relative;
                        *bottom: -3px;
                        border: 2px solid #CCD4D9;
                        border-radius: 2px;
                        height: 34px;
                        padding: 3px 5px;
                        outline: none;
                        width: 220px;
                        box-shadow: none;
                    }
                    >span{
                        color: #999;
                    }
                }
            }
    }
}
// 相关推荐
.hot{
    padding: 20px;
    >h3{
        display: inline-block;
        margin-bottom: 10px;
        line-height: 32px;
        font-size: 20px;
        font-weight: 600;
        border-bottom: 2px solid #ff5e52;
    }
    >ul{
        height: 100%;
        width: 100%;
        >li{
            display: inline-block;
            width: 24.5%;
            font-size: 14px;
            overflow: hidden;
            >a{
                display: inline-block;
                color: #666;
                >img{
                    height: 132px;
                    margin-bottom: 5px;
                }
                >span{
                    display: inline-block;
                    height: 40px;
                    overflow: hidden;
                }
            }
            &:hover{
                a{
                    color:#428bca;
                }
            }
        }
    }
}

</style>

