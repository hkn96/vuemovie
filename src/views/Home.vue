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
    <form @submit.prevent="" class="search-box">
      <input type="text" placeholder="Wonach suchst du?" />
      <input type="submit" value="Search" />
    </form>
    <div class="movies-list">MOVIES</div>
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
  .search-box {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 16px;

    input {
      display: block;
      appearance: none;
      border: none;
      outline: none;
      background: none;

      &[type='text'] {
        width: 100%;
        color: #fff;
        background-color: #496583;
        font-size: 20px;
        padding: 10px 16px;
        border-radius: 8px;
        margin-bottom: 15px;
        transition: 0.4s;

        &::placeholder {
          color: #f3f3f3;
        }

        &:focus {
          box-shadow: 0px 3px 6px rgba(0, 0, 0, 0.6);
        }
      }
      &[type='submit'] {
        width: 100%;
        max-width: 300px;
        background-color: #42b883;
        padding: 16px;
        border-radius: 8px;
        color: #fff;
        font-size: 20px;
        text-transform: uppercase;
        transition: 0.4s;

        &:active {
          background-color: #3b8070;
        }
      }
    }
  }
}
</style>
