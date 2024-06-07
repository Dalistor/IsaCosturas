<style scoped>
    .button {
        text-decoration: none;
        background-color: rgb(114, 241, 114);
        color: white;
        transition: 0.5s;
        cursor: pointer;
        margin: 1rem;
        padding: 0.5rem;
        border-radius: 10px;
    }

    .button:hover {
        transform: scale(1.1);
        background-color: rgb(169, 248, 169);
    }
</style>

<template>
    <a :href="`https://api.whatsapp.com/send/?phone=${number}`" class="button" target="_blank">{{ text }}</a>
</template>

<script>
    export default {
        name: 'WhatsAppButton',
        props: {
            text: {
                type: String,
                required: true
            },
            number: {
                type: String,
                required: true
            }
        }
    }
</script>
