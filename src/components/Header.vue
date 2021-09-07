<template>
  <header class="navbar">
    <div class="row">
      <div class="col">
        <a href="#" id="logo"><img src="@/img/dc-logo.png" alt="DC Comics"/></a>
      </div>
      <div class="col">
        <ul>
          <li v-for="(link, index) in links" :key="index">
            <a :href="link.url" :class="{ active: link.current }">{{
              link.text
            }}</a>
          </li>
        </ul>
      </div>
    </div>
  </header>
</template>

<style>
.navbar {
  background-color: #fff;
  height: 100px;
}

.row {
  display: flex;
  justify-content: space-around;
  align-items: center;
  height: auto;
}

.active,
a:hover:not(#logo) {
  border-bottom: 2px solid blue;
}

.row div {
  display: inline-block;
  height: auto;
}

li {
  list-style-type: none;
  display: inline;
  height: auto;
}

a {
  color: #000;
  text-decoration: none;
  margin: 0 10px;
}
</style>

<script>
export default {
  name: "Header",
  data() {
    return {
      links: [
        {
          text: "Characters",
          url: "#",
          current: false,
        },
        {
          text: "Comics",
          url: "#",
          current: true,
        },
        {
          text: "Movies",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "Games",
          url: "#",
          current: false,
        },
        {
          text: "Collectibles",
          url: "#",
          current: false,
        },
        {
          text: "Videos",
          url: "#",
          current: false,
        },
        {
          text: "Fans",
          url: "#",
          current: false,
        },
        {
          text: "News",
          url: "#",
          current: false,
        },
        {
          text: "Shop",
          url: "#",
          current: false,
        },
      ],
    };
  },
};
</script>
