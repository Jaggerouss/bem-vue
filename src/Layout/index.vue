<template>
    <div class="ja-wraps">
         <div>
            <Menu></Menu>
         </div>
         <div class="ja-wraps__right">
            <Header></Header>
            <Content></Content>
         </div>
    </div>
</template>
 
<script setup>
import { ref, reactive } from "vue"
import Menu from './Menu/index.vue'
import Content from './Content/index.vue'
import Header from './Header/index.vue'
</script>
 
<style lang="scss" scoped>
@include b('wraps'){
    @include bfc;
    @include flex;
    @include e(right){
        flex:1;
        display: flex;
        flex-direction: column;
    }
}
</style>