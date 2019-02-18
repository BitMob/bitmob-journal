# BitMob Blog CMS

(TBD)

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

## 其他
- 文章列表默认按发布时间逆序
- 支持手动排序