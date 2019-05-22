<template>
    <div id="exercise-1" class="mb-5 p-4 border">
        <div class="col-11 border-bottom my-2">
            <h4>Exercise 1</h4>
        </div>
        <div class="col-11 my-2 py-2">
            <p>{{ message }} - {{ name }} ({{ age }})</p>
        </div>
        <div class="col-11 my-2 py-2">
            <p>Age * 3</p>
            <code>{{ age }} * 3 = {{ age * 3 }}</code>
        </div>
        <div class="col-11 my-2 py-2">
            <h6>{{ outputRandom() }}</h6>
        </div>
        <div class="col-11 my-2 py-2">
            <label for="age"><b>Age</b></label>
            <input id="age" class="form-control" type="number" v-model.number="age" >
            <label for="name"><b>Name</b></label>
            <input id="name" class="form-control" type="text" v-model="name" >
        </div>
        <div class="col-11 my-2 py-2">
            <img class="img-fluid" :src="imageURL">
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            message: 'VueJS is pretty cool',
            name: 'Erick',
            age: 23,
            imageURL: 'https://www.osf-global.com/assets/img/content/logo-big.jpg'
        };
    },
    methods: {
        outputRandom() {
            return Math.random();
        }
    }
};
</script>
