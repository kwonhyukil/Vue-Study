<template>
    <div>
        <div v-if="isVisible" class="red"></div>
        <div v-if="isVisible === true" class="blue"></div>

        <div v-else class="black"></div>
        <button @click="change">변경</button>

        <div v-if="count > 1" class="green"></div>
        <div v-else class="yellow"></div>
        <div>{{ count }}</div>

        <button @click="count++">증가</button>
        <button @click="count--">감소</button>

        <!-- 자주 변경될 때 -->
        <div v-show="isVisible" class="red"></div>
        <div v-show="!isVisible" class="blue"></div>

        <!-- 자주 변경되지 않을 때 -->
        <div v-if="isVisible" class="black"></div>
    </div>
</template>

<script>

export default {
    data() {
        return {
            isVisible: false,
            count: 0
        }
    },
    methods: {
        change() {
            this.isVisible = !this.isVisible
        }
    }
}
</script>

<style scoped>
.red {
    width: 100px;
    height: 100px;

    background-color: red;
}
.blue {
    width: 100px;
    height: 100px;

    background-color: blue;
}
.black {
    width: 100px;
    height: 100px;

    background-color: black;
}
.green {
    width: 100px;
    height: 100px;

    background-color: green;
}
.yellow {
    width: 100px;
    height: 100px;

    background-color: yellow;
}


</style>