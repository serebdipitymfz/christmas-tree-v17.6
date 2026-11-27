# 🎄 christmas-tree-v17.6（微信兼容版）

Grand Luxury Tree v17.6 — 单文件 Three.js 粒子圣诞树，已针对手机微信内置浏览器优化。

**在线预览：https://serebdipitymfz.github.io/christmas-tree-v17.6/**

## 本次改造（微信兼容）

原版在微信里打不开，原因是依赖 ES Module + importmap、jsDelivr CDN、Google Fonts、Google 手势模型（国内均不可达）。现已改为：

- 所有 Three.js 及插件用 esbuild 打包成经典脚本内联进 `index.html`，**零外部依赖**，单文件即可运行。
- 移除 Google Fonts，改用系统字体栈（iOS/安卓微信自带字体，无需联网）。
- 微信内置浏览器中自动跳过摄像头手势识别（微信无可用的 `getUserMedia`），不影响主场景；非微信环境且摄像头可用时手势功能仍保留。

## 操作说明

| 操作 | 效果 |
| --- | --- |
| 拖动 / 单指滑动 | 旋转场景 |
| 双指缩放 | 缩放 |
| 聚合 / 散开 按钮（或空格 / Z） | 切换圣诞树 / 星云形态 |
| 抓图（或 X） | 保存当前画面 |
| 镜头 | 显示/隐藏摄像头画面（微信里不可用） |
| 设置 | 打开文字、音乐、粒子等设置面板 |

## 致谢

项目源自 [liq47317-boop/christmas-tree-v17.6](https://github.com/liq47317-boop/christmas-tree-v17.6)。
