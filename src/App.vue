<template>

<!--  <nav class="navigation" id="mainNav">-->
<!--    <a class="navigation__link" href="#1">Section 1</a>-->
<!--    <a class="navigation__link" href="#2">Section 2</a>-->
<!--  </nav>-->

  <nav class="navigation" id="mainNav">
    <div class="item" v-for="(tree, index ) in trees"
         :key="index">
<!--         @click="selectItem(index)"-->
<!--         :class="{ active: index === selectedItem }"-->

      <div class="item-title border-bottom">
        {{ tree.title }}
      </div>
      <div v-if="tree.children" class="item-children">
        <RecursiveComp :trees="tree.children"></RecursiveComp>
      </div>
    </div>
  </nav>

  <div class="page-section hero" id="s1">
    <h1>Section 1</h1>
  </div>
  <div class="page-section hero" id="s1_c1">
    <h1>Section 1_1</h1>
  </div>
  <div class="page-section hero" id="s1_c1_c1">
    <h1>Section 1_1_1</h1>
  </div>
  <div class="page-section hero" id="s1_c1_c2">
    <h1>Section 1_1_2</h1>
  </div>
  <div class="page-section hero" id="s1_c1_c3">
    <h1>Section 1_1_3</h1>
  </div>
  <div class="page-section hero" id="s1_c2">
    <h1>Section 1_2</h1>
  </div>
  <div class="page-section hero" id="s1_c2_c1">
    <h1>Section 1_2_1</h1>
  </div>
  <div class="page-section hero" id="s1_c2_c2">
    <h1>Section 1_2_2</h1>
  </div>
  <div class="page-section" id="s2">
    <h1>Section 2</h1>
  </div>
  <div class="page-section" id="s3">
    <h1>Section 3</h1>
  </div>
  <link href='https://fonts.googleapis.com/css?family=Lato:100,400,700' rel='stylesheet' type='text/css'>
</template>

<script setup>
import { ref } from 'vue'
// const selectedItem = ref(null)
// let isActive = false
    const trees = ref([
        { title: 'Web Development',
        key: 's1',
        children: [
          {
            title: 'JavaScript',
            key: 's1_c1',
            children: [
              { title: 'Vue.js', key: 's1_c1_c1' },
              { title: 'React.js', key: 's1_c1_c2' },
              { title: 'Angular.js', key: 's1_c1_c3' }
            ]
          },
          {
            title: 'CSS',
            key: 's1_c2',
            children: [
              { title: 'Foundation', key: 's1_c2_c1' },
              { title: 'Bootstrap', key: 's1_c2_c2' }
            ]
          }
        ]},
        {title: 'Frameworks',
          key: 's2',
          children: [
            {
              title: 'JavaScript',
              key: 's2_c1',
              children: [
                { title: 'Vue.js', key: 's2_c1_c1' },
                { title: 'React.js', key: 's2_c1_c2' },
                { title: 'Angular.js', key: 's2_c1_c3' }
              ]
            },
            {
              title: 'CSS',
              key: 's2_c2',
              children: [
                { title: 'Foundation', key: 's2_c2_c1' },
                { title: 'Bootstrap', key: 's2_c2_c2' }
              ]
            }
          ]},
        {title: 'Programming Languages',
          key: 's3',
          children: [
            {
              title: 'JavaScript',
              key: 's3_c1',
              children: [
                { title: 'Vue.js', key: 's3_c1_c1' },
                { title: 'React.js', key: 's3_c1_c2' },
                { title: 'Angular.js', key: 's3_c1_c3' }
              ]
            },
            {
              title: 'CSS',
              key: 's3_c2',
              children: [
                { title: 'Foundation', key: 's3_c2_c1' },
                { title: 'Bootstrap', key: 's3_c2_c2' }
              ]
            }
          ]}
      ])
// const selectItem = (id) => {
//   selectedItem.value = id
//   trees.forEach((tree, index) => {
//     return (isActive = tree === trees[index])
//   })
//   return selectedItem
// }

</script>

<style lang="scss">

.item-title {
  line-height: .8rem;
  font-size: 1.32rem;
  padding: .5rem .2rem;
  background-color: #d9c7f1;
  margin-bottom: .2rem;
}
.item-children {
padding: .2rem;
  margin-bottom: .2rem;
}

* {
  font-family: 'Lato', sans-serif;
  font-weight: 500;
  transition: all .1s ease;
}

html, body {
  height: 100%;
}

h1 { font-size: 64px;

}

.page-section {
  height: 380px;
  width: 50%;
  margin-left: 35%;
  margin-top: 5%;
  padding: 3em;
  background: #541599;
  color: white;
  box-shadow: 0 3px 10px 0 rgba(0,0,0,0.5);
}

.navigation {
  position: fixed;
  width: 30%;
  margin-left: 2%;
  background-color: #ffffff;
  color: #000;

&__link {
   display: block;
   color: #ffffff;
   text-decoration: none;
   padding: 1em;
   font-weight: 400;

&:hover {
   background-color: #aaa;
 }

&.active {
   color: red;
   background-color: rgba(0,0,0,0.1);
 }
}
}
</style>
