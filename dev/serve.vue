<script>
import Vue from 'vue';
// Uncomment import and local "components" registration if library is not registered globally.
// import { JmgayossoIpfsComponentsVueSample } from '@/entry.esm';
import { IpfsUploaderFile, IpfsImageViewer } from '@/entry.esm'

export default Vue.extend({
  name: 'ServeDev',
  components: {
    IpfsUploaderFile,
    IpfsImageViewer
  }
});
</script>

<template>
  <div id="app">
    <ipfs-uploader-file />
    <ipfs-image-viewer />
  </div>
</template>
