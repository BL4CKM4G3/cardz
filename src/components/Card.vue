<template>
  <article>
    <div class="card-title">{{ content.title }}</div>
    <div class="card-subtitle">{{ content.subtitle }}</div>
    <div class="card-description">{{ content.description }}</div>
  </article>
</template>

<script>
export default {
  name: 'Card',
  props: ['content'],
}
</script>

<style lang="scss" scoped>
article {
  width: 25vw;
  height: 25vh;
  display: flex;
  flex-direction: column;
  margin: 10px 15px 10px 15px;
  border: 1px solid var(--secondary);
  padding: 10px 5px 10px 5px;
  transition: all .5s ease-in;
  &:hover {
    transition: background-color .5s ease-out;
    background-color: var(--background-hover);
  }
  .card-title {
    color: var(--primary);
    font-family: 'Lekton', sans-serif;
    font-weight: 700;
    margin: 0 0 10px 0;
    text-align: center;
    &:hover {
      border-bottom: 1px solid var(--caption);
      transition: all 1.9s ease-out;
    }
  }

  .card-subtitle {
    color: var(--caption);
    font-family: 'Lekton', sans-serif;
    text-align: center;
  }

  .card-description {
    color: var(--secondary);
    font-family: 'Lekton', sans-serif;
    margin: 10px 0 0 0;
    padding: 0 10px 0 10px;
    text-align: justify;
  }
}
</style>