<template>
    <PageHeader></PageHeader>
    <div class="main">
        <AsideMenuVue></AsideMenuVue>
        <router-view></router-view>
    </div>
</template>

<script setup>
import PageHeader from '@/components/PageHeader.vue'
import AsideMenuVue from '@/components/AsideMenu.vue';
</script>

<style lang="scss" scoped>
.main{
    display: flex;
    justify-content:flex-start;
}
</style>