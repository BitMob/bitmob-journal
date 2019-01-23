# BitMob 通用 CMS 文章编辑器

## 基础字段
- `_id: ''`
- `createdAt`
- `updatedAt`
- 标题 `title: { zh: '', en: '' }`
- url 标识 `slug: ''`
- 分类标签 `tags: ['']`
- 是否发布 `isPublished: true`
- 正文内容 `content: { zh: '', en: '' }`

## 扩展字段
- 自定义封面图 `cover: {desk: 'http://bitmob.cc/imgUrl.jpg', mobile: ''}`
- 自定义微信转发信息，不填则由前端自动选择相关信息
  ```
  {
    imgUrl: 'http://bitmob.cc/imgUrl.jpg',
    title: '转发给朋友的标题'
    desc: '转发给朋友在标题下显示的文字',
    timeline: '转发到朋友圈的文字'
  }
  ```

## 富文本编辑框
- 过滤粘贴过来的 `html`, `XML` 字符
- 自定义或引用实际页面排版样式/字体，做到「所见即所得」
- 支持富文本编辑状态，以及 `markdown` 编辑状态
- 保存后接口返回 `markdown` 字符串
- Markdown 语法可扩展，参考 [Khan Simple Markdown](https://github.com/Khan/simple-markdown)

## 样式控件
- 六级标题，即 `#` `##` `###` `####` `#####` `######`
- 文字**加粗**，即 `**text**`
- 文字链接，即 `[我是链接](http://google.com)`
- 插入图片，即 `![alt text](https://abc.com/images/icons/favicon-16x16.png)`
- 有序 / 无序列表，即 `1. a` / `- a`
- 扩展 1: 文字对齐 `>>居中<<` `>>右对齐>>` `<<两边对齐>>` 

## 其他
- 文章列表默认按发布时间逆序
- 支持手动排序