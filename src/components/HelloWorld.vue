<template>

<button v-on:click="suckit" style="margin-left: 47.5%">suckit</button>
  <DxPopup
  v-model:visible="popupVisible"
  :close-on-outside-click="true"
  :show-close-button="true"
   id='anus'
    :width="550"
    :height="350"
    :visible="true"
    :show-title="false"
   
  > 
    <template #content>
      <DxScrollView
        width="100%"
        height="100%"
      >
  <button v-on:click ="fuckyou" style="margin-left: 46.5%">anus</button>
        <div id="textBlock">
          The <b>ScrollView</b> allows users to scroll its content vertically.
          To enable horizontal and vertical scrolling, set the <b>direction</b>
          option to <i>&quot;both&quot;</i>. Horizontal scrolling is available
          only if the content is wider than the <b>ScrollView</b>. Otherwise,
          the content adapts to the widget&apos;s width.<br><br>The <b>ScrollView</b>
          uses native scrolling on most platforms, except desktops. To use it on all
          platforms, assign <b>true</b> to the <b>useNative</b> option. If you assign
          <b>false</b>, scrolling is simulated on all platforms.The <b>ScrollView</b> allows users to scroll its content vertically.
          To enable horizontal and vertical scrolling, set the <b>direction</b>
          option to <i>&quot;both&quot;</i>. Horizontal scrolling is available
          only if the content is wider than the <b>ScrollView</b>. Otherwise,
          the content adapts to the widget&apos;s width.<br><br>The <b>ScrollView</b>
          uses native scrolling on most platforms, except desktops. To use it on all
          platforms, assign <b>true</b> to the <b>useNative</b> option. If you assign
          <b>false</b>, scrolling is simulated on all platforms.The <b>ScrollView</b> allows users to scroll its content vertically.
          To enable horizontal and vertical scrolling, set the <b>direction</b>
          option to <i>&quot;both&quot;</i>. Horizontal scrolling is available
          only if the content is wider than the <b>ScrollView</b>. Otherwise,
          the content adapts to the widget&apos;s width.<br><br>The <b>ScrollView</b>
          uses native scrolling on most platforms, except desktops. To use it on all
          platforms, assign <b>true</b> to the <b>useNative</b> option. If you assign
          <b>false</b>, scrolling is simulated on all platforms.The <b>ScrollView</b> allows users to scroll its content vertically.
          To enable horizontal and vertical scrolling, set the <b>direction</b>
          option to <i>&quot;both&quot;</i>. Horizontal scrolling is available
          only if the content is wider than the <b>ScrollView</b>. Otherwise,
          the content adapts to the widget&apos;s width.<br><br>The <b>ScrollView</b>
          uses native scrolling on most platforms, except desktops. To use it on all
          platforms, assign <b>true</b> to the <b>useNative</b> option. If you assign
          <b>false</b>, scrolling is simulated on all platforms.
        </div>
      </DxScrollView>
    </template>
  
  </DxPopup>
</template>
<script>
import { DxPopup } from 'devextreme-vue/popup';
import { DxScrollView } from 'devextreme-vue/scroll-view';
export default {
  components: {
    DxPopup,
    DxScrollView,
  },
  data() {
    return {
      popupVisible: false
    }
  },
  
methods: {

fuckyou() { alert('ass');
this.popupVisible = false
},

suckit() { alert('tits');
this.popupVisible = true
}
  },

};
</script>
<style>
#textBlock {
  padding-left: 20px;
  padding-right: 20px;
  line-height: 1.6em;
}

.center {
  display: block;
  margin-left: auto;
  margin-right: auto;
  padding-top: 20px;
  width: 300px;
}
</style>
