<template>
  <h1>Welcome to Reise-Forum</h1>
  <div id="carouselExampleControls" class="carousel slide" data-ride="carousel">
    <div class="carousel-inner">
      <div class="carousel-item active">
        <img class="d-block w-100" src="../assets/Sakura.jpg" alt="Second slide">
      </div>
      <div class="carousel-item">
        <img class="d-block w-100" src="../assets/berlinerDom.jpg" alt="Third slide">
      </div>
    </div>
    <a class="carousel-control-prev" href="#carouselExampleControls" role="button" data-slide="prev">
      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      <span class="sr-only">Previous</span>
    </a>
    <a class="carousel-control-next" href="#carouselExampleControls" role="button" data-slide="next">
      <span class="carousel-control-next-icon" aria-hidden="true"></span>
      <span class="sr-only">Next</span>
    </a>
  </div>
  <div class="container-fluid">
    <div class="row row-cols-1 row-cols-nd-4 g-4">
      <div class="col" v-for="reise in reisen" :key="reise.id">
        <div class="card h-100">
          <img src="../assets/gobi.jpg" class="card-img-top" :alt="reise.landname + ' ' + reise.reisename">
          <div class="card-body">
            <h5 class="card-title">{{reise.landname}} {{reise.reisename}}</h5>
            <p class="card-text">
              {{reise.landname}} {{reise.reisename}} {{reise.description}} {{reise.vote.length}}
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ReisenView',
  data () {
    return {
      reisen: [
        {
          id: 1,
          landname: 'Mongolei',
          reisename: 'Gobi',
          description: 'Die Gobi ist der zentrale Teil des Mongolischen Beckens. Es ist eine ausgedehnte flache Hochebene, die durchschnittlich 1500 m über dem Meeresspiegel liegt.',
          vote: []
        },
        {
          id: 2,
          landname: 'Deutschland',
          reisename: 'Berliner Dom',
          description: 'Der Berliner Dom ist eine evangelische Kirche im Zentrum Berlins und ein wahres Universum, das es zu entdecken gilt.',
          vote: [1,2,3]
        }
      ]
    }
  }
}
</script>

<style scoped>

</style>
