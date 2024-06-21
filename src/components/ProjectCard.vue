<template>
    <ul>
        <li v-for="project in projects" :key="project.id">
            <h2>{{ project.project_name }}</h2>
            <p>{{ project.slug }}</p>
        </li>
    </ul>
</template>

<script>
export default {
    setup() {


        return {}
    }
}
</script>

<style lang="scss" scoped></style>