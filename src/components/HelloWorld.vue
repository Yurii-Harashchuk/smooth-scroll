<!--<template>-->
<!--  &lt;!&ndash;  <div class="container">&ndash;&gt;-->
<!--  &lt;!&ndash;    <h4>Implement Tree with checkboxes and drag drop<br/><small>(Using Vue, Recursive Component, Vue Draggable)</small></h4>&ndash;&gt;-->
<!--  &lt;!&ndash;    <div id="app"&ndash;&gt;-->
<!--  &lt;!&ndash;         :nodes="tree.nodes"&ndash;&gt;-->
<!--  &lt;!&ndash;         :depth="0"&ndash;&gt;-->
<!--  &lt;!&ndash;         :label="tree.label"&ndash;&gt;-->
<!--  &lt;!&ndash;         :selected="tree.selected"&ndash;&gt;-->
<!--  &lt;!&ndash;    >&ndash;&gt;-->

<!--  &lt;!&ndash;    </div>&ndash;&gt;-->

<!--  &lt;!&ndash;  </div>&ndash;&gt;-->
<!--  <nav class="navigation" id="mainNav">-->
<!--    <a class="navigation__link" href="#1">Section 1</a>-->
<!--    <a class="navigation__link" href="#2">Section 2</a>-->
<!--    <a class="navigation__link" href="#3">Section 3</a>-->
<!--    <a class="navigation__link" href="#4">Section 4</a>-->
<!--    <a class="navigation__link" href="#5">Section 5</a>-->
<!--    <a class="navigation__link" href="#6">Section 6</a>-->
<!--    <a class="navigation__link" href="#7">Section 7</a>-->
<!--  </nav>-->

<!--  <div class="page-section hero" id="1">-->
<!--    <h1>Smooth scroll, fixed jump menu with active class</h1>-->
<!--  </div>-->
<!--  <div class="page-section" id="2">-->
<!--    <h1>Section Two</h1>-->
<!--  </div>-->
<!--  <div class="page-section" id="3">-->
<!--    <h1>Section Three</h1>-->
<!--  </div>-->
<!--  <div class="page-section" id="4">-->
<!--    <h1>Section Four</h1>-->
<!--  </div>-->
<!--  <div class="page-section" id="5">-->
<!--    <h1>Section Five</h1>-->
<!--  </div>-->
<!--  <div class="page-section" id="6">-->
<!--    <h1>Section Six</h1>-->
<!--  </div>-->
<!--  <div class="page-section" id="7">-->
<!--    <h1>Section Seven</h1>-->
<!--  </div>-->
<!--  <link href='https://fonts.googleapis.com/css?family=Lato:100,400,700' rel='stylesheet' type='text/css'>-->
<!--</template>-->

<!--<script>-->
<!--export default {-->
<!--  name: 'App',-->
<!--  components: {-->
<!--  },-->
<!--  setup () {-->
<!--    // const tree = {-->
<!--    //   label: 'root',-->
<!--    //   selected: false,-->
<!--    //   nodes: [-->
<!--    //     {-->
<!--    //       label: 'item1',-->
<!--    //       selected: false,-->
<!--    //       nodes: [-->
<!--    //         {-->
<!--    //           label: 'item1.1',-->
<!--    //           selected: false-->
<!--    //         },-->
<!--    //         {-->
<!--    //           label: 'item1.2',-->
<!--    //           selected: false,-->
<!--    //           nodes: [-->
<!--    //             {-->
<!--    //               label: 'item1.2.1',-->
<!--    //               selected: false-->
<!--    //             }-->
<!--    //           ]-->
<!--    //         }-->
<!--    //       ]-->
<!--    //     },-->
<!--    //     {-->
<!--    //       label: 'item2',-->
<!--    //       selected: false-->
<!--    //     }-->
<!--    //   ]-->
<!--    // }-->


<!--    return {-->
<!--      // tree-->
<!--    }-->
<!--  }-->
<!--}-->
<!--</script>-->

<!--<style lang="scss">-->
<!--/*body {*/-->
<!--/*  font-family: "Open Sans", sans-serif;*/-->
<!--/*  font-size: 18px;*/-->
<!--/*  font-weight: 300;*/-->
<!--/*  line-height: 1em;*/-->
<!--/*}*/-->

<!--* {-->
<!--  font-family: 'Lato', sans-serif;-->
<!--  font-weight: 300;-->
<!--  transition: all .1s ease;-->
<!--}-->

<!--html, body {-->
<!--  height: 100%;-->
<!--}-->

<!--h1 { font-size: 64px; }-->

<!--.page-section {-->
<!--  height: 480px;-->
<!--  width: 50%;-->
<!--  margin-left: 35%;-->
<!--  margin-top: 5%;-->
<!--  padding: 3em;-->
<!--  background: linear-gradient(45deg, #43cea2 10%, #185a9d 90%);-->
<!--  color: white;-->
<!--  box-shadow: 0 3px 10px 0 rgba(0,0,0,0.5);-->
<!--}-->

<!--.navigation {-->
<!--  position: fixed;-->
<!--  width: 30%;-->
<!--  margin-left: 2%;-->
<!--  background-color: #999;-->
<!--  color: #fff;-->

<!--  &__link {-->
<!--    display: block;-->
<!--    color: #ddd;-->
<!--    text-decoration: none;-->
<!--    padding: 1em;-->
<!--    font-weight: 400;-->

<!--    &:hover {-->
<!--      background-color: #aaa;-->
<!--    }-->

<!--    &.active {-->
<!--      color: white;-->
<!--      background-color: rgba(0,0,0,0.1);-->
<!--    }-->
<!--  }-->
<!--}-->



<!--</style>-->
