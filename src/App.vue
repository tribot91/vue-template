<template>
    <b-container id="app">
        <b-row class="app-container w-100 p-5">
            <b-col cols="2"> <router-view /></b-col>
            <b-col cols="8">
                <b-row>
                    <b-col cols="8"> <router-view name="Home"/></b-col>
                    <b-col cols="4"> <router-view name="Sidebar"/></b-col>
                </b-row>
            </b-col>
        </b-row>
    </b-container>
</template>

<style lang="scss">
#app {
    background: rgb(230, 230, 230);
}
html,
body,
#app {
    margin: 0;
    padding: 0;
    min-height: 100vh;
    min-width: 100%;
}
.app-container {
    display: flex;
    justify-content: center;
}
</style>
