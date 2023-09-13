<template>
    <div class="cobblestone-path">
        <div class="path-side">
            <a class="stone"></a>
            <a class="stone"></a>
            <a class="stone"></a>
            <a class="stone"></a>
            <a class="stone"></a>
            <a class="stone"></a>
        </div>
        <div class="path-side">
            <a class="stone"></a>
            <a class="stone"></a>
            <a class="stone"></a>
            <a class="stone"></a>
            <a class="stone"></a>
        </div>
        <div class="path-side">
            <a class="stone"></a>
            <a class="stone"></a>
            <a class="stone"></a>
            <a class="stone"></a>
            <a class="stone"></a>
            <a class="stone"></a>
        </div>
    </div>
</template>

<style scoped>
.path-side {
    gap: .2rem;
    display: flex;
    flex-direction: column;
}
.stone {
    width: 100%;
    height:100%;
    background: #667085;
    border-radius: 50%;
    border: 1px solid black;
    box-shadow: 5px 5px 5px black;
}
.cobblestone-path {
    width:10%;
    height:100%;
    display:grid;
    grid-template-columns: auto auto auto;
}
</style>

<script>
export default {
    
}
</script>