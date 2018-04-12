<template>
  <mu-flexbox>
    <mu-flexbox-item class="flex-demo" grow='1'>
    </mu-flexbox-item>
    <mu-flexbox-item class="flex-demo person" grow='5'>
      <mu-paper class="demo-paper" circle :zDepth="1" />
      <mu-list>
        <mu-list-item title="Inbox">
          <mu-icon slot="left" value="inbox" />
        </mu-list-item>
        <mu-list-item title="Starred">
          <mu-icon slot="left" value="grade" />
        </mu-list-item>
        <mu-list-item title="Sent mail">
          <mu-icon slot="left" value="send" />
        </mu-list-item>
        <mu-list-item title="Drafts">
          <mu-icon slot="left" value="drafts" />
        </mu-list-item>
      </mu-list>
      <mu-divider />
      <mu-list>
        <mu-list-item title="All mail">
          <mu-icon slot="right" value="info" />
        </mu-list-item>
        <mu-list-item title="Trash">
          <mu-icon slot="right" value="info" />
        </mu-list-item>
        <mu-list-item title="Spam">
          <mu-icon slot="right" value="info" />
        </mu-list-item>
        <mu-list-item title="Follow up">
          <mu-icon slot="right" value="info" />
        </mu-list-item>
      </mu-list>
    </mu-flexbox-item>
    <mu-flexbox-item class="flex-demo" grow='0'>
    </mu-flexbox-item>
  </mu-flexbox>
</template>

<script>
  export default {}
</script>

<style scoped>
  .flex-demo {
    min-height: 32px;
    /* background-color: #e0e0e0; */
    text-align: center;
    line-height: 32px;
  }
  .person {
    /* border: 1px dashed darkgray; */
  }
  .demo-paper {
    display: inline-block;
    height: 150px;
    width: 150px;
    margin: 20px;
    text-align: center;
    background: url(http://www.muse-ui.org/images/uicon.jpg) no-repeat center;
  }
</style>
