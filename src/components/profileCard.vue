<template>
    <div class="box">
        <img :src="picUrl" :alt="altText">
        <p>{{ name }}</p>
    </div>
</template>

<script>
    export default {
        name: "profileCard",
        props: {
            name: {
                type: String,
                required: true,
            },
            picUrl: {
                type: String,
                required: true,
            },
            altText: String,
        }
    }
</script>