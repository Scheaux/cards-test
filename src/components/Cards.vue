<script lang="ts">
import Card from './Card.vue';

export default {
    data() {
        return {
            renderedCards: this.cards,
        };
    },
    props: ['cards'],
    components: {
        Card,
    },
    created() {
        document.addEventListener('keypress', (evt) => {
            if (evt.ctrlKey === true && evt.key === 'F') {
                this.renderedCards = this.renderedCards.reverse();
            }
        });
    },
};
</script>

<template>
    <div class="flex flex-col md:flex-row gap-8 justify-around">
        <Card
            v-for="card in renderedCards"
            v-bind:title="card.title"
            v-bind:body="card.body"
            v-bind:icon="card.icon"
        />
    </div>
</template>
