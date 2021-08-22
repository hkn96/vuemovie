<template>
  <div class="home">
    <div class="feature-card">
      <router-link to="/movie/tt0409591">
        <img
          class="featured-img"
          src="https://occ-0-3568-3212.1.nflxso.net/dnm/api/v6/9pS1daC2n6UGc3dUogvWIPMR_OU/AAAABfMeHBEISlGky5F9xeESoO8bMuqxAbHr_fwF3oVeR5g_rZkYB_ESRB3HT_GZrW8g0wYOZRNfoi6n3vi7MaxCHnxBUTH_POCCWRlSqrX2L1njcIvT.jpg?r=33a"
          alt="Naruto Poster"
        />
        <div class="detail">
          <h3>Naruto</h3>
          <p>
            Guided by the spirit demon within him, orphaned Naruto learns to
            harness his powers as a ninja in this anime adventure series.
          </p>
        </div>
      </router-link>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
};
</script>

<style lang="scss">
.home {
  .feature-card {
    position: relative;
    .featured-img {
      display: block;
      width: 100%;
      height: 300px;
      object-fit: cover;
      position: relative;
      z-index: 0;
    }
    .detail {
      position: absolute;
      left: 0;
      right: 0;
      bottom: 0;
      background-color: rgba(0, 0, 0, 0.6);
      padding: 16px;
      z-index: 1;
      h3 {
        color: #fff;
        margin-bottom: 16px;
      }
      p {
        color: #fff;
      }
    }
  }
}
</style>
