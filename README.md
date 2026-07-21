# AI model frontend test set

- 本项目所有（100%）代码均由 AI 生成。运行前请自行审查，任何后果概不负责。
- 一个基于 HTML5 Canvas 和 Three.js 的交互式天文、物理模拟合集，所有文件均为独立的 `.html` 文件，双击即可在浏览器中运行。

## 目录结构

```
stars/
├── a/        # 主版本 - Canvas 2D 完整功能模拟
├── d/        # 多样版本 - Three.js 3D 模拟 + 小游戏
├── q/        # 轻量版本 - Canvas 2D 精简模拟
└── z/        # 进阶版本 - Three.js + 自定义 Shader
```

## 项目列表

| 分类 | 子目录 | 文件名 | 技术栈 | 说明 |
|------|--------|--------|--------|------|
| 🪐 太阳系 | `a/` | `sun.html` | Canvas 2D | 八大行星运行模拟，含控制面板、行星选择、轨迹记录 |
| 🪐 太阳系 | `q/` | `solar-system.html` | Canvas 2D | 精简版太阳系模拟 |
| 🪐 太阳系 | `z/` | `sun-system.html` | Three.js + Shader | 3D 太阳系，自定义着色器、点击聚焦、图例交互 |
| 🌍 日地月 | `a/` | `seasons.html` | Canvas 2D | 四季成因演示，可调地轴倾角、昼夜标注 |
| 🌍 日地月 | `d/` | `solar-system-seasons.html` | Three.js | 3D 日地月系统，四季标记、地轴倾角 |
| 🌍 日地月 | `z/` | `seasons.html` | Three.js + Shader | 3D 四季模拟，昼夜分界线着色器、子太阳点标记 |
| 🛰️ 国际空间站 | `a/` | `iss.html` | Canvas 2D | ISS 轨道模拟，伪 3D 渲染、鼠标拖动旋转 |
| 🛰️ 国际空间站 | `z/` | `iss.html` | Three.js + Shader | 3D ISS 模拟，自定义地球着色器、夜景灯光 |
| 🌕 地月系统 | `d/` | `earth-moon.html` | Three.js | 地月质心系统，潮汐锁定、相位角计算 |
| 🧊 魔方 | `d/` | `cube.html` | Three.js | 3D 交互式魔方，键盘/按钮控制、打乱与计时 |
| 🎮 俄罗斯方块 | `d/` | `tetris.html` | Canvas 2D | 经典俄罗斯方块，Ghost Piece、计分等级 |
| 🏍️ 四冲程引擎 | `q/` | `moto.html` | Canvas 2D | 四缸摩托车发动机模拟，活塞/气门/点火动画 |
| ⚛️ 氢原子模型 | `q/` | `h2.html` | Canvas 2D | 氢原子模拟，玻尔轨道/量子云两种模式 |

## 使用方法

直接双击任意 `.html` 文件即可在浏览器中运行，或使用 HTTP 服务器：

```bash
python -m http.server 8000
```

## 技术特点

- **Canvas 2D** 版本：纯 HTML + CSS + JavaScript，零依赖
- **Three.js 3D** 版本：引入 Three.js 库（CDN），部分含自定义 GLSL Shader
- 所有模拟均支持交互控制（缩放、速度调节、暂停等）
- 响应式设计，适配不同屏幕尺寸
- 面向对象设计，高效的动画循环

## 浏览器兼容性

- Chrome / Edge - ✅ 完美支持
- Firefox - ✅ 完美支持
- Safari - ✅ 完美支持
- Opera - ✅ 完美支持

## 许可证

本项目为 AI 生成的演示用途代码，可自由使用和修改。
