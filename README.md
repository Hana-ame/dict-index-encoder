# 词典索引编码器

把单词映射为永久递增的编号，再把编号编码成 a-z 字母；词表跨多次输入永久累积，原文与密文双向联动。数据保存在浏览器本地。

**在线体验：** https://hana-ame.github.io/dict-index-encoder/

## 说明

单文件静态页面，无构建、无依赖、无后端。`index.html` 即全部内容。

## 部署

由 GitHub Actions 自动发布，本地无需任何操作：

- 工作流：`.github/workflows/deploy.yml`
- 触发：推送到 `main`，或在 Actions 页面手动 `Run workflow`
- Pages 发布源：**GitHub Actions**（不使用 `gh-pages` 分支）

更新后推送即可：

```bash
git add -A && git commit -m "your change" && git push origin main
```
