<a href="https://vuejs.org/">
    <img src="https://img.shields.io/badge/vue-%3E=2.0.0-brightgreen.svg" alt="Vue version"/>
</a>

# vue-plugin（这个只是记录一下开发 Vue 插件的过程，没有发布 npm）

- Tiny and very very easy to use.

- List with high performance.

- Sort automatically by initials.

## Live demos

- [vue-plugin](#).

## Simple usage

```
npm install vue-plugin or yarn add vue-plugin
```

```vue
// main.js import VuePlugin from 'vue-plugin' Vue.use(VuePlugin) // app.js
<template>
  <div>
    <vue-plugin :options="options" @change="cb" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      options: [
        {
          name: "上海市",
          tags: "SHANGHAI,上海市",
          cityid: 4
        },
        {
          name: "深圳市",
          tags: "SHENZHEN,深圳市",
          cityid: 2
        },
        {
          name: "广州市",
          tags: "GUANGZHOU,广州市",
          cityid: 3
        },
        {
          name: "武汉市",
          tags: "WUHAN,武汉市",
          cityid: 6
        }
      ]
    };
  }
};
</script>
```

## Notice

- The `key` of the passed in `options` for sorting attribute values must be `name`

## Props type

| _Prop_  | _Type_ | _Required_ | _Description_                                                                       |
| :------ | :----- | :--------- | :---------------------------------------------------------------------------------- |
| options | Array  | ✓          | Incoming data list, as long as each object's name attribute is a value for sorting. |

## Contributions

Welcome to improve vue-plugin with any issue, pull request or code review.

## Changelogs

Maintain and update occasionally, for changes see [release](https://github.com/xxj95719/vue-plugin/releases).
