<template>
    <a class="cloud-base">
        <a class="cloud-pouf pouf-1"></a>
        <a class="cloud-pouf pouf-2"></a>
        <a class="cloud-pouf pouf-3"></a>
    </a>
</template>

<style scoped>
.pouf-2 {
    left: 5rem;
    bottom: 1rem;
    width: 5rem;
    height: 5rem;
}
.pouf-1 {
    left: 4.5rem;
    bottom: 1.5rem;
    width: 6rem;
    height: 6rem;
}
.cloud-pouf {
    border-radius: 50%;
    background: white;
    position: relative;
}
.cloud-base {
    border-radius: 50%;
    background: white !important;
    display: grid;
    width: 15rem;
    height: 3rem;
}
</style>