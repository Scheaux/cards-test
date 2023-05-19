<script setup>
import Cards from './components/Cards.vue';
import icon1 from './assets/icon1.png';
import icon2 from './assets/icon2.png';
import icon3 from './assets/icon3.png';

const cards = [
    {
        title: 'Поставка электронных компонентов',
        body: 'Оптовые и мелкооптовые партии от ведущих производителей Китая и различных стран Азии.',
        icon: icon1,
    },
    {
        title: 'Контрактное производство',
        body: 'Сборка электронных модулей и монтаж печатных плат, под ваши запросы. Собственная производственная линия.',
        icon: icon2,
    },
    {
        title: 'Производство трансформаторов и дросселей',
        body: 'Многолетний успешный опыт разработки и производства на заказ. Надёжность и высокое качество продукции.',
        icon: icon3,
    },
];
</script>

<template>
    <Cards v-bind:cards="cards" />
</template>
