<template>
    <div v-if="isACloud">
        <a class="cloud-base" :style="computedStyle">
            <a id="1" class="cloud-pouf pouf-1" @click="handlePoufClick(1)"></a>
            <a id="2" class="cloud-pouf pouf-2" @click="handlePoufClick(2)"></a>
            <a id="3" class="cloud-pouf pouf-3" @click="handlePoufClick(3)"></a>
        </a>
    </div>
    <div v-else>
        
    </div>
</template>

<style scoped>
.pouf-3 {
    left: 9rem;
    bottom: 12rem;
    width: 5rem;
    height: 5rem;
}
.pouf-2 {
    left: 1.5rem;
    bottom: 7rem;
    width: 5rem;
    height: 5rem;
}
.pouf-1 {
    left: 4.5rem;
    bottom: 1.5rem;
    width: 6rem;
    height: 6rem;
}
.pouf-3:hover {
    display: none;
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

<script setup>
import { reactive, computed, ref } from 'vue'

const props = defineProps({
    top: {
        type: String,
        required: true
    },
    right: {
        type: String,
        required: true
    }
})

const remainingPoufs = ref(3)
const isACloud = ref(true)

const computedStyle = computed(() => {
    return 'top: ' + props.top + ';right: ' + props.right
})

function handlePoufClick(id) {
    if (remainingPoufs > 0) {
        remainingPoufs = remainingPoufs.value - 1
        document.getElementById(id).style = 'display: none;'
    } else {
        isACloud.value = false
    }
}
</script>