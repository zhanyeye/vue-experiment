<template>
  <div id="app">
    <myheader />
    <div id="main">
      <sidebar />
      <myarticle />
    </div>
    <myfooter />
  </div>
</template>
<script>
export default {
  components: {
    myheader: () => import("@/views/Header.vue"),
    myarticle: () => import("@/views/Article.vue"),
    sidebar: () => import("@/views/Sidebar.vue"),
    myfooter: () => import("@/views/Footer.vue")
  }
};
</script>

<style>
#main {
  margin: 5px 0px;
  border: 1px solid red;
}
</style>
