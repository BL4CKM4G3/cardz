<template>
  <div class="home">
    <sidebar></sidebar>
    <card v-for="card in cards" :key="card.id" :content="card"></card>
  </div>
</template>

<script>
import Card from '../components/Card.vue'
import Sidebar from '../components/Sidebar.vue'
// @ is an alias to /src

export default {
  name: 'Home',
  components: {
    Sidebar,
    Card
  },
  data: () => ({
    cards: [
      {
        id: 1,
        title: 'Create a design for Acme Corporation',
        level: 'medium',
        subtitle: 'need to focus',
        priority: 'high',
        description: 'Need to create a design for Acme Corporation, need to think as a child watching a cartoon.'
      },
      {
        id: 2,
        title: 'Create a design for Acme Corporation',
        level: 'medium',
        subtitle: 'need to focus',
        priority: 'high',
        description: 'Need to create a design for Acme Corporation, need to think as a child watching a cartoon.'
      },
      {
        id: 3,
        title: 'Create a design for Acme Corporation',
        level: 'medium',
        subtitle: 'need to focus',
        priority: 'high',
        description: 'Need to create a design for Acme Corporation, need to think as a child watching a cartoon.'
      },
      {
        id: 4,
        title: 'Create a design for Acme Corporation',
        level: 'medium',
        subtitle: 'need to focus',
        priority: 'high',
        description: 'Need to create a design for Acme Corporation, need to think as a child watching a cartoon.'
      },
    ]
  })
}
</script>

<style lang="scss" scoped>
  .home {
    display: flex;
    flex-direction: row;
    width: auto;
  }
</style>