<template>
  <div id="app">
    <Header/>
    <Container/>
  </div>
</template>

<script>
import Header from './components/Header'
import Container from './components/Container'

export default {
  name: 'App',
  components: {
    Header,
    Container
  }
}
</script>