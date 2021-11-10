<template>
    <view class="index">
        <view class="btn">
            <nut-button type="primary" @click="pop()">返回</nut-button>
        </view>
    </view>
</template>

<script>
    import Taro from "@tarojs/taro";

    export default {
        name: "Index",
        components: {},
        setup() {
            const pop = () => {
                Taro.navigateBack();
            };
            return {
                pop
            };
        }
    };
</script>

<style lang="scss">
</style>
