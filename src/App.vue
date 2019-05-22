<template>
    <div class="container mt-5" id="app">
        <div class="jumbotron">
            <h1 class="display-4">Erick Dos Santos</h1>
            <p
                class="lead"
            >Practical Exercises Resolution</p>
        </div>
        <div class="row">
            <div class="col-3">
                <nav id="list-exercise" class="list-group">
                    <a class="list-group-item list-group-item-action" href="#exercise-1">Exercise 1</a>
                </nav>
            </div>
            <div class="col-9">
                <div
                    data-spy="scroll"
                    data-target="#list-exercise"
                    data-offset="0"
                    class="scrollspy-exercises"
                >
                    <exercise1-vue/>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import Exercise1Vue from './components/exercises/Exercise1.vue';

export default {
    name: 'app',
    components: {
        Exercise1Vue,
    }
};
</script>

<style>
body {
    position: relative;
    height: 100%;
}
.scrollspy-exercises {
    height: 50vh;
    overflow: auto;
    position: relative;
}
</style>
