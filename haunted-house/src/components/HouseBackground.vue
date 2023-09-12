<template>
    <div class="sky-main-color">
        <a class="moon"></a>
        <div class="horizon-line">
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
        </div>
    </div>
</template>

<style scoped>
.moon {
    width: 2rem;
    height: 2rem;
    border-radius: 50%;
    background: #667085;
    position:absolute;
    left:2rem;
    top:2rem;
    box-shadow: 5px 5px 5px black;
}
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
.horizon-line {
    background:#0b1f03;
    width: 100%;
    height: 35%;
    position:relative;
    top:40rem;
    border-radius:5%;
    display:flex;
    justify-content: center;;
}
.sky-main-color {
    background: linear-gradient(0deg, rgba(1,2,20,1) 0%, rgba(13,41,128,1) 100%);
    height: 60rem;
    width: 100%;
    overflow: hidden;
    display: flex;
}
</style>