<template>
    <div class="page">
        <!-- 主动打招呼弹窗-有依赖于BasePhoneLogin，千万别删除BasePhoneLogin -->
        <BasePhoneLogin ref="phoneLogin"></BasePhoneLogin>
        <BasePopSayHello ref="BasePopSayHello"></BasePopSayHello>
    </div>
</template>
<script>
export default {
    data() {
        return {}
    },
    computed: {},
    components: {},
    methods: {},
    onLoad() {},
    onReady() {},
    onShow() {},
    onHide() {},
    async onReady(){
        // 检查是否打开主动打招呼弹窗-
        await this.$refs?.BasePopSayHello.open()
    },
    onUnload() {},
    onPullDownRefresh() {},
    onReachBottom() {},
    onPageScroll() {}
}
</script>
<style lang="scss" scoped>
</style>
