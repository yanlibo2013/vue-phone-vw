<template>
    <div class="">
        <mt-header :title="$route.meta.header.title" v-if="$route.meta.header">
            <mt-button v-if="$route.meta.header.back" icon="back" slot="left" @click="$router.go(-1)">返回</mt-button>
        </mt-header>
        <mt-field label="数字" placeholder="请输入数字" type="number" v-model="number"></mt-field>
    </div>
</template>

<script>
    export default {
        name:'shop',
        data() {
            return {
                number:0
            }
        }
    }
</script>


<style lang="scss" type="text/scss" scoped>

</style>

  