<template>
    <!-- 선언적 렌더링, class bind rendering, Style bind rendering -->
    <BindingPractice />

    <!-- 조건부 렌더링 -->
    <div>
        <DeclarativeRendering />
    </div>
    <!-- v-if, v-show 활용 -->
    <div>
        <ConditionalRendering />
    </div>
    <!-- v-for 리스트 렌더링 -->
    <div>
        <ListRendering />
    </div>
    <div>
        <ListRandering2 />
    </div>
</template>

<script>
import BindingPractice from './components/binding-practice.vue';
import ConditionalRendering from './components/Conditional-Rendering.vue';
import DeclarativeRendering from './components/Declarative-Rendering.vue';
import ListRandering2 from './components/List-Randering2.vue';
import ListRendering from './components/List-Rendering.vue';


export default {
    components: {
        DeclarativeRendering,
        ConditionalRendering,
        ListRendering,
        BindingPractice,
        ListRandering2,
    },
}
</script>

