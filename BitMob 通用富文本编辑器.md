# BitMob 通用富文本编辑器

## 阶段性目标
### 第一阶段: 核心富文本编辑器

#### 基本功能
- 粘贴时清除原有格式
- 输出 `html` 代码

#### 工具栏
- 文字加粗
- 文字斜体
- 文字超链接
- 文字下划线
- 文字中间划掉
- 选择字体
- 选择字号
- 文字背景颜色
- 首行缩进
- 两端缩进
- 文字左对齐/右对齐/两端对齐
- 行间距
- 段间距
- 字间距
- 有序 / 无序列表
- 清除格式
- 插入图片（上传或引用 URL）
- 引用 (quoteblock)

#### 可选字体
- 思源黑体
- 思源宋体
- Helvetica Neue
- (待🦄️🈹补充)

#### 可选字号
- H1 ~ H6

#### 图片格式
- JPG / JPEG
- PNG
- GIF

#### 快捷键
- 选择文字后按 `crtl/cmd + B` 字体加粗
- 选择文字后按 `crtl/cmd + I` 字体倾斜

<br/>

### 第二阶段
#### 新增功能
- 支持分栏 - 自定义栏数、栏宽、栏距、可选手机版是否保持分栏
- 上传图片自动压缩
- 支持 MP4 视频上传，自动处理文件格式适配主流浏览器
- 支持引用第三方平台视频
- 素材库，储存用户上传过的图片及视频

#### 创建 **Module Template**
- 用户可以使用核心编辑器创建 Module Template，并保存到 `template` 库，编辑文章时直接复制出一个 `template` 实例作为 `module` 开始编辑
- 一篇文章可以使用多个 / 重复使用 `template` ，拼接成一篇文章
- 文章内 `Module` 可以调整顺序

<br/>

### 第三阶段 - CMS
另写文档描述

<br/>

## 竞品资料
### Medium
原版需要付费才能开通作者功能。GitHub 有克隆的[开源编辑器](http://yabwe.github.io/medium-editor/) 
**Features**
- 本身编辑框没有工具条，Highlight 文字之后才出现工具条
- 自带的 styling 工具看[这里](https://github.com/yabwe/medium-editor#all-buttons)
- 有第三方开发者贡献的 **extensions**
- 可以用快捷键设定样式，比如
  ```javascript
  {
    command: 'bold',
    key: 'B',
    meta: true,
    shift: false,
    alt: false
  }
  ```
- 图片支持 drag & drop
- 支持更换编辑器主题
- 可配置 `复制/粘贴` 过滤机制

### 微信公众号编辑器
**Features**
- 可以参考的工具：`首行锁进`, `两端锁进`, `行间距`, `字间距`, `段前/段后距`, `文字背景色`

### [Cargo Collective](https://2.cargocollective.com)
Cargo 是整站自由设计，基本上是我们的终极目标。至于编辑器都是标准的那些东西，除了：
- 分栏
- 插入音频 URL
- 自由涂鸦、插入图形、画曲线

### 秀米
非常「接地气」的产品。特色：
- 悬浮的编辑工具条
- 模块化拼接
- 支持自定义动画（持续时间、延迟、次数、速度）
