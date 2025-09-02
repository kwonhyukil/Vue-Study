<template>
    <button @click="test">로그아웃</button>
    <!-- v-if는 존재 자체를 없앰 -->
    <div>
        <p v-if="isLogin">로그인이 되었습니다.</p>
        <p v-else>로그인이 필요합니다.</p>
    </div>
    <!-- v-show는 존재는 두고 보이는지만 바꿈 -->
    <div>
        <p v-show="isVisible">항상 DOM에 존재하지만 display:none 처리</p>
    </div>
</template>

<script>
export default {
    data() {
        return {
            isLogin: true
        }
    },
    methods: {
        test() {
            this.isLogin = false
        }
    }
}
</script>