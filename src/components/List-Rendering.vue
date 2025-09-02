<template>
    <div>
        <ul>
            <li v-for="item in items" :key="item.id">
                {{ item.name }}
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    data() {
        return {
            items: [
                { id: 1, name: "일번" },
                { id: 2, name: "이번" },
                { id: 3, name: "삼번" },
                { id: 4, name: "사번" },
                { id: 5, name: "오번" },
            ]
        }
    }
}
</script>