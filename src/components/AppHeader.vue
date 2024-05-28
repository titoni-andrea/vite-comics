<script>

export default {
    data() {
        return {
            numbers: [
            1,2,3,4,5,6,7,8,9,10
            ]
        }
    },
}

</script>

<template>
    <header>
        <div class="cont-flex">
            <img class="logo" src="/public/dc-logo.png" alt="">

            <div class="menu">
                <a v-for="elemento in numbers" href="#">bottone {{ elemento }}</a>
            </div>

        </div>
    </header>
</template>

<style scoped>
header {
    padding: 1rem 0px;
}

.cont-flex {
    width: 1200px;
    margin: auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    height: 100%;
}

.menu {
    display: flex;
    gap: 15px;
}

.menu a {
    color: #222;
    text-decoration: none;
}

.menu a:hover {
    color: #0B7CEC;
}

</style>