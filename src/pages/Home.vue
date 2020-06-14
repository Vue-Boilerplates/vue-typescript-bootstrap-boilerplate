<template>
  <div class="text-center p-0 m-0 container-fluid">
    <Navbar />
    <div class="jumbotron m-0 p-0 p-3 jumbotron-fluid">
      <div class="container">
        <h2 class="display-4">Vue Boilerplates</h2>
        <p class="lead">vue-typescript-bootstrap-boilerplate</p>
        <div class="row mb-4 no-gutters justify-content-center">
          <img width="130px" height="auto" src="/img/vue-boilerplates.svg" />
        </div>
        <p class="m-0 p-0">
          Vue + Typescript + Bootstrap + Lazy loading and code splitting
        </p>
      </div>
    </div>
    <div class="container">
      <div class="row">
        <div class="col">
          <div
            class="jumbotron text-left m-0 text-dark bg-white border-white border"
          >
            <h2 class="display-5">Why Vue Boilerplates?</h2>
            <p>
              While mobile-first approach becomes a standard and uncertain
              network conditions are something we should always take into
              consideration, it’s harder and harder to keep your application
              loading fast. Vue Boilerplates was built with vue.js performance
              optimization techniques that make them loading instantly and
              perform smooth 🚀.
            </p>
          </div>
        </div>
        <div class="col">
          <div
            class="jumbotron text-left m-0 text-dark bg-white border-white border"
          >
            <h2 class="display-5">Lets grow together!</h2>
            <p class="lead">Please consider becoming a donor 🙏.</p>
            <p>
              Make a custom one time or recurring contribution to support my
              open source projects
            </p>
            <a
              href="https://opencollective.com/vue-boilerplates"
              rel="noopener"
              target="_blank"
              class="btn btn-success"
            >
              Donate
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Vue, Component } from "@/utils/vue-imports";
import Navbar from "@/components/Navbar.vue";

@Component({
  name: "Home",
  components: {
    Navbar,
  },
})
export default class Home extends Vue {
  images = [
    ["/img/pwa.png", "/img/pwa.png", "/img/pwa.png"],
    ["/img/pwa.png", "/img/pwa.png"],
  ];
}
</script>
