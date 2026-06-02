# Ogden Basic English 850

一个静态版 Ogden Basic English 850 词学习手册，可直接本地打开，也可部署到任意静态服务器。

## 本地使用

直接双击 `index.html` 即可打开页面。

如果希望测试 PWA、Service Worker 或更接近线上部署环境，可以在当前目录运行：

```bash
python3 -m http.server 8000
```

然后访问：

```text
http://localhost:8000
```

## 部署

把整个目录上传到静态站点服务即可，例如 Nginx、Apache、Vercel、Netlify、Cloudflare Pages 或任意对象存储静态托管。

需要一起部署的文件：

- `index.html`
- `manifest.json`
- `sw.js`
- `favicon.png`
- `icons/`

页面是纯静态实现，没有必需后端。发音会优先尝试 `/api/tts`，如果部署环境没有该接口，会自动回退到 Google TTS。
