<template lang="pug">
.container
  p collapsible
  collapsible
    collapsible-item
      p(slot="header") header1
      p body 1
    collapsible-item
      p(slot="header") header2
      p body 2
    collapsible-item
      p(slot="header") header3
      p body 3
  p accordion
  collapsible(accordion)
    collapsible-item
      p(slot="header") header1
      p Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.
    collapsible-item(is-opened)
      p(slot="header") header2
      p body 2
    collapsible-item
      p(slot="header") header3
      p body 3
  p
    a(href="https://github.com/paulpflug/vue-materialize/blob/master/dev/collapsible.vue") source
</template>

<script lang="coffee">
require("./materialize.config.scss")
module.exports =
  components:
    "collapsible" : require "../src/collapsible.coffee"
    "collapsible-item" : require "../src/collapsible-item.coffee"

</script>
