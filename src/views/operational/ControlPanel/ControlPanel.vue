<script setup>
import CardInfoServiceByProducts from './components/CardInfoServiceByProducts.vue';
import CardInfoServiceByStatus from './components/CardInfoServiceByStatus.vue';
import CardInfoServiceByStatusPayment from './components/CardInfoServiceByStatusPayment.vue';
import CardInfoServicePerformance from './components/CardInfoServicePerformance.vue';
</script>

<template>
    <div class="grid">

        <div class="col-12 xl:col-12 mobile-hidden">
            <CardInfoServicePerformance />
        </div>

        <div class="col-12 xl:col-4">
            <CardInfoServiceByStatus />
        </div>

        <div class="col-12 xl:col-4">
            <CardInfoServiceByStatusPayment />
        </div>

        <div class="col-12 xl:col-4">
            <CardInfoServiceByProducts />
        </div>
        
    </div>
</template>

<style scoped>
.mobile-hidden {
    display: block;
}

@media screen and (max-width: 900px) {
    .mobile-hidden {
        display: none;
    }
}
</style>
