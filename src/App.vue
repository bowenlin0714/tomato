<template lang="pug">
  #app
    b-navbar(toggleable='lg' type='dark' variant='danger')
     b-container
      b-navbar-brand(to='/') 番茄鐘
      b-navbar-toggle(target='nav-collapse')
      b-collapse#nav-collapse(is-nav)
        b-navbar-nav
          //- https://bootstrap-vue.org/docs/components/nav#comp-ref-b-nav-item
          b-nav-item(to='/list') 待辦
          b-nav-item(to='/settings') 設定
    //- 避免元件在換頁時被銷毀
    keep-alive
      router-view
</template>
