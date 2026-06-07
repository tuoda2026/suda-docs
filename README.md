# 速搭文档站点

本仓库仅包含速搭（Suda）产品的说明文档，通过 GitHub Pages 自动部署为在线文档网站。

## 在线访问地址

部署成功后可通过以下地址访问：

```
https://tuoda2026.github.io/suda-docs
```

## 本地预览

```bash
# 安装依赖
pip install mkdocs-material

# 启动本地预览
mkdocs serve

# 访问 http://127.0.0.1:8000
```

## 如何推送并部署

1. 在 GitHub 上创建新仓库，命名为 `suda-docs`
2. 将本文件夹推送到该仓库：

```bash
cd suda-docs
git init
git add .
git commit -m "init docs site"
git branch -M main
git remote add origin https://github.com/tuoda2026/suda-docs.git
git push -u origin main
```

3. 打开 GitHub 仓库页面 → **Settings** → **Pages**
4. **Build and deployment** → Source 选择 **GitHub Actions**
5. 等待 Actions 运行完成，即可通过上述地址访问

## 绑定自定义域名（可选）

1. 在 `docs/` 目录下创建 `CNAME` 文件，写入你的域名（如 `docs.yourdomain.com`）
2. 域名解析添加 CNAME 记录指向 `tuoda2026.github.io`
3. 在 GitHub Pages 设置中填入自定义域名并开启 HTTPS
