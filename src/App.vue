<template>
  <div class="layout">
    <div class="header">
      <mu-appbar title="Title">
        <mu-icon-button icon="menu" slot="left" />
        <mu-text-field icon="search" class="appbar-search-field" slot="right" hintText="请输入搜索内容" @change="submit" />
        <mu-flat-button color="white" label="flat Button" slot="right" />
      </mu-appbar>
    </div>
    <div class="content">
      <div class="content-left">
        <content-left></content-left>
      </div>
      <div class="content-center">
        <content-center></content-center>
      </div>
      <div class="content-right">
        <content-right></content-right>
      </div>
    </div>
    <div class="footer">
      martin-chen ©2018 Created by vue-dataMock
    </div>
  </div>
</template>

<script>
  import ContentLeft from '@/containers/ContentLeft'
  import ContentCenter from '@/containers/ContentCenter'
  import ContentRight from '@/containers/ContentRight'
  export default {
    data() {
      return {
        activeTab: 'tab1',
        activeList: 'list1'
      }
    },
    methods: {
      handleTabChange(val) {
        this.activeTab = val
      },
      handleListChange(val) {
        this.activeList = val
      },
      submit(val) {
        console.log(val.target.value)
      }
    },
    components: {
      ContentLeft,
      ContentRight,
      ContentCenter
    }
  }
</script>

<style scoped>
  .layout {
    background-color: rgb(236, 236, 236);
    display: flex;
    flex-flow: column;
    /* height: 100vh; */
  }
  .header {
    background-color: #7e57c2;
  }
  .logo {
    font-size: 24px;
    color: white;
    display: inline-block;
    padding: 10px 20px;
  }
  .nav {
    display: inline-block;
    width: calc(100% - 150px);
    margin: 0 auto;
  }
  .tab {
    margin: 0 auto;
    width: 400px;
    background-color: rgba(0, 0, 0, 0);
  }
  .content {
    /* overflow: hidden; */
    flex: 1;
    display: flex;
  }
  .content-left {
    flex: 3;
    float: left;
    background-color: white;
    padding: 10px 10px;
    background-color: rgba(0, 0, 0, 0)
    /* margin-bottom: -4000px; */
    /* padding-bottom: 4000px; */
  }
  .content-center {
    flex: 6;
    padding: 10px 10px;
    background-color: rgba(0, 0, 0, 0)
  }
  .content-right {
    flex: 3;
    display: inline-block;
    float: right;
    padding: 10px 10px;
    background-color: rgba(0, 0, 0, 0)
  }
  .breadcrumb {
    margin: 10px 0;
  }
  .body {
    background-color: white;
    border-radius: 5px;
    min-height: 500px;
  }
  .footer {
    padding: 20px 0;
    text-align: center;
    flex: 0
  }
</style>
