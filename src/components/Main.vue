<template>
  <div class="page">
  <div id="home" class="inner">
    <h1>Ken Erikson</h1>
    <p>
      For a guide and recipes on how to configure / customize this project,<br>
      check out the docs.
    </p>
  </div>
  <div id="about" class="inner orange">
    <div>
    <h1>Ken Erikson</h1>
    <p>
      For a guide and recipes on how to configure / customize this project,<br>
      check out the docs.
    </p>
    </div>
  </div>
  <div id="portfolio" class="inner">
    <div class="white-card margin-minus">
    <h1>Ken Erikson</h1>
    <p>
      For a guide and recipes on how to configure / customize this project,<br>
      check out the docs.
    </p>
    </div>
  </div>
  <div id="contact" class="inner">
    <h1>Ken Erikson</h1>
    <p>
      For a guide and recipes on how to configure / customize this project,<br>
      check out the docs.
    </p>
  </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component'

@Options({
  props: {
    msg: String
  }
})
export default class HelloWorld extends Vue {
  msg!: string
}
</script>
