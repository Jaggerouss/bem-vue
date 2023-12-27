<template>
    <div class="ja-content">
        <div class="ja-content__items" v-for="item in 200">
            {{ item }}
        </div>
    </div>
</template>

<script setup>

</script>
<style scoped lang="scss">
@include b(content){
    flex:1;
    padding: 20px;
    overflow: auto;
    @include e(items){
        padding: 10px;
        margin: 10px;
        border: 1px solid black;
        border-radius: 4px;
    }
}
</style>