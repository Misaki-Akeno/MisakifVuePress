---
lang: zh-CN
title: 页面的标题
description: 页面的描述
---
# 我的测试页面

```md:no-v-pre
<!-- 这里会被 Vue 编译 -->

1 + 2 + 3 = {{ 1 + 2 + 3 }}
```

<span v-for="i in 3"> span: {{ i }} </span>

这是默认主题内置的 `<Badge />` 组件 <Badge text="演示" />


<script setup>
import { ref } from 'vue';
const count = ref(0)
</script>
<button type="button" class="modern-button" @click="count++">无聊的小按钮 {{ count }}</button>

<style scoped>
.modern-button {
  padding: 10px 20px;       /* 按钮内边距 */
  font-size: 16px;          /* 文字大小 */
  font-family: var(--font-family);
  color: white;             /* 文字颜色 */
  background-color: #007BFF; /* 按钮背景颜色 */
  border: none;             /* 移除边框 */
  border-radius: 5px;       /* 边框圆角 */
  cursor: pointer;          /* 鼠标悬停时的指针样式 */
  outline: none;            /* 移除焦点轮廓 */
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); /* 添加阴影效果 */
  transition: all 0.3s;     /* 过渡动画效果 */
}

.modern-button:active {
  background-color: #004085; /* 鼠标点击时的背景颜色 */
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2); /* 鼠标点击时的阴影效果 */
}
</style>