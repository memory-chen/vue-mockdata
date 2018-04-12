<template>
  <div class="gridlist-demo-container">
  <mu-grid-list class="gridlist-demo" >
    <mu-sub-header>推荐</mu-sub-header>
    <mu-grid-tile class="tj-image">
      <img src="http://www.muse-ui.org/images/breakfast.jpg"/>
      <span slot="title">{{'Breakfast'}}</span>
      <span slot="subTitle">by <b>{{'tile.author'}}</b></span>
      <mu-icon-button icon="star_border" slot="action"/>
    </mu-grid-tile>
  </mu-grid-list>
</div>
</template>

<script>
  export default {
  }
</script>

<style scoped>
.gridlist-demo-container{
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
}

.gridlist-demo{
  /* width: 500px; */
  /* height: 450px; */
  /* overflow-y: auto; */
}
.tj-image{
  width: 100% !important;
}
.mu-grid-tile > img{
  width: 100%;
}
</style>
