# GitHub Profile 项目说明

## 项目概述
本项目是一个展示个人 GitHub 信息的 HTML 页面，通过简洁而美观的界面展示个人头像、姓名、个人名言以及一些代表性项目链接。页面背景图会随机从指定图片列表中选择，同时名言也会随机显示，为页面增添了一些动态和趣味性。

## 项目结构
项目主要包含一个 HTML 文件 `GitHub Profile.html`，其结构如下：
- **HTML 部分**：构建页面的基本结构，包括头部信息、主体内容以及各个元素的布局。
- **CSS 部分**：对页面进行样式设计，包括字体、颜色、布局、背景等方面的设置，确保页面美观且具有响应式设计。
- **JavaScript 部分**：实现页面的动态效果，如随机选择背景图片和名言。

## 主要功能
### 1. 随机背景图片
页面加载时，会从 `img` 文件夹中的 10 张图片中随机选择一张作为背景图，为页面带来不同的视觉效果。相关代码如下：
```javascript
const images = ['1.jpg', '2.jpg', '3.jpg', '4.jpg', '5.jpg', '6.jpg', '7.jpg', '8.jpg', '9.jpg', '10.jpg'];
const randomImage = images[Math.floor(Math.random() * images.length)];
document.body.style.backgroundImage = `url('img/${randomImage}')`;