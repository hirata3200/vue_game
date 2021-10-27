<template>
    <div class="marubatu" v-on:click="doAction">
        {{marubatu}}
    </div>
</template>

<script>
export default {
    name: "Marubatu",
    data() {
        return {
            marubatu:"",
        };
    },
    props: {
        count: Number,
    },
    methods: {
        doAction(){
            this.marubatu = "〇"
        },
    },
};
</script>

<style>
.marubatu{
    width: 150px;
    height: 150px;
    border: 1px solid black;
    text-align: center;
    font-size: 80px;
    color: red;
}
</style>