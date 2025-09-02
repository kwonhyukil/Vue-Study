<template>
    <div>
        {{ count }}
    </div>
    <h1>Vue.js 라이프사이클 테스트</h1>

    <div>
        <DeclarativeRendering />
    </div>

    <div>
        <ConditionalRendering />
    </div>

    <div>
        <ListRendering />
    </div>
</template>

<script>
import ConditionalRendering from './components/Conditional-Rendering.vue';
import DeclarativeRendering from './components/Declarative-Rendering.vue';
import ListRendering from './components/List-Rendering.vue';

export default {
    components: {
        DeclarativeRendering,
        ConditionalRendering,
        ListRendering,
    },
    data() {
        return {
            count: 0,
        }
    },    
}
</script>

