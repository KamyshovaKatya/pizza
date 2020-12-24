<template>
    <div>
        <slot name="n1"></slot>
        <h2>Название пиццы: {{pizzaName}}</h2>
        <p>Размер: {{pizzaSize}}см</p>
        <p>Цена: {{pizzaPrice}}$</p>
        <slot></slot>
    </div>
</template>

<script>
export default {
    props: ['pizzaName','pizzaPrice', 'pizzaSize']   
}
</script>