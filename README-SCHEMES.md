# 点滴 · 多方案 Tweaks

从 `meiyou-diandi-jingqi` main（`213dc14`）拉出的独立仓库，用于对比不同交互/视觉方案。

## 打开

本地起静态服务后打开根目录 `index.html`。右下角 **方案 Tweaks** 面板可切换：

| 分组 | 项 | 说明 |
|------|----|------|
| Liquid Dock | 毛玻璃透明度 | 透白 / 柔白 / 实灰 |
| 经期反馈 | 趋势入口时机 | 播完再出 / 立刻出现 |
| 经期反馈 | 月经走了图标 | 水滴内勾 / 角标勾 |
| 经期反馈 | 来了引导文案 | 输入框预填后缀 |

## 加新方案

1. 在 `index.html` 的 `TWEAK_DEFAULTS` 增加字段  
2. 在 `app.jsx` 的 `<TweaksPanel>` 加控件  
3. 用 `window.__LIVE_TWEAKS` 或 `document.documentElement.dataset.*` 接到样式/逻辑  

定稿后把选中方案回写到主仓库 `meiyou-diandi-jingqi`。
