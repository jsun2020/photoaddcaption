# 部署指南

本指南将帮助你将图片字幕生成器部署到 Vercel.com 上。

## 准备工作

1. 确保你有一个 [GitHub](https://github.com) 账号
2. 注册一个 [Vercel](https://vercel.com) 账号（可以使用 GitHub 账号登录）

## 部署步骤

### 方法一：通过 GitHub 部署（推荐）

#### 步骤 1：上传代码到 GitHub

1. 在 GitHub 上创建一个新的仓库（Repository）
2. 将项目文件上传到仓库中，包括：
   - `index.html`
   - `vercel.json`
   - `package.json`
   - `README.md`
   - `.gitignore`

#### 步骤 2：连接 Vercel

1. 访问 [Vercel.com](https://vercel.com)
2. 点击 "Sign Up" 或 "Login"
3. 选择 "Continue with GitHub" 使用 GitHub 账号登录
4. 授权 Vercel 访问你的 GitHub 账号

#### 步骤 3：部署项目

1. 在 Vercel 控制台中，点击 "New Project"
2. 选择 "Import Git Repository"
3. 找到并选择你刚才创建的 GitHub 仓库
4. 点击 "Import"
5. 在配置页面中：
   - **Project Name**: 可以保持默认或自定义
   - **Framework Preset**: 选择 "Other" 或保持默认
   - **Root Directory**: 保持默认（./）
   - **Build and Output Settings**: 保持默认
6. 点击 "Deploy"

#### 步骤 4：等待部署完成

- Vercel 会自动构建和部署你的项目
- 通常需要 1-3 分钟
- 部署完成后，你会看到一个成功页面和你的网站链接

### 方法二：通过 Vercel CLI 部署

#### 步骤 1：安装 Vercel CLI

```bash
npm install -g vercel
```

#### 步骤 2：登录 Vercel

```bash
vercel login
```

#### 步骤 3：部署项目

在项目目录中运行：

```bash
vercel
```

按照提示完成配置：
- 选择账号
- 确认项目名称
- 确认部署设置

## 部署后的操作

### 获取网站链接

部署完成后，Vercel 会提供几个链接：
- **Production URL**: 你的正式网站地址（如：`https://your-project.vercel.app`）
- **Preview URLs**: 预览地址

### 自定义域名（可选）

1. 在 Vercel 控制台中选择你的项目
2. 进入 "Settings" → "Domains"
3. 添加你的自定义域名
4. 按照提示配置 DNS 记录

### 更新网站

当你需要更新网站时：

**方法一（GitHub 部署）**：
- 直接更新 GitHub 仓库中的文件
- Vercel 会自动检测变更并重新部署

**方法二（CLI 部署）**：
- 在项目目录中运行 `vercel --prod`

## 故障排除

### 常见问题

1. **部署失败**
   - 检查 `vercel.json` 文件格式是否正确
   - 确保 `index.html` 文件存在

2. **网站无法访问**
   - 等待几分钟，DNS 传播需要时间
   - 检查 Vercel 控制台中的部署状态

3. **功能异常**
   - 检查浏览器控制台是否有错误信息
   - 确保所有文件都已正确上传

### 获取帮助

- [Vercel 官方文档](https://vercel.com/docs)
- [Vercel 社区论坛](https://github.com/vercel/vercel/discussions)

## 分享给朋友

部署完成后，你可以将生成的网站链接分享给朋友：

```
https://your-project-name.vercel.app
```

你的朋友可以直接访问这个链接使用图片字幕生成器，无需安装任何软件！

---

祝你部署顺利！如有问题，欢迎查阅相关文档或寻求帮助。