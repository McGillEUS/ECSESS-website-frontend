<template>
    <div>
        <div id="subtitle" class="subtitle">
            <h2>Who we are</h2>
        </div>
        <div id="section-text" class="section-text">
            <div id="textbox" class="textbox">
                <p>The 
                    <i>
                        Electrical, Computer and Software Engineering Students' Society
                    </i>
                    is the student council for the largest Engineering department at McGill, serving and helping over 900 students across campus (or at home this Fall).
                    <br>
                    <br>
                    By hosting numerous events throughout the year and giving diverse resources and networking opportunities to students, 
                    <b>
                        we are committed to building a lively community and growing young engineers' future careers.
                    </b>
                </p>
                <button id="learn-more" class="learn-more" @click="goToCouncil()">Learn More</button>
            </div>
            <div id="textimage" class="textbox">
                <img id="council20192020" class="image" src="../../assets/council2019-2020.jpg" />
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "AboutUs",
    components: {},
    methods: {
        goToCouncil: function () {
            window.scrollTo(0,0);
            this.$router.push({path: '/council'});
        }
    }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');
</style>