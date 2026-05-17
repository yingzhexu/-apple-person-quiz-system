# 苹果人答题系统 / Apple Person Quiz System

一个 iOS 风格的网页答题系统，围绕“户子 / 苹果体系”的总成本、效率、标准化、现金流、城市选择、工具思维、社交过滤等内容设计。

This is an iOS-style browser quiz app about the “Apple Person System”: total cost, efficiency, standardization, cash flow, city choice, tool thinking, and social filtering.

## 功能亮点

- 500 道普通题库，支持 10 / 20 / 50 / 100 题随机抽题
- 50 道固定顺序最终测试
- 中英文界面切换，包含英文题库与英文语音播报
- 每题选项自动打乱，避免答案集中在某个选项
- iOS / Apple Pay 风格答对动画和音效
- 语音播报与答题音效可分别开关
- 根据正确率触发成就系统，并在结算页展示称号
- 隐藏测试后门：连续点击顶部制作名 10 次，可选择题量直接满分结算

## 使用方式

直接用浏览器打开 `index.html` 即可运行，无需安装依赖。

```text
index.html
```

如果你想部署到 GitHub Pages，把整个仓库推送到 GitHub 后，在仓库设置里开启 Pages，选择根目录作为发布源即可。

## 文件结构

```text
.
├── index.html
├── styles.css
├── app.js
├── questions-en.js
├── questions-en-201-300.js
├── questions-en-301-400.js
├── questions-en-401-500.js
└── questions-en-final.js
```

## 开源说明

本项目是一个静态网页小工具，适合用于梗文化教学、朋友测试、答题互动和前端 UI 练习。

题库内容来自用户整理的“户子 / 苹果体系”选择题；项目代码以 MIT License 开源。

## License

MIT
