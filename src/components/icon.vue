<template>
    <div class="icon text-start">
        <img class="w-100 mb-2" :src="icon.thumb" alt="">
        <span class="text-uppercase">{{icon.series}}</span>
    </div>
</template>

<script>
export default {
    name:'mainIcon',
    props:{icon:Object}
}
</script>

<style lang="scss" scoped>
.icon{
    width: calc(100% / 6 - 1.3rem);
    // height: 12rem;
    flex-direction: column;
    img{
        height: 10rem;
        object-fit: cover;
        object-position: top;
    }
    span{
        font-size: small;
    }
}
</style>