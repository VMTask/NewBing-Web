<template>
  <a-layout-content style="margin: 0 16px">
    <a-breadcrumb style="margin: 16px 0">
      <a-breadcrumb-item>主页</a-breadcrumb-item>
      <a-breadcrumb-item>聊天</a-breadcrumb-item>
    </a-breadcrumb>
    <div :style="{ padding: '24px', background: '#fff', minHeight: '360px' }">
      <Chat_view />
    </div>
  </a-layout-content>
</template>
<script lang="ts">
import chat_view from './chat_view.vue';
import { Breadcrumb , BreadcrumbItem,LayoutContent} from "ant-design-vue"
export default {
  components: {
    ABreadcrumb: Breadcrumb,
    ABreadcrumbItem: BreadcrumbItem,
    ALayoutContent: LayoutContent,
    Chat_view: chat_view
  }
}
</script>