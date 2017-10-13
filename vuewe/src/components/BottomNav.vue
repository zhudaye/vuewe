<template>
	<div class="weui-tabbar">
        <a href="javascript:;" class="weui-tabbar__item" :class="index == 0 ? 'weui-bar__item_on' : ''" @click="changeIndex(0)">
        	<i class="iconfont big">&#xe8b9;</i>
            <p class="weui-tabbar__label">主页</p>
        </a>
        <a href="javascript:;" class="weui-tabbar__item" :class="index == 1 ? 'weui-bar__item_on' : ''" @click="changeIndex(1)">
        	<i class="iconfont big">&#xe630;</i>
            <p class="weui-tabbar__label">阅读</p>
        </a>
        <a href="javascript:;" class="weui-tabbar__item" :class="index == 2 ? 'weui-bar__item_on' : ''" @click="changeIndex(2)">
        	<i class="iconfont big">&#xe8cc;</i>
            <p class="weui-tabbar__label">写作</p>
        </a>
        <a href="javascript:;" class="weui-tabbar__item" :class="index == 3 ? 'weui-bar__item_on' : ''" @click="changeIndex(3)">
        	<i class="iconfont big">&#xe8c8;</i>
            <p class="weui-tabbar__label">个人</p>
        </a>
    </div>
</template>
<script>
export default {
	name: 'bottomNav',
	data: function(){
		return {
			index: 0
		}
	},
	methods: {
		changeIndex(nummber){
			this.index = nummber;
			this.$emit('indexChange',nummber);
		}
	}
}
</script>