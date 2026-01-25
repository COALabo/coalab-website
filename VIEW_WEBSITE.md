# COALAB 网站查看指南

## 当前状态
GitHub Pages 功能尚未启用，因此 `https://peter-awe.github.io/coalab-website` 暂时无法访问。

## 解决方案

### 方案一：立即启用 GitHub Pages（推荐）
**您需要手动启用 GitHub Pages：**

1. **打开仓库设置页面**：
   - 访问：`https://github.com/Peter-awe/coalab-website/settings/pages`

2. **配置 GitHub Pages**：
   - 在 "Build and deployment" 部分
   - "Source"：选择 "Deploy from a branch"
   - "Branch"：选择 "main" 和 "/ (root)"
   - 点击 "Save"

3. **等待构建**：
   - 启用后，等待 1-2 分钟
   - 访问：`https://peter-awe.github.io/coalab-website`

### 方案二：导师本地查看（立即可用）

#### 方法 A：使用 Docker（最简单，无需安装 Ruby）
```bash
# 1. 克隆仓库
git clone https://github.com/Peter-awe/coalab-website.git
cd coalab-website

# 2. 使用 Docker 运行网站
docker run --rm -it -v "$PWD:/srv/jekyll" -p 4000:4000 jekyll/jekyll:4.2.2 jekyll serve

# 3. 在浏览器中打开
# 访问 http://localhost:4000
```

#### 方法 B：本地安装 Jekyll
```bash
# 1. 克隆仓库
git clone https://github.com/Peter-awe/coalab-website.git
cd coalab-website

# 2. 安装 Ruby 和 Bundler（如果尚未安装）
# macOS: brew install ruby
# Ubuntu: sudo apt install ruby ruby-dev
# Windows: 安装 RubyInstaller

# 3. 安装依赖
gem install bundler
bundle install

# 4. 运行网站
bundle exec jekyll serve

# 5. 访问 http://localhost:4000
```

#### 方法 C：查看静态文件
网站已经构建好，可以直接查看静态文件：
1. 克隆仓库后，打开 `_site` 目录
2. 用浏览器直接打开 `_site/index.html`

### 方案三：使用在线预览服务
1. 访问：`https://htmlpreview.github.io/`
2. 输入：`https://raw.githubusercontent.com/Peter-awe/coalab-website/main/index.html`
3. 注意：此方法可能无法正确加载 CSS 和图片

## 网站内容概览
- **首页**：实验室介绍、研究亮点、特色项目、最新新闻
- **研究**：语言障碍、发育神经科学、人工智能三个研究方向
- **项目**：当前和已完成的研究项目
- **出版物**：按年份排列的学术论文
- **团队**：实验室成员介绍
- **新闻**：实验室动态和事件
- **联系**：联系信息和加入机会

## 故障排除

### GitHub Pages 启用后仍无法访问
1. 检查 Actions 页面：`https://github.com/Peter-awe/coalab-website/actions`
2. 确保构建成功（绿色勾号）
3. 等待 DNS 传播（最多 10 分钟）

### 本地运行问题
```bash
# 清理并重新构建
bundle exec jekyll clean
bundle exec jekyll build
bundle exec jekyll serve
```

## 联系方式
如有技术问题，请联系网站开发者。

**启用 GitHub Pages 后，网站将永久在线访问！**
