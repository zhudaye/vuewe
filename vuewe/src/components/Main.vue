<template>
    <div class="weui-tab">
	    <div class="weui-tab__panel">
	    </div>
	    <my-nav @indexChange="indexed"></my-nav>   
	</div>
</template>
<script>
import bottomNav from "@/components/BottomNav"
export default {
	name: 'main',
	components: {
	    'my-nav': bottomNav
	},
	methods: {
		indexed: function(nummber) {
			console.log(nummber);
		}
	}
}
</script>