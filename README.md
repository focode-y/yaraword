# yara-agency-html-site 交付说明

这是一个纯静态网站项目（`index.html + styles.css + content.js`）。

## 目录结构

```text
yara-agency-html-site/
├─ index.html
├─ styles.css
├─ content.js
├─ assets/
│  ├─ videos/
│  ├─ fonts/
│  └─ images/
└─ README.md
```

## 你最常改的文件

1. `content.js`：改页面文案、多语言内容、案例卡片文案。
2. `styles.css`：改样式和布局。
3. `index.html`：改结构、联系方式、页面基础配置。

## 重点：案例图片路径

案例图片已统一放在：`assets/images/`

当前使用：
- `./assets/images/li1.png`
- `./assets/images/li2.png`
- `./assets/images/li3.png`

如果要换图：
- 直接替换同名文件，最省事；或
- 在 `content.js` 的 `cases` 字段中改图片路径。

## 本地预览

执行路径：`D:\Business\WebProjects\yara-agency-html-site`

```powershell
python -m http.server 8080
```

浏览器打开：`http://localhost:8080`

## 交付建议（安全）

只交付业务文件：
- `index.html`
- `styles.css`
- `content.js`
- `assets/`

不要交付本地缓存目录（例如 `.wrangler/`）。
