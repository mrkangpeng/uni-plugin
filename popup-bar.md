```javascript
import popupBar from '@/components/popup-bar/popup-bar.vue';
export default {
    components:{
        popupBar
    },
}
```

```javascript
<template>
	<view class="content">
		<popupBar size="middle" position="right"  bgColor="#10baaa">
			<view slot="main" class="refrash_wrap" @click="handleRefrash">
				<image class="icon" src="../../static/refrash.png"></image>
				<view class="text">重置</view>
			</view>
		</popupBar>
	</view>
</template>
```

