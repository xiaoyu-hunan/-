# 部署指南

## GitHub Pages 部署

### 1. Fork 项目
1. 访问 [项目页面](https://github.com/your-username/pharma-safety-notes)
2. 点击右上角的 "Fork" 按钮
3. 选择你的 GitHub 账户

### 2. 启用 GitHub Pages
1. 进入你的 Fork 项目页面
2. 点击 "Settings" 标签
3. 在左侧菜单中找到 "Pages"
4. 在 "Source" 部分选择 "Deploy from a branch"
5. 选择 "main" 分支和 "/ (root)" 文件夹
6. 点击 "Save"

### 3. 自定义域名（可选）
1. 在项目根目录创建 `CNAME` 文件
2. 添加你的域名（例如：`pharma-safety.yourdomain.com`）
3. 在域名服务商处配置 CNAME 记录指向 `your-username.github.io`

### 4. 访问网站
- 默认地址：`https://your-username.github.io/pharma-safety-notes`
- 自定义域名：`https://your-domain.com`

## 本地开发

### 环境要求
- Python 3.6+ 或 Node.js 12+ 或 PHP 7.4+

### 启动本地服务器

#### 使用 Python
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

#### 使用 Node.js
```bash
# 安装 http-server
npm install -g http-server

# 启动服务器
http-server -p 8000
```

#### 使用 PHP
```bash
php -S localhost:8000
```

### 访问本地网站
打开浏览器访问 `http://localhost:8000`

## 内容更新

### 添加新内容
1. 在相应的 `content/` 子目录中创建新的 Markdown 文件
2. 按照现有文件的格式编写内容
3. 提交更改并推送到 GitHub

### 修改现有内容
1. 编辑相应的 Markdown 文件
2. 提交更改并推送到 GitHub
3. GitHub Pages 会自动重新部署

### 更新图片
1. 将图片文件放在 `assets/images/` 目录中
2. 在 Markdown 文件中使用相对路径引用图片
3. 提交更改并推送到 GitHub

## 自定义配置

### 修改网站信息
1. 编辑 `index.html` 中的标题和描述
2. 修改 `README.md` 中的项目信息
3. 更新 `_config.yml` 中的配置（如果使用 Jekyll）

### 添加新功能
1. 在 `assets/js/` 中添加新的 JavaScript 文件
2. 在 `assets/css/` 中添加新的样式文件
3. 在 HTML 文件中引用新文件

### 修改样式
1. 编辑 `assets/css/style.css` 修改主样式
2. 编辑 `assets/css/responsive.css` 修改响应式样式
3. 提交更改并推送到 GitHub

## 故障排除

### 常见问题

#### 1. 网站无法访问
- 检查 GitHub Pages 是否已启用
- 确认分支和文件夹设置正确
- 等待几分钟让 GitHub Pages 完成部署

#### 2. 图片无法显示
- 检查图片文件路径是否正确
- 确认图片文件已提交到 GitHub
- 检查图片文件格式是否支持

#### 3. 样式不生效
- 检查 CSS 文件路径是否正确
- 确认 CSS 文件已提交到 GitHub
- 清除浏览器缓存

#### 4. JavaScript 功能不工作
- 检查 JavaScript 文件路径是否正确
- 确认 JavaScript 文件已提交到 GitHub
- 检查浏览器控制台是否有错误信息

### 调试技巧
1. 使用浏览器开发者工具检查网络请求
2. 查看浏览器控制台的错误信息
3. 检查 GitHub Pages 的构建日志
4. 使用在线工具验证 HTML 和 CSS

## 性能优化

### 图片优化
- 使用 WebP 格式图片
- 压缩图片文件大小
- 提供多种尺寸的图片

### 代码优化
- 压缩 CSS 和 JavaScript 文件
- 使用 CDN 加速资源加载
- 启用浏览器缓存

### 内容优化
- 优化页面标题和描述
- 使用语义化 HTML 标签
- 添加结构化数据

## 安全考虑

### HTTPS
- GitHub Pages 默认使用 HTTPS
- 确保所有资源都使用 HTTPS 链接

### 内容安全
- 避免在代码中硬编码敏感信息
- 定期更新依赖项
- 使用安全的第三方服务

## 备份和恢复

### 备份策略
- 定期备份项目文件
- 使用 Git 版本控制
- 保存重要的配置文件

### 恢复步骤
1. 从 GitHub 克隆项目
2. 恢复配置文件
3. 重新部署到 GitHub Pages

## 监控和维护

### 网站监控
- 使用 Google Analytics 监控访问量
- 设置 Uptime Robot 监控网站可用性
- 定期检查网站性能

### 内容维护
- 定期更新内容
- 检查链接有效性
- 更新过时信息

### 技术维护
- 定期更新依赖项
- 检查安全漏洞
- 优化网站性能

## 支持和帮助

### 获取帮助
- 查看 GitHub Issues
- 阅读项目文档
- 联系项目维护者

### 贡献代码
- Fork 项目
- 创建功能分支
- 提交 Pull Request

### 报告问题
- 使用 GitHub Issues 报告问题
- 提供详细的错误信息
- 包含复现步骤

---

**注意**：本部署指南基于 GitHub Pages 服务。如果使用其他托管服务，请参考相应的文档。
