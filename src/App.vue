<template>
  <a-layout style="min-height:100vh">
    <!-- Menu -->
    <Menu/>
    <a-layout>
      <!-- Header -->
      <Header/>
      <!-- Content -->
      <Content/>
    </a-layout>
  </a-layout>
</template>
<script lang="ts">
import {
  UserOutlined,
  VideoCameraOutlined,
  UploadOutlined,
  MenuUnfoldOutlined,
  MenuFoldOutlined,
} from "@ant-design/icons-vue";
import Menu from "./components/core/Menu.vue";
import Header from "./components/core/Header.vue";
import Content from "./components/core/Content.vue";
import { defineComponent, ref } from "vue";
export default defineComponent({
  components: {
    Content,
    Header,
    Menu,
    
    
  },
  setup() {
    return {
      selectedKeys: ref<string[]>(["1"]),
      collapsed: ref<boolean>(false),
    };
  },
});
</script>

