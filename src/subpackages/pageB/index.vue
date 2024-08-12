<template>
    <view>
        分包B
        <CMPB></CMPB>
        <CMPC></CMPC>
    </view>
</template>

<script>
    import CMPB from '@/components/CMPB.vue';
    import CMPC from '../components/CMPC.vue';

    export default {
        components: {
            CMPB,
            CMPC,
        }
    };
</script>

<style lang="scss">

</style>
