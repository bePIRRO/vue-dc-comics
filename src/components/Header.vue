<template>
  <header>
    <!-- navbar -->
    <div class="navbar">
      <div class="row">
        <div class="col">
          <a href="#" id="logo"
            ><img src="@/img/dc-logo.png" alt="DC Comics"
          /></a>
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
    </div>

    <!-- hero -->

    <div id="hero"></div>
  </header>
</template>

<style>
.navbar {
  background-color: #fff;
}

.row {
  display: flex;
  justify-content: space-around;
  align-items: center;
  height: 100px;
}

.active,
a:hover:not(#logo) {
  color: #0282f9;
  border-bottom: 2px solid #0282f9;
}

.row div {
  display: inline-block;
  height: auto;
}

img {
  width: auto;
  max-height: 80px;
}

.col,
ul,
li {
  height: auto;
}

li {
  list-style-type: none;
  display: inline;
}

a {
  color: #000;
  text-decoration: none;
  margin: 0 10px;
}

#hero {
  width: 100vw;
  height: 400px;
  background-image: url("../img/jumbotron.jpg");
  background-repeat: no-repeat;
  background-size: cover;
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
