<template>
  <div class="container">
    <div class="row">
      <div class="col-sm-12">
        <div class="col-sm-10 col-sm-offset-1 text-center">
          <div class="four_zero_four_bg">
            <h1 class="text-center">404</h1>
          </div>
          <div class="contant_box_404">
            <h2>Page not found!</h2>
            <router-link :to="{ name: 'Table' }" class="link_404"
              >Go to Home</router-link
            >
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.page_404 {
  padding: 40px 0;
  background: #fff;
  font-family: "Arvo", serif;
}

.page_404 img {
  width: 100%;
}

.four_zero_four_bg h1 {
  font-size: 80px;
}

.four_zero_four_bg h3 {
  font-size: 80px;
}

.link_404 {
  color: #fff;
  padding: 10px 20px;
  background: #39ac31;
  margin: 20px 0;
  display: inline-block;
}
</style>
