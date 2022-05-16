<script>
import Vue from 'vue';
// Uncomment import and local "components" registration if library is not registered globally.
// import { JmgayossoIpfsComponentsVueSample } from '@/entry.esm';
import { IpfsUploaderFile, IpfsImageViewer, testFunction } from '@/entry.esm'

export default Vue.extend({
  name: 'ServeDev',
  components: {
    IpfsUploaderFile,
    IpfsImageViewer
  },
  methods: {
    test() {
      testFunction()
    }
  }
});
</script>

<template>
  <div id="app">
    <ipfs-uploader-file @onEvent="test" />
    <ipfs-image-viewer />
  </div>
</template>
