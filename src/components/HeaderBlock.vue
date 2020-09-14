<template>
  <div class="section-dark wrapper">
    <div class="text-grid">
        <div class="fmname">
          <div class="fname">Cael</div>
          <div class="mname">Ryker</div>
        </div>
        <div class="lname">Mosh</div>
        <div class="header-menu">
          <ul>
            <li><a href="#" @click.prevent>About Me</a></li>
            <li><a href="#" @click.prevent>Projects</a></li>
            <li><a href="#" @click.prevent>Resume</a></li>
            <li><a href="#" @click.prevent>Github</a></li>
          </ul>
        </div>
    </div>
  </div>
</template>

<script>
  // import headerStreakVertical from '../assets/header-streak-vertical.png';
  export default {
    data: function () {
      return {
        // headerStreakVertical 
      };
    }
  }
</script>

<style scoped>
  .wrapper {
    height: 600px;
    font-family: 'Rubik Mono One', sans-serif;
    color: #fffff3;
    border-bottom: 15px solid #d00;
    background-image: url('../assets/streak-vertical.svg'), url('../assets/mosh-m.svg'), url('../assets/grid-straight.svg');
    background-position: calc(50% + 108px) 0, 10px calc(100% - 10px), center;
    background-repeat: no-repeat, no-repeat, repeat;
    background-size: auto 80%, 40% auto, 60px;
  }
  .text-grid {
    display: inline-grid;
    grid-template-columns: max-content auto;
    grid-template-rows: max-content auto;
    margin-top: 4rem;
    margin-right: 2rem;
    text-transform: uppercase;
  }
  .fmname {
    grid-column-start: 1;
    grid-row-start: 1;
    text-align: right;
    padding-bottom: 0.5rem;
  }
  .fname {
    height: 4.2rem;
    font-size: 4.2rem;
    line-height: 1;
  }
  .mname {
    height: 5.5rem;
    font-size: 5.5rem;
    line-height: 1;
  }
  .lname {
    grid-column-start: 2;
    grid-row-start: 1;
    grid-row-end: 3;
    writing-mode: vertical-rl;
    width: 8rem;
    font-size: 8rem;
    text-align: left;
    line-height: 1;
  }
  .header-menu {
    grid-column-start: 1;
    grid-row-start: 2;
    text-align: right;
    font-size: 2.4rem;
    line-height: 1.35;
  }
  .header-menu ul {
    float: right;
    margin: 0;
    padding: 0;
    padding-top: 1rem;
    list-style-type: none;
    border-top: 3px solid #fffff3;
  }
  .header-menu a {
    color: #fffff3;
    text-decoration: none;
  }
  .header-menu a:hover {
    color: #d00;
    text-decoration: none;
  }
  @media(min-width: 768px) {
    .wrapper {
      height: 700px;
      background-image: url('../assets/streak-diagonal.svg'), url('../assets/mosh-m.svg'), url('../assets/grid-diagonal.svg');
      background-position: 8.5rem top, calc(100% - 10px) 10px, -16rem 0;
      background-repeat: no-repeat, no-repeat, no-repeat;
      background-size: auto 75%, 32% auto, auto 100%;
      text-align: left;
    }
    .text-grid {
      transform: rotate(-45deg);
      margin-top: 11rem;
      margin-left: 5rem;
      margin-right: 0;
    }
    .fname {
      height: 6rem;
      font-size: 6rem;
    }
    .mname {
      height: 8rem;
      font-size: 8rem;
    }
    .lname {
      width: 14rem;
      font-size: 13rem;
    }
    .header-menu {
      writing-mode: vertical-rl;
      text-align: left;
      font-size: 3rem;
      line-height: 1.4;
    }
    .header-menu ul {
      float: none;
      padding-top: 2.5rem;
    }
  }
  @media(min-width: 991px) {
    .wrapper {
      background-position: 12rem top, calc(100% - 10px) 10px, -12rem 0;
      background-size: auto 90%, 32% auto, auto 100%;
    }
    .text-grid {
      margin-top: 12rem;
      margin-left: 5rem;
    }
    .fname {
      height: 8rem;
      font-size: 8rem;
    }
    .mname {
      height: 10rem;
      font-size: 10rem;
    }
    .lname {
      width: 17rem;
      font-size: 16rem;
    }
    .header-menu {
      font-size: 3rem;
      line-height: 1.4;
    }
    .header-menu ul {
      padding-top: 2.5rem;
    }
  }
  @media(min-width: 1200px) {
    .wrapper {
      background-size: auto 90%, auto 60%, auto 100%;
    }
  }
</style>