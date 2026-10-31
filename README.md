# 312 记忆卡

四组心理学 312 记忆卡，共 409 张。单页应用，无外部依赖，可离线使用。

## 部署到 GitHub Pages

1. 新建仓库，选 **Public**
2. 上传本目录全部文件（含 `icons/` 文件夹）
3. Settings → Pages → Source 选 **Deploy from a branch** → `main` / `/ (root)` → Save
4. 等 1–2 分钟，访问 `https://<用户名>.github.io/<仓库名>/`

## 手机安装

- iPhone：Safari 打开 → 分享 → 添加到主屏幕
- 安卓：Chrome 打开 → ⋮ → 安装应用

首次打开必须联网，等首页加载完成，离线缓存才会写入。之后断网可用。

## 更新内容

改动任何卡片文件后，**必须同时修改 `sw.js` 第一行的缓存版本号**：

```js
const CACHE = 'memcard-312-v2';   // v1 → v2
```

否则浏览器会继续用旧缓存。

## 数据

- 进度存在浏览器 localStorage，按域名隔离
- 换域名、清缓存、换设备都会丢
- 备份：各卡组「卡片库 → ⤒」导出 JSON

## 文件

| 文件 | 说明 |
|---|---|
| `index.html` | 总入口 |
| `measure-1.html` | 测量与统计 162 张 |
| `measure-2.html` | 测量统计 2 · 79 张 |
| `dev-edu.html` | 发展教育 85 张 |
| `general.html` | 普心 83 张 |
| `framework.html` | 空白模板 |
| `sw.js` | 离线缓存 |
| `manifest.webmanifest` | 应用信息 |
