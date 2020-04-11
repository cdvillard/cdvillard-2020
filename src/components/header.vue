<template>
  <header class="header">
    <g-image class="headshot" src="../../static/images/cdv-headshot.jpg" />
    <div class="header__navigation">
      <strong class="name">
        <g-link to="/">{{ $static.metadata.siteName }}</g-link>
      </strong>
      <nav class="nav">
        <g-link class="nav__link" to="/about/">About</g-link>
        <g-link class="nav__link" to="/about/">Work</g-link>
        <g-link class="nav__link" to="/about/">Blog</g-link>
      </nav>
    </div>
  </header>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<script>
export default {};
</script>

<style lang="scss">
.header {
  background: rebeccapurple;
  display: flex;
  flex-flow: row nowrap;
  justify-content: center;
  align-items: center;
  padding: 1rem;
  overflow-x: hidden;

  &__navigation {
    .name {
      font-size: 2.5rem;
      text-transform: uppercase;
      line-height: 1.25;
      > * {
        color: #fff;
      }
    }
    .nav {
      /* padding-left: 3.5rem; */

      .nav__link {
        font-size: 1.25rem;
        color: white;
      }
    }
  }

  .headshot {
    width: auto;
    height: 15rem;
    border-radius: 50%;
    margin-right: -2.5rem;
  }

  .nav__link {
    /* margin-left: 20px; */
  }
}
</style>
