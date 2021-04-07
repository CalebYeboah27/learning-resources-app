<template>
  <div>
    <li>
      <base-card>
        <header>
          <h3>{{ title }}</h3>
          <button>Delete</button>
        </header>
        <p>{{ description }}</p>
        <nav>
          <a :href="link">View resource</a>
        </nav>
      </base-card>
    </li>
  </div>
</template>

<script>

export default {

  props: ['title', 'description', 'link']
};
</script>

<style scoped>
li {
  margin: auto;
  max-width: 40rem;
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

h3 {
  font-size: 1.25rem;
  margin: 0.5rem 0;
}

a {
  text-decoration: none;
  text-transform: capitalize;
  color: coral;
}
</style>
