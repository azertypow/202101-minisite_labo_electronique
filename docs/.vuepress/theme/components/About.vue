<template>
    <section class="v-about">
        <div class="v-about__left"></div>

        <div class="v-about__center">
            <h5>Head of Department</h5>
            <h6>Alexia Mathieu</h6>
            <br>
            <h5>graphic design</h5>
            <h6 class="cap">font</h6>
            <h6>Inter, Inter Display</h6>
            <h6 class="cap">graphic / interaction design</h6>
            <h6>Nicolas BALDRAN</h6>
        </div>

        <div class="v-about__right">
          <h5>Interaction Design, Game Design, Connected objects</h5>
          <h6>Creating tomorrow’s connected experiences</h6>
          <br>
          <h6>The MA in Media Design offers a two-year professional programme based on learning about interactive design for scientific and social innovation. Whether you are a graphic or industrial designer, a general engineer or computer engineer, you will address the technological and societal challenges generated by artificial intelligence and new interfaces.</h6>
        </div>
    </section>
</template>

<script lang="ts">
    import { Vue, Component, Prop } from "vue-property-decorator";

    @Component
    export default class About extends Vue {

    }
</script>

<style lang="scss" scoped>
    @import "../styles/params";
    @import "../styles/font-settings";
    @import "../styles/grid";

    .v-about {
        background-color: $site-color;
        color: $site-theme-color;
        @include column-container;
        padding-top: $font-small--line-height;
        padding-bottom: $font-small--line-height;
        align-items: baseline;
    }

    .v-about__left {
        @include grid-coll-number(2, 12);
        @include font--2;
        padding: 0 $grid-gutter-width / 2;
        margin: 0;

        > * {
            margin: 0;
        }
    }

    .v-about__center {
        @include font--2;
        @include grid-coll-number(4, 12);
        padding: 0 $grid-gutter-width / 2;
        margin: 0;

        > * {
            margin: 0;
        }
    }

    .v-about__right {
        @include font--2;
        @include grid-coll-number(6, 12);
        padding: 0 $grid-gutter-width / 2;
        margin: 0;

        > * {
            margin: 0;
        }
    }

    .cap {
        text-transform: uppercase;
    }
</style>
