<template>
    <header>
        <div class="header-top">
            <h1>ISA COSTURAS</h1>
        </div>
        <section class="hero">
            <div class="overlay">
                <img :src="imageSrc" alt="Imagem do cabeçalho">
                <div class="content">
                    <h2 class="mb-3">Transformando tecidos em sonhos<br>com dedicação e arte.</h2>
                    <p class="mb-4">Deseja confeccionar sua roupa ou concertar ela?</p>
                    <WhatsAppButton text="Converse comigo" number="5543996726268"/>
                </div>
            </div>
        </section>
    </header>
</template>

<style scoped>
    .header-top {
        background-color: #e6ab94;
        padding: 20px;
        text-align: center;
        border-radius: 0px 0px 10px 10px;
    }

    .header-top h1 {
        margin: 0;
        color: #ffffff;
        font-size: 1.5em;
    }

    .hero .overlay img {
        width: 100%;
        max-height: 300px;
        object-fit: cover;
        position: relative;
        bottom: 1rem;
        z-index: -1;
        filter: brightness(0.5);
    }

    .overlay {
        position: relative;
    }

    .overlay .content {
        position: absolute;
        top: 40%;
        left: 50%;
        color: white;
        font-size: large;
        text-align: center;
        transform: translate(-50%, -50%);
    }
</style>

<script>
    import WhatsAppButton from '@/components/itens/links/WhatsAppButton.vue'

    export default {
        name: 'PageHeader',
        components: {
            WhatsAppButton
        },
        data() {
            return {
                imageSrc: require('@/assets/images/headerImage.jpg')
            };
        }
    }
</script>
