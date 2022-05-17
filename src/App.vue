<template>
<div id="app">
    <header>
        <h1>The Vue Accordion</h1>
    </header>
    <accordion>
        <accordion-item>
            <!-- This slot will handle the title/header of the accordion and is the part you click on -->
            <template slot="accordion-trigger">
                <h3>Item 1</h3>
            </template>
            <!-- This slot will handle all the content that is passed to the accordion -->
            <template slot="accordion-content">
                <div class="flex flex-col">
                    <div>
                        <span>Content 1</span>
                        <span>Content 2</span>
                    </div>
                    <div>
                        <span>Content 1</span>
                        <span>Content 2</span>
                    </div>
                </div>
            </template>
        </accordion-item>

        <accordion-item>
            <template slot="accordion-trigger">
                <h3>Item 2</h3>
            </template>
            <template slot="accordion-content">
                <span>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</span>
            </template>
        </accordion-item>

        <accordion-item>
            <template slot="accordion-trigger">
                <h3>Item 3</h3>
            </template>
            <template slot="accordion-content">
                <span>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</span>
            </template>
        </accordion-item>
    </accordion>
</div>
</template>

<script>
import Accordion from './components/Accordion.vue'
import AccordionItem from './components/AccordionItem.vue'

export default {
    name: 'App',
    components: {
        Accordion,
        AccordionItem
    }
}
</script>

<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}
</style>
