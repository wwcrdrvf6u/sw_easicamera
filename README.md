# sw_easicamera
# 希沃视频展台（我写的）
## 下载 download
[releases] https://github.com/wwcrdrvf6u/sw_easicamera/releases/tag/easicamera
## 软件介绍

希沃视频展台专业版是一款专为教育场景设计的视频展示工具，集成了实时摄像头展示、图像批注、梯形校正、画面调节和扫描功能。软件特别优化了触控操作体验，支持全屏模式，方便教师在教学过程中展示实物、批注重点内容。

### 主要功能：
- **实时摄像头展示**：支持多摄像头切换和自动连接
- **专业批注工具**：提供画笔、橡皮擦工具，支持实时批注
- **梯形校正**：消除摄像头角度造成的图像畸变
- **画面调节**：调整亮度、对比度、旋转和镜像
- **扫描功能**：模拟扫描仪效果，逐行捕获图像
- **照片管理**：内置照片库管理捕获的图像
- **移动缩放**：支持画面拖动和缩放操作
- **触控优化**：完美支持触摸屏设备操作

## 文件目录结构

```
希沃视频展台专业版/
├── easicamera.py                # 主程序文件
├── config.json                  # 配置文件（自动生成）
├── boot.JPG                     # 启动画面图片
├── icons/                       # 工具图标目录
│   ├── adjust.png               # 画面调节图标
│   ├── capture.png              # 拍照图标
│   ├── clear.png                # 清除图标
│   ├── correction.png           # 梯形校正图标
│   ├── eraser.png               # 橡皮擦图标
│   ├── exit.png                 # 退出图标
│   ├── minimize.png             # 最小化图标
│   ├── move.png                 # 移动工具图标
│   ├── pen.png                  # 画笔图标
│   ├── photos.png               # 照片库图标
│   ├── save.png                 # 保存图标
│   ├── scan.png                 # 扫描图标
│   ├── settings.png             # 画笔设置图标
│   ├── switch_camera.png        # 切换摄像头图标
│   └── undo.png                 # 撤回图标
└── captures/                    # 捕获照片存储目录（可选）
    ├── 20231015_093045.jpg      # 示例捕获的照片
    └── scan_20231015_093512.jpg # 示例扫描的照片
```

## 使用说明

### 基本操作：
1. 启动软件后会自动检测并连接摄像头
2. 使用底部工具栏选择工具：
   - 画笔：红色默认颜色，可在设置中更改
   - 橡皮擦：擦除批注内容
   - 移动：拖动和缩放画面
   - 扫描：模拟扫描仪效果
3. 拍摄的照片会自动保存到照片库

### 快捷键：
- 空格键：拍照
- P键：画笔工具
- M键：移动工具
- E键：橡皮擦工具
- Ctrl+Z：撤回操作
- Ctrl+S：保存当前画面
- Esc：退出软件

### 高级功能：
1. **梯形校正**：点击"梯形校正"按钮，拖动四个角点调整图像
2. **画面调节**：调整亮度、对比度、旋转和镜像效果
3. **扫描功能**：点击"扫描"按钮开始逐行捕获图像
4. **照片管理**：点击"照片"按钮查看所有捕获的图像

## 技术特点
- 基于PySide2和OpenCV开发
- 支持高DPI显示和触控操作
- 自动保存用户配置（摄像头设置、校正点等）
- 多线程摄像头初始化，避免界面卡顿
- 实时图像处理优化

## 运行要求
- Python 3.6+
- 依赖库：`opencv-python`, `numpy`, `PySide2`
- 操作系统：Windows/macOS/Linux

## 安装指南
1. 安装Python 3.6或更高版本
2. 安装依赖库：
      pip install opencv-python numpy PySide2
   
3. 下载软件文件到本地目录
4. 运行主程序：
      python easicamera.py
   

这款软件特别适合教育场景，帮助教师清晰地展示教材、实验过程和学生作品，提升课堂教学效果。
