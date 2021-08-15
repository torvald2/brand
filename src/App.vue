<template lang="pug">
  #app
    header
      b-navbar(toggleable="lg" type="dark" variant="light")
          b-navbar-brand(href="#")
             b-img(v-bind="mainProps" rounded="circle" alt="Сток та секонд хенд Каменское" src="static/img/brand/back2.png")
             span Сток та секонд хенд у Кам`янстькому 
          b-navbar-toggle(target="nav-collapse")
          b-collapse(id="nav-collapse" is-nav)
              b-navbar-nav
                  b-nav-item(href="#") Чому ми 
                  b-nav-item(href="shop") Замовити онлайн
    main
      router-view.mr-6.ml-6
    b-card(no-body class="text-center").mt-5
        .bg-secondary.text-light.text-center Copyright ФОП Скрипник І.С 2021
  </b-card>
</template>

<script>
export default {
  name: 'app'
}
</script>
<style scoped>
 .navbar{
    background-color: #ff7e18!important;
 }
</style>
