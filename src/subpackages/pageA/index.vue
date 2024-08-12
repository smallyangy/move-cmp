<template>
    <view>
        分包A
        <CMPB></CMPB>
        <CMPC></CMPC>
        <CMPD></CMPD>
    </view>
</template>

<script>
    import CMPB from '@/components/CMPB.vue';
    import CMPC from '../components/CMPC.vue';
    import CMPD from './components/CMPD.vue';

    export default {
        components: {
            CMPB,
            CMPC,
            CMPD,
        }
    };
</script>

<style lang="scss">

</style>
