<template>
    <div class="index">
        <div class="container clearfix">
            <com-header></com-header>
            <div class="content-wrap">
                <div class="content">
                    <div class="title">
                        <h1>生活馆</h1>
                        <div class="text">
                            分享转发世界各地各种最贴近生活的技巧方法和有趣的生活方式
                        </div>
                    </div>
                    <!-- 最新发布 -->
                    <div class="new">
                        <div class="entry entry-once">
                            <div class="head">
                                <a href="#">星球大战：原力觉醒视频演示 电影票68</a>
                                <p class="icon iconfont icon-tupian">5</p>
                            </div>
                            <p class="text-muted time">万林论 发布于 2015-11-30</p>
                            <p class="imgs">
                                <a href="#">
                                    <span><img src="@/assets/images/focus.jpg" alt=""></span>
                                </a>
                            </p>
                            <p class="note">2015年11月29日，四川成都，貌似马云的门卫柯全寿。日前，在新鸿路南一巷一小区内，一名叫柯全寿的门卫被许多小区住户认为其长相貌似阿里巴巴总裁 ...</p>
                            <div class="text-muted">
                                <span class="post-views">阅读(6993)</span>
                                <span class="post-comments">评论(19)</span>
                                <a href="#" class="like"><span class="icon iconfont icon-zan"></span>赞(964)</a>
                                <span class="post-tags">标签：
                                    <a href="#" title="查看奇趣事的文章">奇趣事</a>&nbsp;/&nbsp;<a href="#" title="查看会生活的文章">会生活</a>
                                </span>
                            </div>
                        </div>
                    </div>
                    <!-- 更多 -->
                    <div class="ias_trigger">More</div>
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
    name:"index",
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
}
.title{
        overflow: hidden;
    clear: both;
    background-color: #f9f9f9;
    text-align: center;
    padding: 30px 20px;
    border-bottom: 1px solid #eee;
    >h1{
        font-size: 22px;
        line-height: 1;
        position: relative;
    }
    >.text{
        overflow: hidden;
        position: relative;
        margin-top: 15px;
        color: #999;
        font-size: 14px;
        
    }
}
// 最新发布
.new{
    margin-bottom: 20px;
    padding: 20px;
    .entry{
        padding: 10px 0;
        border-bottom: 1px solid #eee;
        >.head{
           height: 30px;
           line-height: 1;
           padding: 5px 0;
           margin: 8px 0 10px 0;
           box-sizing: border-box;
           font-size: 22px;
           color: #444;
           >a{
               color: #444;
               float: left;
               transition: all 0.5s;
               &:hover{
                   color:red;
               }
            }
            >p{
                float: left;
                padding-left: 5px;
                padding-top: 3px;
            }
        }
        >.text-muted{
            font-size: 12px;
        }
        >.imgs{
            margin: 10px 0;
            >a{
                display: inline-block;
                >span{
                    display: inline-block;
                    width: 166px;
                    >img{
                        width: 100%;
                        height: 132px;
                        &:hover{
                           opacity: .6;
                        }
                    }
                }
            }
        }
        >.note{
            color: #777;
            font-size: 14px;
            line-height: 22px;
            margin-bottom: 10px;
        }
        >.text-muted{
            margin-bottom: 10px;
            >span{
                margin-right: 20px;
            }
           .like:hover{
               color: #428bca;
           }
           a:hover{
                color: #428bca;
           }
        }
    }
    >.entry-once{
        padding: 10px 0 40px 0;
        >span{
            margin-right: 25.3%;
        }
        >.imgs{
            float: right;
            width: 25.3%;
            margin-top: -23px;
        }
    }
}
// 更多
.ias_trigger{
    margin: 20px 0;
    background-color: #eee;
    display: block;
    line-height: 35px;
    text-align: center;
    font-size: 14px;
    color: #999;
    cursor: pointer;
    &:hover{
        background-color: #ddd;
        color: #666;
    }
}

</style>

