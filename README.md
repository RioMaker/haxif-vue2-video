# haxif-vue2-video
### 安装
npm install haxif-vue2-video --save
### 引用
```html
<template>
  <div>
    <!-- 
      title 快捷标题 不推荐使用
      :speeds 倍速控制器自定义 传值必须数组类型 为保持位数应为String类型内容
      :festival 节日图标，暂只开放已下三种【'bilibili','Bug','Spring Festival'】
     -->
    <haxif-video
      title="快捷标题"
      :speeds="['2.0', '1.5', '1.0', '0.5', '0.25']"
    >
      <!-- 自定义表头 -->
      <template #title>
        <div style="xxx">
          <h1>标题</h1>
          任意自定义内容，只需保持在规定宽度内即可
        </div>
      </template>
      <!-- 支持直接插入Local视频资源 -->
      <source src="../assets/海浪30.mp4">
    </haxif-video>
  </div>
</template>
<script>
import haxifVideo from 'haxif-vue2-video'
export default {
  components:{
    haxifVideo
  },
}
</script>
```