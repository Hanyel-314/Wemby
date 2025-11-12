# Victor Wembanyama 个人网页

这是一个关于NBA球星 Victor Wembanyama 的现代化、响应式个人网页项目。

## 项目简介

这个项目展示了圣安东尼奥马刺队新秀 Victor Wembanyama 的个人信息、职业数据、成就和精彩瞬间。网站采用现代化设计，具有流畅的动画效果和完全响应式布局。

## 主要特性

### 🎨 设计特点
- **现代化界面**：采用黑色、白色和橙色的配色方案
- **响应式设计**：完美适配桌面、平板和移动设备
- **流畅动画**：页面滚动和元素交互都带有精美的动画效果
- **视觉层次**：清晰的信息架构和视觉引导

### 📱 页面结构

1. **首页英雄区域**
   - 大标题展示
   - 关键统计数据（身高、选秀顺位、球衣号码）
   - 滚动指示器

2. **关于部分**
   - 个人简介
   - 出生信息
   - 身体数据（身高、体重、臂展）
   - 职业背景

3. **数据统计**
   - 场均得分
   - 场均篮板
   - 场均盖帽
   - 投篮命中率
   - 场均助攻
   - 场均上场时间

4. **荣誉成就**
   - 时间线展示
   - 从早期到现在的各项荣誉

5. **精彩瞬间**
   - 职业生涯重要时刻展示

### ⚡ 技术特性

- **原生技术栈**：HTML5 + CSS3 + JavaScript
- **无依赖**：不需要任何外部库或框架
- **性能优化**：
  - 懒加载支持
  - 防抖优化
  - 交叉观察者API
  - 平滑滚动
- **辅助功能**：
  - 键盘导航支持
  - 语义化HTML
  - 移动端触摸优化

### 🎯 交互功能

- 响应式导航菜单（移动端汉堡菜单）
- 平滑滚动到各个部分
- 数据卡片的动态数字计数动画
- 滚动时的导航栏效果
- 时间线项目的淡入动画
- 卡片悬停效果
- 视差滚动效果

## 文件结构

```
Wemby/
│
├── index.html          # 主HTML文件
├── styles.css          # 样式表
├── script.js           # JavaScript交互脚本
├── README.md           # 项目说明文档
└── images/             # 图片文件夹
    └── IMAGE_GUIDE.md  # 图片使用指南
```

## 📸 添加图片

网站已经预留了5个图片位置，需要你添加 Victor Wembanyama 的照片：

1. **wembanyama-profile.jpg** - 个人肖像照（关于部分）
2. **wembanyama-draft.jpg** - 选秀之夜照片
3. **wembanyama-debut.jpg** - NBA首秀照片
4. **wembanyama-scoring.jpg** - 得分瞬间照片
5. **wembanyama-defense.jpg** - 防守瞬间照片

### 快速添加图片

1. 准备5张 Victor Wembanyama 的照片
2. 按照上述文件名重命名
3. 将它们放入 `images/` 文件夹
4. 刷新浏览器查看效果

📖 **详细说明：** 查看 `images/IMAGE_GUIDE.md` 获取完整的图片要求和指南

⚠️ **注意：** 即使没有添加图片，网站也能正常显示（会显示占位符）

## 快速开始

### 本地运行

1. 克隆或下载项目到本地
2. 使用浏览器直接打开 `index.html` 文件

或者使用本地服务器：

```bash
# 使用 Python 3
python -m http.server 8000

# 使用 Python 2
python -m SimpleHTTPServer 8000

# 使用 Node.js (需要安装 http-server)
npx http-server
```

然后在浏览器中访问 `http://localhost:8000`

### 使用 Live Server (推荐)

如果你使用 VS Code，可以安装 "Live Server" 扩展：
1. 在 VS Code 中打开项目文件夹
2. 右键点击 `index.html`
3. 选择 "Open with Live Server"

## 浏览器兼容性

- ✅ Chrome (推荐)
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ 移动浏览器

## 自定义修改

### 修改颜色主题

在 `styles.css` 文件的开头找到 CSS 变量：

```css
:root {
    --primary-color: #000000;      /* 主色调 */
    --secondary-color: #c4c4c4;    /* 次要色 */
    --accent-color: #ff6b35;       /* 强调色 */
    --text-light: #ffffff;         /* 浅色文字 */
    --text-dark: #333333;          /* 深色文字 */
    --bg-light: #f8f9fa;          /* 浅色背景 */
}
```

### 更新统计数据

在 `index.html` 文件中找到对应的 `data-target` 属性并修改数值：

```html
<div class="stat-value" data-target="21.4">0</div>
```

### 添加真实图片

将图片文件放入项目文件夹，然后在 HTML 中替换占位符：

```html
<!-- 原始占位符 -->
<div class="image-placeholder">...</div>

<!-- 替换为真实图片 -->
<img src="your-image.jpg" alt="Victor Wembanyama">
```

## 性能优化建议

1. **图片优化**：使用 WebP 格式以减小文件大小
2. **CDN 部署**：将静态资源部署到 CDN
3. **压缩代码**：在生产环境中压缩 CSS 和 JS
4. **缓存策略**：配置适当的浏览器缓存

## 部署

### GitHub Pages

1. 将代码推送到 GitHub 仓库
2. 进入仓库的 Settings > Pages
3. 选择分支并保存
4. 访问 `https://your-username.github.io/repository-name`

### Netlify

1. 注册 Netlify 账号
2. 拖拽项目文件夹到 Netlify
3. 网站自动部署完成

### Vercel

```bash
npm i -g vercel
vercel
```

## 未来改进计划

- [ ] 添加真实的球员照片和视频
- [ ] 集成实时数据API
- [ ] 添加多语言支持
- [ ] 添加暗黑模式切换
- [ ] 集成社交媒体动态
- [ ] 添加互动式统计图表
- [ ] 性能进一步优化

## 数据来源

本项目中的统计数据基于 2023-24 NBA 赛季。实际数据可能会有所不同，请访问 NBA 官方网站获取最新信息。

## 免责声明

这是一个演示项目，仅用于学习和展示目的。所有关于 Victor Wembanyama 的信息均为公开信息。本项目与 NBA、圣安东尼奥马刺队或 Victor Wembanyama 本人无任何官方关联。

## 许可证

本项目仅供学习和个人使用。

## 联系方式

如有问题或建议，欢迎提交 Issue 或 Pull Request。

---

**享受探索 Wemby 的世界！** 🏀
