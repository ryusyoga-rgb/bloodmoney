# 📸 Meme Generator 图片设置指南

## 🎯 快速设置

### 1. 创建图片文件夹
在网站根目录下创建一个名为 `images` 的文件夹：

```
D:\Download\bloodgame\
├── index.html
├── images-setup.md
└── images\
    ├── harvey1.png  ← 你的第一张图片
    ├── harvey2.png  ← 你的第二张图片  
    ├── harvey3.png  ← 你的第三张图片
    ├── harvey4.png  ← 你的第四张图片
    ├── harvey5.png  ← 你的第五张图片
    └── harvey6.png  ← 你的第六张图片
```

### 2. 重命名你的图片文件
将你的6张PNG文件重命名为：
- `harvey1.png`
- `harvey2.png`
- `harvey3.png`
- `harvey4.png`
- `harvey5.png`
- `harvey6.png`

### 3. 放置图片
将重命名后的图片文件放入 `images` 文件夹中。

## 🔧 技术细节

### 图片规格建议
- **格式**: PNG (支持透明背景)
- **尺寸**: 建议 400x400px 或更大
- **文件大小**: 建议 1MB 以下以保证加载速度
- **宽高比**: 1:1 (正方形) 效果最佳

### 代码功能说明
```html
<!-- 图片会自动加载，如果加载失败会显示彩色占位符 -->
<img src="images/harvey1.png" alt="Harvey 1" 
     onerror="this.style.display='none'; this.nextElementSibling.style.display='flex';">
```

### JavaScript 图片预加载
```javascript
function preloadImages() {
    const imageNames = ['harvey1', 'harvey2', 'harvey3', 'harvey4', 'harvey5', 'harvey6'];
    // 自动预加载所有图片到内存中
}
```

## 🎨 功能特性

### ✅ 已实现的功能
1. **图片预加载** - 页面加载时自动缓存图片
2. **回退机制** - 图片不存在时显示美观的占位符
3. **自适应缩放** - 图片自动适应画布大小
4. **选择反馈** - 选中状态有视觉反馈
5. **悬停效果** - 鼠标悬停时有缩放动画

### 🎭 Meme 生成器功能
- 📝 可拖拽文字
- 🎨 可调节文字大小和颜色
- 🖼️ 支持6张不同的Harvey图片
- 💾 一键下载PNG格式
- 📱 响应式布局，支持手机和桌面

## 🚀 测试步骤

1. **创建文件夹**: 在网站目录创建 `images` 文件夹
2. **添加图片**: 放入你的6个PNG文件
3. **重命名**: 确保文件名为 `harvey1.png`, `harvey2.png`, `harvey3.png`, `harvey4.png`, `harvey5.png`, `harvey6.png`
4. **刷新页面**: 重新打开网站查看效果
5. **测试功能**: 点击不同图片，添加文字，拖拽位置
6. **检查布局**: 确认6张图片在2行3列的网格中正确显示

## 🔍 故障排除

### 图片不显示？
1. 检查文件名是否正确
2. 确认图片在正确的文件夹中
3. 检查图片格式是否为PNG
4. 查看浏览器控制台是否有错误信息

### 占位符仍然显示？
这是正常的！如果图片无法加载，系统会自动显示彩色占位符，确保用户体验不受影响。

### 文字拖拽不工作？
确保点击的是文字本身，而不是空白区域。文字会有黑色描边，便于识别。

## 📞 技术支持

如果遇到任何问题，检查：
- 文件路径是否正确
- 图片文件名拼写
- 浏览器控制台错误信息
- 图片文件是否损坏

---

**设置完成！** 🎉
现在你的meme生成器已经支持真实图片了！