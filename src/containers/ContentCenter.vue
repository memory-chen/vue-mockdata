<template>
  <div>
    <p class="btn-right">
      <mu-raised-button class="demo-raised-button" label="发布" primary>
        <i class="mdui-icon material-icons">&#xe3ba;</i>
      </mu-raised-button>
    </p>
    <mu-card v-for="(data,index) in 5" :key="index">
      <mu-card-header title="陈灏" subTitle="指尖的阳光">
        <mu-avatar src="http://www.muse-ui.org/images/uicon.jpg" slot="avatar" />
      </mu-card-header>
      <mu-card-media title="阳光漫延" subTitle="阳光漫延">
        <img src="http://www.muse-ui.org/images/sun.jpg" />
      </mu-card-media>
      <mu-card-title title="红叶阳光" />
      <mu-card-text>
        散落在指尖的阳光，我试着轻轻抓住光影的踪迹，它却在眉宇间投下一片淡淡的阴影。 调皮的阳光掀动了四月的心帘，温暖如约的歌声渐起。 似乎在诉说着，我也可以在漆黑的角落里，找到阴影背后的阳光， 找到阳光与阴影奏出和谐的旋律。我要用一颗敏感赤诚的心迎接每一缕滑过指尖的阳光！
      </mu-card-text>
        <!-- <mu-card-actions>
          <mu-flat-button label="Action 1" />
          <mu-flat-button label="Action 2" />
        </mu-card-actions> -->
    </mu-card>
  </div>
</template>

<script>
  export default {}
</script>

<style scoped>
  .btn-right {
    text-align: right;
    padding-right: 10px;
  }
  .mu-card{
    margin: 5px 0px;
  }
</style>
