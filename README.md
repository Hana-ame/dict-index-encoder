# 词典编号编码器 · 中文码表 2 万字

把单词映射为永久递增的编号，再按数字 / 字母 / 中文三种模式编码；词表跨多次输入永久累积，支持打乱，原文与密文双向联动。数据保存在浏览器本地。

- **数字模式**：编号直接输出为数字串
- **字母模式**：编号编码为 a-z 字母（1→a、26→z、27→aa…）
- **中文模式**：内置 20992 字汉字码表（CJK 基本区 U+4E00–U+9FFF），一个汉字对应一个密文字符

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
