<template>
  <aside class="sidebar">
    <ul>
      <li>tasks</li>
      <li>profile</li>
      <li>feed</li>
      <li>about</li>
    </ul>
  </aside>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.sidebar {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  width: 10vw;
  height: 80vh;
  padding: 0 5px 0 0;
  border-right: 1px solid var(--caption);

  ul {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    height: inherit;
    li {
      color: var(--secondary);
      font-family: "Montserrat", sans-serif;
      margin: 10px auto 10px auto;
      padding: 0 10px 10px 10px;
      border-bottom: 1px solid var(--caption);
      transition: all 0.05s ease-out;
      &:hover {
        color: var(--secondary-hover);
        font-weight: var(--sidebar-item-font-weight-hover);
        transition: all 0.05s ease-in;
      }
    }
  }
}
</style>