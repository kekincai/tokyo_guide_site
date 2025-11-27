# Kanto Guide Notes  
**关东沿线 · 车站周边 · 居住与出行攻略示例网站**

本项目用于整理关东地区主要车站周边的居住体验、生活机能、通勤线路参考等攻略内容，  
通过 GitHub Pages 展示为轻量级静态网站。

本站不包含个人信息，所有内容均以“站点攻略 / 城市体验”为主，侧重普通生活参考。

---

## 📌 项目目标（Project Goals）

- 为 **关东地区沿线居住者 / 租房者** 提供可读性强的攻略页面  
- 针对各个车站整理：  
  - 生活圈与环境  
  - 通勤路线与换乘便利性  
  - 一日踩点路线示例  
  - 购房 / 租房时可参考的周边信息  
- 网站结构清晰，可持续扩展为：  
  - 多站点  
  - 多线路  
  - 多主题（如消费记录、通勤比较等）

---

## 🗂 文件结构（Folder Structure）

```
tokyo_guide_site/
├── index.html                 # 首页：导航与全站入口
├── trips/
│   └── soka-room-hunting.html # 示例：草加站攻略，可替换为自定义内容
└── assets/
    └── css/
        └── main.css           # 全站通用样式
```

说明：

- `index.html`  
  网站首页，用于展示各攻略入口。样式轻量、可扩展更多卡片。
- `trips/`  
  放置每一个站点 / 区域的攻略网页，例如：  
  - `soka-room-hunting.html`  
  - `kasukabe-area-guide.html`  
  - `north-chiba-hunting.html`
- `assets/css/main.css`  
  全站通用样式，可根据需要修改或增加页面级样式。

---

## 🌐 部署（Deployment）

项目基于 **GitHub Pages**：

1. 将整个目录推送到仓库根目录  
2. 打开 GitHub 项目  
3. 进入 *Settings → Pages*  
4. Source 选择：  
   - Branch：`main`  
   - Folder：`/ (root)`  
5. 保存后稍等片刻，即可通过 Pages 访问本站

部署完成后网站地址一般为：

```
https://<your-github-username>.github.io/<your-repo-name>/
```

---

## ➕ 如何扩展（Adding New Guides）

你可以按以下方式扩展站点内容：

### 1. 添加新攻略页面
在 `trips/` 中新增 HTML 文件，例如：

```
trips/kasukabe-area-guide.html
trips/kitakasukabe-life-guide.html
```

### 2. 修改首页入口
在 `index.html` 中复制「卡片」结构：

```html
<div class="card">
  <div class="card-type">AREA · ROOM HUNTING</div>
  <div class="card-title">春日部站周边 · 生活机能与看房参考</div>
  <div class="card-desc">
    <!-- 描述文字 -->
  </div>
  <div class="card-link">
    <a href="trips/kasukabe-area-guide.html">打开攻略 →</a>
  </div>
</div>
```

即可实现一个新的攻略入口。

---

## 🧩 自定义样式（Customization）

所有页面默认使用：

```
<link rel="stylesheet" href="assets/css/main.css" />
```

如需增加页面专属样式，可在对应页面添加：

```html
<style>
  /* custom css here */
</style>
```

---

## 📄 许可协议（License）

本仓库用于站点结构示例及攻略内容整理，不包含专有代码。  
内容可根据需要自由修改与再使用（MIT License）。

---

## 🙌 致谢（Thanks）

- GitHub Pages 提供静态网站托管  
- 所有外部地图地址来自公开的 Google Maps/My Maps  
