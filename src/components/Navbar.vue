<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <a class="navbar-brand" href="#">Reise Forum</a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
      <div class="navbar-nav">
        <routerlink class="nav-item nav-link" to="/">Home</routerlink>
        <routerlink class="nav-item nav-link" to="/about">About</routerlink>
        <routerlink class="nav-item nav-link" to="/reisen">Reise</routerlink>
        <!--        <a class="nav-item nav-link active" aria-current="page" href="#">Home</a>-->
        <!--        <a class="nav-item nav-link" href="#">About</a>-->
        <!--       <a class="nav-item nav-link" href="#">Reise</a>-->
        <!--        <form class="form-inline">
                  <input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">
                  <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
                </form>-->
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "NavbarComponent"
}
</script>

<style scoped>

</style>
