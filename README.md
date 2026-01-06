# 手工制作类APP原型设计

> **最新版本：v2.0** - UI设计全面升级
> 从单调灰色系统升级为现代多彩设计体系，完全符合iOS HIG设计规范

## 更新日志

### v2.0 (2024年最新)
**UI设计全面升级** ✨

- 🎨 **色彩系统升级**：从单一灰色系→现代6色分类系统
  - 主色：活力红#FF6B6B（CTA操作）
  - 次色：清爽青绿#4ECDC4（次要操作）
  - 分类色：6种彩色渐变系统

- 🎯 **所有页面优化**：
  - 首页：彩色分类卡片 + 渐变活动卡片 + 渐变按钮
  - 搜索页：圆形搜索框 + 2xl圆角卡片 + hover效果
  - 详情页：粘性导航 + 渐变按钮组 + badge指示器
  - 工作台：彩色icon卡片 + 彩色进度条 + 交互动画
  - 个人页：动态渐变头部 + 彩色stat卡片 + 装饰元素

- ✨ **交互体验升级**：
  - 玻璃效果导航栏（毛玻璃模糊）
  - 缩放+阴影提升的hover效果
  - 彩色圆点导航指示器
  - 平滑的iOS风格过渡动画

- 🔧 **设计规范完善**：
  - CSS变量化色彩系统
  - 详细的间距/圆角/阴影规范
  - iOS缓动曲线标准化

### v1.0 (初始版本)
- 基础功能框架设计
- 单色灰度系统
- 简单的页面布局

## 产品功能分析

### 核心功能模块

1. **首页**
   - 顶部导航栏：好友、合集、推荐、社区、资讯等
   - 分类浏览：布艺、木工、纸艺、饰品、高达等分类（横向滚动卡片）
   - 活动卡片：投票、活动等
   - 内容流：帖子列表展示，包含用户信息、图片、互动数据

2. **搜索功能**
   - 支持搜索高达模型内容
   - 搜索结果列表展示
   - 快速查看详情

3. **内容详情页**
   - 高达模型图片展示
   - 板件取件表：显示各板件信息、零件数、颜色、取件状态

4. **工作台**
   - 项目管理：创建和管理手工项目
   - 图片管理：上传和管理参考图片
   - 进度跟踪：记录制作进度和里程碑
   - 最近项目列表：显示项目进度条

5. **我的页面**
   - 个人信息展示
   - 数据统计：作品数、收藏数、项目数
   - 我的作品集
   - 我的收藏
   - 设置功能
   - 最近作品展示

## 设计规范

### 色彩系统（已升级为现代多彩系统）
- **主色**：活力红 (#FF6B6B) - 用于CTA按钮、首页导航、强调操作
- **次色**：清爽青绿 (#4ECDC4) - 用于工作台导航、次要操作
- **强调色**：温暖金色 (#FFD93D) - 用于特殊提示和标签
- **分类色系**（6种彩色渐变）：
  - 布艺：粉红渐变 (#FFC0CB → #FFB6C1)
  - 木工：琥珀渐变 (#FFB347 → #FFA500)
  - 纸艺：紫色渐变 (#DA70D6 → #DA70D6)
  - 饰品：青色渐变 (#20B2AA → #5F9EA0)
  - 高达：橙色渐变 (#FF8C00 → #FF7F50)
  - 全部：灰色渐变 (#D3D3D3 → #C0C0C0)

### 背景与中性色
- 背景：#FAFBFC（浅蓝灰）
- 卡片：#FFFFFF（纯白）
- 分割线：#E5E8EB（浅灰）
- 文字主：#0F1419（深色）
- 文字次：#626B73（中灰）
- 文字辅：#8B95A0（浅灰）

### 视觉元素
- **圆角**：12px（按钮/输入框）、16px（卡片）、20px（2xl大圆角）
- **阴影**：
  - 浅阴影(sm)：`0 2px 8px rgba(15,20,25,0.06)`
  - 中阴影(md)：`0 4px 12px rgba(15,20,25,0.1)`
  - 深阴影(lg)：`0 8px 24px rgba(15,20,25,0.12)`
- **渐变**：135deg线性渐变，用于卡片、按钮、进度条
- **玻璃效果**：10px模糊+白色半透明背景，用于导航栏

### 交互动画
- **过渡曲线**：`cubic-bezier(0.4, 0, 0.2, 1)`（iOS标准缓动）
- **Hover效果**：缩放(scale-102) + 阴影提升
- **按压反馈**：缩放(scale-0.96)
- **Icon动画**：横向平移(translate-x-1)
- **过渡时间**：0.3s（快速、流畅）

### 字体
- **系统字体栈**：`-apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif`
- **字重**：
  - 标题：Bold (700) / Semibold (600)
  - 正文：Medium (500) / Regular (400)
- **大小**：
  - 大标题：20-24px
  - 小标题：16-18px
  - 正文：14px
  - 小字：12-13px

### 栅格与间距
- **屏幕宽度**：393px（iPhone 14 Pro）
- **屏幕高度**：852px
- **内边距**：16px（页面左右）、12px（卡片内部）
- **间距**：4px、8px、12px、16px、24px（递进关系）
- **行高**：1.5倍（文字易读性）

## 文件说明

### HTML版本（推荐用于预览和演示）

- `index.html` - 主入口，使用iframe展示所有页面
- `home.html` - 首页原型
- `search.html` - 搜索列表页原型
- `detail.html` - 内容详情页原型
- `workspace.html` - 工作台页面原型
- `profile.html` - 我的页面原型
- `styles.css` - 自定义样式文件

### SVG版本（用于Figma编辑）

- `home.svg` - 首页原型
- `search.svg` - 搜索列表页原型
- `detail.svg` - 内容详情页原型
- `workspace.svg` - 工作台页面原型
- `profile.svg` - 我的页面原型

## 使用方法

### HTML版本
1. **直接在浏览器中打开** `index.html` 查看所有页面
   - 所有页面以iframe网格展示
   - 支持响应式缩放

2. **或单独打开各个HTML文件进行预览**
   - `home.html` - 首页
   - `search.html` - 搜索页
   - `detail.html` - 详情页
   - `workspace.html` - 工作台
   - `profile.html` - 个人页

3. **技术说明**
   - 所有页面使用Tailwind CSS CDN（无需本地安装）
   - FontAwesome 6.4.0图标库
   - 图片来自Unsplash API（动态加载）
   - 完全本地运行，无需后端服务

### SVG版本
1. **直接在浏览器中打开SVG文件进行预览**
2. **将SVG文件拖入Figma进行编辑**
3. **在Figma中按 `<g>` 组的ID进行分层编辑**

## 自定义指南

### 修改色彩系统
编辑 `styles.css` 中的CSS变量：

```css
:root {
  --color-primary: #FF6B6B;        /* 主色 */
  --color-secondary: #4ECDC4;      /* 次色 */
  --color-tertiary: #FFD93D;       /* 强调色 */
  /* ... 其他颜色 */
}
```

### 修改渐变色
各页面使用的渐变：

```html
<!-- 红粉渐变（主要CTA） -->
<div class="bg-gradient-to-r from-red-500 to-pink-500"></div>

<!-- 青绿渐变（次要操作） -->
<div class="bg-gradient-to-r from-cyan-500 to-teal-500"></div>

<!-- 琥珀橙渐变（木工类） -->
<div class="bg-gradient-to-r from-amber-500 to-orange-500"></div>
```

### 修改分类色系
编辑 `home.html` 中的分类卡片：

```html
<!-- 布艺 - 粉红 -->
<div class="bg-gradient-to-br from-pink-200 to-pink-100">

<!-- 木工 - 琥珀 -->
<div class="bg-gradient-to-br from-amber-200 to-amber-100">

<!-- 纸艺 - 紫色 -->
<div class="bg-gradient-to-br from-purple-200 to-purple-100">
```

### 修改间距与圆角
使用Tailwind类名：
- `rounded-xl` = 12px（按钮）
- `rounded-2xl` = 16px（卡片）
- `p-4` = 16px内边距
- `gap-3` = 12px间距
- `py-3` = 12px上下边距

### 修改按钮样式
```html
<!-- 渐变主按钮 -->
<button class="bg-gradient-to-r from-red-500 to-pink-500 text-white shadow-md hover:shadow-lg">

<!-- 白色次按钮 -->
<button class="bg-white text-gray-700 hover:bg-gray-50">
```

## 关键特性

### 🎨 设计系统
- ✅ **现代色彩系统**：6种主题色 + 12种辅助色
- ✅ **完整的视觉层次**：字号、权重、间距有机统一
- ✅ **iOS HIG规范**：圆角、阴影、过渡曲线完全符合
- ✅ **品牌一致性**：所有页面视觉风格统一
- ✅ **可访问性**：足够的色彩对比度和文字可读性

### ⚡ 交互体验
- ✅ **丰富的微交互**：缩放、阴影、颜色变化反馈
- ✅ **平滑的动画**：所有过渡使用iOS缓动曲线
- ✅ **视觉反馈**：按钮、链接、卡片都有hover状态
- ✅ **玻璃效果**：导航栏使用毛玻璃模糊效果
- ✅ **色彩指示器**：导航栏用彩色圆点指示当前页面

### 🛠️ 开发友好
- ✅ **完全CDN部署**：无需本地构建，直接浏览器打开
- ✅ **模块化代码**：每个页面独立，易于修改
- ✅ **CSS变量化**：修改色彩只需改一处
- ✅ **Tailwind CSS**：快速复用，易于定制
- ✅ **无依赖库**：仅使用标准库和CDN资源

### 📱 适配与性能
- ✅ **iPhone 14 Pro适配**：393×852精确设计
- ✅ **轻量级资源**：无本地图片，全部来自Unsplash CDN
- ✅ **快速加载**：CDN加速，毫秒级渲染
- ✅ **高效图标**：FontAwesome矢量图标
- ✅ **响应式设计**：支持各种屏幕尺寸

## 对标产品参考
本设计参考了以下优秀产品的设计模式：
- **小红书**：社区内容流、卡片设计、分类系统
- **得物**：彩色分类、渐变设计、交互反馈
- **抖音**：简洁导航、沉浸式内容、快速操作
- **Apple官方**：系统字体、圆角规范、玻璃效果

## 文件大小与性能

| 文件 | 大小 | 说明 |
|------|------|------|
| home.html | ~8KB | 首页 |
| search.html | ~5KB | 搜索页 |
| detail.html | ~15KB | 详情页 |
| workspace.html | ~6KB | 工作台 |
| profile.html | ~6KB | 个人页 |
| styles.css | ~4KB | 自定义样式 |
| **总计** | **~44KB** | **极轻量级** |

> 外部资源（CDN）：Tailwind CSS、FontAwesome、Unsplash图片

## 浏览器兼容性
- ✅ Chrome (推荐)
- ✅ Safari
- ✅ Firefox
- ✅ Edge
- ✅ 移动浏览器

## 许可证与资源

### 开源许可
- 代码：MIT License（可自由使用、修改、商用）
- 图片：来自Unsplash（CC0许可，可免费使用）
- 图标：FontAwesome（可商用）

### 致谢
感谢以下服务提供商：
- [Tailwind CSS](https://tailwindcss.com/) - 样式框架
- [FontAwesome](https://fontawesome.com/) - 图标库
- [Unsplash](https://unsplash.com/) - 免费高质量图片
- [Apple Human Interface Guidelines](https://developer.apple.com/design/human-interface-guidelines/) - 设计规范

## 联系与反馈

发现问题或有改进建议？欢迎提Issue或PR！

---

**最后更新**：2024年
**设计者**：UI/UX Designer
**项目状态**：✅ 活跃维护中

## 技术栈

- **HTML5** - 页面结构
- **Tailwind CSS** - 样式框架（CDN）
- **FontAwesome 6.4.0** - 图标库（CDN）
- **Unsplash** - 图片资源
