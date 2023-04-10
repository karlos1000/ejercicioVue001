<template>
    <div class="hello">
        <h1>Recorrer listado</h1>
        <ul>
            <li v-for="(item, index) in listado" v-bind:key="index">{{ item.nombre }} - {{ item.edad }}</li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'Lista',
    props: {
        // msg: String
    },
    setup() {
        let listado = [
            {
                nombre: "Carlos",
                edad: 35
            },
            {
                nombre: "Ramiro",
                edad: 18
            }
        ];

        return {
            listado
        }
    }

}
</script>

<style>
</style>
