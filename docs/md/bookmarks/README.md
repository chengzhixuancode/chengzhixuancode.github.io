# 🔖 文章收藏

收藏平时看到的优秀文章、博客、教程，不定期更新。

<div id="bookmarks-container">
  <div id="bookmarks-filters" class="bookmarks-filters"></div>
  <div id="bookmarks-grid" class="bookmarks-grid"></div>
  <div id="bookmarks-loading" style="text-align: center; padding: 40px; color: #999;">加载中...</div>
  <div id="bookmarks-error" style="display: none; text-align: center; padding: 40px; color: #999;">加载失败，请刷新重试</div>
</div>

---

## 添加新收藏

添加新收藏只需要两步：

1. 编辑 `/data/bookmarks.json` 文件
2. 在数组中添加一个新对象，格式如下：

```json
{
  "title": "文章标题",
  "url": "https://example.com/article",
  "excerpt": "文章摘要或你的点评",
  "category": "分类名称",
  "tags": ["标签1", "标签2"],
  "addedAt": "YYYY-MM-DD",
  "screenshot": ""
}
```

分类会自动提取到筛选按钮，不需要手动维护。

特点：
- ✅ 卡片网格布局，美观清晰
- ✅ 支持按分类筛选查看
- ✅ 响应式设计，适配手机
- ✅ 数据统一存在 JSON 文件，方便版本管理
