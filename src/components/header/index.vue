<template>
    <div id="header">
        <header>
            <div class="icon search">
                <Icon size='20' type='search' />
            </div>
            <div class="text">
                <h3>Management Task</h3>
                <p>We make your projects happen!</p>
            </div>
            <div class="icon user">
                <Icon size="20" type="success" />
            </div>
        </header>
        <div class="slide">
            <div class="item todo active">
                <span>To do</span>
            </div>
            <div class="item progress">
                <span>In progress</span>
            </div>
            <div class="item completed">
                <span>Completed</span>
            </div>
        </div>
    </div>
</template>

<script setup lang="ts">
import { Icon } from '@tarojs/components';
</script>

<style scoped lang="scss">
::-webkit-scrollbar{
    opacity: 0;
}
#header{
    background-color: #F6F9FF;
    border-bottom-left-radius: 60px;
    border-bottom-right-radius: 60px;
    padding-bottom: 20px;
    header{
        padding: 50px 40px;
        display: flex;
        justify-content: space-between;
        align-items:flex-start;
    }
    .icon{
        height: auto;
        display: inline-block;
        width: 88px;
        height: 88px;
        background-color: #FFFFFF;
        display: flex;
        justify-content: center;
        align-items: center;
        border-radius: 15px;
    }
    
    .search{

    }
    .text{
        text-align: center;
        h3{
            font-size: 40px;
        }
        p{
            font-size: 13px;
        }
    }
    .user{}

    .slide{
        width: 100%;
        margin: 30px 40px;
        overflow-y: scroll; 
        white-space: nowrap;
        
        .item{
            width: auto;
            height: 84px;
            margin-right: 30px;
            display: inline-flex;
            align-items: center;
            justify-content: center;
            border-radius: 15px;
            background-color: #FFFFFF;
            padding: 0 80px;
            &.active{
                background-color: #3E7FFF;
                color: #FFFFFF;
            }
        }
        span{
            font-size: 15px;
        }
    }
}

</style>