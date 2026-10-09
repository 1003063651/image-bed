# image-bed

个人图床：GitHub 仓库 + jsDelivr CDN。

## 图片地址格式

```
https://cdn.jsdelivr.net/gh/1003063651/image-bed@main/<仓库里的路径>
```

例如：

```
https://cdn.jsdelivr.net/gh/1003063651/image-bed@main/images/2026/10/xxx.png
```

在 Markdown 里引用：

```markdown
![](https://cdn.jsdelivr.net/gh/1003063651/image-bed@main/images/2026/10/xxx.png)
```

## 上传图片

### 方法一：网页拖拽（最简单）

1. 打开 https://github.com/1003063651/image-bed
2. 进入 `images/` 目录（建议按 `年/月` 存放，如 `images/2026/10/`）
3. 点 **Add file** → **Upload files**，把图片拖进去，点 **Commit changes**

### 方法二：PicGo（桌面端，截图/拖拽自动上传并复制链接）

PicGo → 图床设置 → GitHub：

| 配置项 | 值 |
|---|---|
| 仓库名 | `1003063651/image-bed` |
| 分支名 | `main` |
| Token | 在 https://github.com/settings/tokens 新建 classic token，勾选 `repo` 权限 |
| 存储路径 | `images/{y}/{m}/` |
| 自定义域名 | `https://cdn.jsdelivr.net/gh/1003063651/image-bed@main` |

设置好后截图 / 拖图片到 PicGo 即自动上传，Markdown 链接自动复制到剪贴板。

## 注意事项

- 仓库是公开的，传到这里的图片任何人都可以通过链接访问，不要传私密图片。
- 单个文件不超过 50MB（jsDelivr 限制）。
- 刚上传的图片 CDN 可能需要几十秒到几分钟生效。
