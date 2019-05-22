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
                    <a class="list-group-item list-group-item-action" href="#exercise-2">Exercise 2</a>
                    <a class="list-group-item list-group-item-action" href="#exercise-3">Exercise 3</a>
                    <a class="list-group-item list-group-item-action" href="#exercise-4">Exercise 4</a>
                    <a class="list-group-item list-group-item-action" href="#exercise-5">Exercise 5</a>
                    <a class="list-group-item list-group-item-action" href="#exercise-6">Exercise 6</a>
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
                    <exercise2-vue/>
                    <exercise3-vue/>
                    <exercise4-vue/>
                    <exercise5-vue/>
                    <exercise6-vue/>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import Exercise1Vue from './components/exercises/Exercise1.vue';
import Exercise2Vue from './components/exercises/Exercise2.vue';
import Exercise3Vue from './components/exercises/Exercise3.vue';
import Exercise4Vue from './components/exercises/Exercise4.vue';
import Exercise5Vue from './components/exercises/Exercise5.vue';
import Exercise6Vue from './components/exercises/Exercise6.vue';

export default {
    name: 'app',
    components: {
        Exercise1Vue,
        Exercise2Vue,
        Exercise3Vue,
        Exercise4Vue,
        Exercise5Vue,
        Exercise6Vue
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
