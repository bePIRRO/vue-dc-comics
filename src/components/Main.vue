<template>
  <main>
    <!-- current series tag -->
    <div class="tag">
      CURRENT SERIES
    </div>

    <!-- cards container -->
    <div class="container">
      <div class="row">
        <div class="card">
          <img src="../img/jumbotron.jpg" alt="card" />
          <h5>title serie</h5>
        </div>
      </div>
    </div>
  </main>
</template>

<style>
main {
  background-color: #1c1c1c;
  height: 1000px;
  margin: 0;
}

.container {
  margin: 0;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

.container .row {
  margin-top: 100px;
}

.tag {
  background-color: #0282f9;
  display: inline;
  color: #fff;
  padding: 1.05rem;
  box-shadow: black 5px 2px 2px;
  position: relative;
  left: 20%;
}

.card {
  color: #fff;
  margin: 0 20px;
}

.card img {
  max-width: 185px;
  min-height: 185px;
}
</style>
