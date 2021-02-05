<template>
  <div class="layout sticky-header" id="app"> 
    <!-- <header class="header">
      <strong>
        <g-link to="/"><img src="/img/logo_332701b7.png"></g-link>
      </strong>
      <nav class="nav">
        <g-link class="nav__link" to="/">Journal</g-link>
        <g-link class="nav__link" to="/about/">Say Hi!</g-link>
      </nav>
    </header> -->

    <header class="header sticky" data-v-7e33895e=""><div class="container" data-v-7e33895e=""><div class="left" data-v-7e33895e=""><a href="/" aria-current="page" class="home-link active--exact active" data-v-7e33895e=""><img src="/img/logo_332701b7.png" alt="Nichlas W. Andersen" class="logo" data-v-7e33895e=""></a></div><nav class="nav right" data-v-7e33895e=""><a href="/journal" class="nav__link" data-v-7e33895e="">Journal</a><a href="/contact" class="nav__link" data-v-7e33895e="">Say Hi!</a></nav></div></header>
    <slot/>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<style>
.left{ float: left;}
.right{ float: right;}
.container{ width: inherit; }
    
body {
  font-family: -apple-system,system-ui,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial,sans-serif;
  margin:0;
  padding:0;
  line-height: 1.5;
}

.layout {
  margin: 0 auto;
  padding: 0 6rem;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  height: 80px;
  position: fixed;
  top: 0;
}

.nav__link {
  margin-left: 60px;
  text-decoration-line: none;
  font-weight: 600;
  color:black
}
.nav__link:hover{
  text-decoration-line: underline;
}
</style>
