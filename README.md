# dgiot_vue_amis

## about

- This project is based on [vuera](https://github.com/akxcv/vuera) and mainly focuses on the encapsulation of [amis-editor](https://www.npmjs.com/package/amis-editor)
- You can edit at [this](https://dgiot_vue_amis.vercel.app/). The [proxy](https://github.com/dgiot/dgiot_vue_amis/blob/master/vercel.json) mode is enabled. You can copy the JSON of [amis](https://aisuda.bce.baidu.com/amis/examples/index). It supports direct rendering

<div align="center">

[![language](https://img.shields.io/github/languages/top/h7ml/dgiot_vue_amis)](https://github.com/dgiot/dgiot_vue_amis/search?l=css)
[![last](https://img.shields.io/github/last-commit/h7ml/dgiot_vue_amis.svg)](https://github.com/dgiot/dgiot_vue_amis/commits)
[![stars](https://img.shields.io/badge/Hosted-Vercel-brightgreen?style=flat&logo=Vercel)](https://amis.vercel.app/)
[![amis](https://img.shields.io/badge/amis-1.9.0-red.svg)](https://www.npmjs.com/package/amis/v/1.9.0)
[![amis-editor](https://img.shields.io/badge/amisEditor-4.1.0.20-red.svg)](https://www.npmjs.com/package/amis-editor/v/4.1.0-beta.20)

<img alt="npm" src="https://img.shields.io/npm/v/amis-editor">
<img src="https://img.shields.io/github/commit-activity/m/h7ml/dgiot_vue_amis" alt="ommit-activity">
<img src="https://badgen.net/badge/package/dgiot_vue_amis/blue"
alt="package" maxretrytimes="3" class="m-1 transition-all duration-1000">
<img src="https://badgen.net/npm/v/dgiot_vue_amis" alt="Npm Version"
maxretrytimes="3" class="m-1 transition-all duration-1000">
<img src="https://badgen.net/npm/node/dgiot_vue_amis" alt="Node Version"
maxretrytimes="3" class="m-1 transition-all duration-1000">
<br>
<img src="https://badgen.net/packagephobia/install/dgiot_vue_amis"
alt="Install Size" maxretrytimes="3" class="m-1 transition-all duration-1000">
<img src="https://badgen.net/npm/types/dgiot_vue_amis" alt="Type Support"
maxretrytimes="3" class="m-1 transition-all duration-1000">
<br>
<img src="https://img.shields.io/librariesio/release/npm/dgiot_vue_amis"
alt="Outdated Dep" maxretrytimes="3" class="m-1 transition-all duration-1000">
<img src="https://img.shields.io/snyk/vulnerabilities/npm/dgiot_vue_amis"
alt="Vulnerablities" maxretrytimes="3" class="m-1 transition-all duration-1000">
<a href="https://www.npmjs.com/package/dgiot_vue_amis"><img src="https://img.shields.io/npm/l/dgiot_vue_amis" alt="License"></a>

</div>

## Installation

```bash
yarn add dgiot_vue_amis @fortawesome/fontawesome-free --save
```

## Quick Start

### [App.vue](https://github.com/dgiot/dgiot_vue_amis/blob/master/examples/App.vue#L1)

```javascript
<template>
  <div id='app'>
    <dgiot_vue_amis
      id='editorName'
      theme='cxd'
      className='is-fixed'
      :preview='isPreview'
      :isMobile='isMobile'
      @onChange='onChange'
      :value='schema'
    />
  </div>
</template>
<script>
import "amis-ui/lib/themes/cxd.css";
import "amis-ui/lib/themes/ang.css";
import "amis-editor/dist/style.css";
export default {
  name: 'App',
  data() {
    return {
      isPreview: false,
      isMobile: false,
      schema: {}
    }
  },
  methods: {
    onChange(e) {
      console.log(e)
    }
  }
}
</script>

```

### version

| [dgiot_vue_amis](https://www.npmjs.com/package/dgiot_vue_amis)                                                                           | [amis](https://www.npmjs.com/package/amis)                                                                 | [amis-editor](https://www.npmjs.com/package/amis-editor)                                                                             |
|--------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------|
| [![amis-editor](https://badgen.net/badge/dgiot_vue_amis/1.10.0/blue)](https://www.npmjs.com/package/dgiot_vue_amis/v/1.10.0)             | [![amis](https://img.shields.io/badge/amis-1.10.0-green.svg)](https://www.npmjs.com/package/amis/v/1.10.0) | [![amis-editor](https://badgen.net/badge/amis-editor/4.1.0-beta.28/blue)](https://www.npmjs.com/package/amis-editor/v/4.1.0-beta.28) |
| [![amis-editor](https://badgen.net/badge/dgiot_vue_amis/2.0.0-beta.5/blue)](https://www.npmjs.com/package/dgiot_vue_amis/v/2.0.0-beta.5) | [![amis](https://img.shields.io/badge/amis-2.0.0-green.svg)](https://www.npmjs.com/package/amis/v/2.0.0)   | [![amis-editor](https://badgen.net/badge/amis-editor/4.2.0-beta.3/blue)](https://www.npmjs.com/package/amis-editor/v/4.2.0-beta.3)   |
| [![amis-editor](https://badgen.net/badge/dgiot_vue_amis/2.0.1-beta.1/blue)](https://www.npmjs.com/package/dgiot_vue_amis/v/2.0.1-beta.1) | [![amis](https://img.shields.io/badge/amis-2.0.1-green.svg)](https://www.npmjs.com/package/amis/v/2.0.1)   | [![amis-editor](https://badgen.net/badge/amis-editor/5.1.8/blue)](https://www.npmjs.com/package/amis-editor/v/5.1.8)                 |
| [![amis-editor](https://badgen.net/badge/dgiot_vue_amis/2.0.2-beta.1/blue)](https://www.npmjs.com/package/dgiot_vue_amis/v/2.0.2-beta.1) | [![amis](https://img.shields.io/badge/amis-2.0.2-green.svg)](https://www.npmjs.com/package/amis/v/2.0.2)   | [![amis-editor](https://badgen.net/badge/amis-editor/5.1.8/blue)](https://www.npmjs.com/package/amis-editor/v/5.1.8)                 |
| [![amis-editor](https://badgen.net/badge/dgiot_vue_amis/2.1.0/blue)](https://www.npmjs.com/package/dgiot_vue_amis/v/2.1.0)               | [![amis](https://img.shields.io/badge/amis-2.1.0-green.svg)](https://www.npmjs.com/package/amis/v/2.1.0)   | [![amis-editor](https://badgen.net/badge/amis-editor/5.2.0/blue)](https://www.npmjs.com/package/amis-editor/v/5.2.0)                 |
| [![amis-editor](https://badgen.net/badge/dgiot_vue_amis/2.2.0/blue)](https://www.npmjs.com/package/dgiot_vue_amis/v/2.2.0)               | [![amis](https://img.shields.io/badge/amis-2.2.0-green.svg)](https://www.npmjs.com/package/amis/v/2.2.0)   | [![amis-editor](https://badgen.net/badge/amis-editor/5.2.0/blue)](https://www.npmjs.com/package/amis-editor/v/5.2.0)                 |

### repo

- [dgiot_vue_amis editor](https://dgiot_vue_amis.vercel.app/)
- [dgiot_vue_amis repo](https://github.com/dgiot/dgiot_vue_amis)
- [dgiot-dashboard](https://github.com/dgiot/dgiot-dashboard)
- [amis-vue-template](https://github.com/kevin361419446/amis-vue-template)
