<script>

export default {
    data() {
        return {
            numbers: [
                1, 2, 3, 4, 5
            ]
        }
    },
}

</script>

<template>
    <footer>


        <div class="cta">
            <div class="cont-flex">

                <div v-for="elemento in numbers" class="second-menu">
                    <img src="/public/buy-comics-digital-comics.png" alt="">
                    <p>DIGITAL COMICS</p>
                </div>

            </div>
        </div>



        <div class="info">
            <div class="cont-flex">

                <div class="note-legali">
                    <div class="colonna">
                        <h3 class="titoletto">DC COMICS</h3>
                        <p v-for="elemento in numbers">Characters</p>
                        <h3 class="titoletto">SHOP</h3>
                        <p v-for="elemento in numbers">Shop DC</p>
                    </div>
                    <div class="colonna">
                        <h3 class="titoletto">DC</h3>
                        <p v-for="elemento in numbers">Term of Use</p>
                    </div>
                    <div class="colonna">
                        <h3 class="titoletto">SITES</h3>
                        <p v-for="elemento in numbers">MAD Magazine</p>
                    </div>
                </div>

                <div class="logo-footer">

                </div>
            </div>
        </div>

        <div class="reg-social">
            <div class="cont-flex">
            <button class="reg">SIGN-UP NOW!</button>
            <div class="social">
                <h2 class="seguici">FOLLOW US</h2>
                <img v-for="elemento in numbers" src="/public/footer-facebook.png" alt="">
            </div>
        </div>
        </div>




    </footer>
</template>

<style scoped>
footer {
    background-image: url("/public/footer-bg.jpg");

}

.cta {
    background-color: #0B7CEC;
    color: white;
    padding: 2rem 0px;
}

.second-menu {
    display: flex;
    align-items: center;
    gap: 1rem;
}

.second-menu img {
    width: 25%;
}


.cont-flex {
    width: 1200px;
    margin: auto;
    padding: 2rem 0px;
    display: flex;
    gap: 30px
}

.note-legali {
    color: grey;
    display: flex;
    gap: 50px;
}

.note-legali p {
    margin-bottom: 5px;
}

.titoletto {
    margin-bottom: 15px;
    margin-top: 15px;
    color: white;
}

.reg-social {
    background-color: #403f3f;
}

.reg {
    background-color: #403f3f;
    border: solid 2px #0B7CEC;
    padding: 10px 18px;
    font-size: 20px;
    color: white;
}

.social {
    display: flex;
    width: 40%;
    align-items: center;
    gap: 15px;
    color: #0B7CEC;
}


</style>