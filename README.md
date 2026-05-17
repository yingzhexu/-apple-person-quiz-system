# 苹果人答题系统 / Apple Person Quiz System

- [中文说明](#中文说明)
- [English README](#english-readme)

---

# 中文说明

一个 iOS 风格的网页答题系统，围绕“户晨风 / 户子 / 苹果体系”相关互联网梗与判断模型制作。

这个项目不是单纯背答案，而是把“总成本、效率、标准化、现金流、工具思维、城市选择、社交过滤、现实筛选”等概念做成选择题、成就系统和最终测试，适合用来朋友互测、梗文化教学、直播互动、前端 UI 练习。

## 如何下载和使用

本项目是纯静态网页，不需要后端，也不需要安装依赖。

### 方法一：直接下载 ZIP

1. 打开本项目 GitHub 仓库页面
2. 点击绿色按钮 `Code`
3. 选择 `Download ZIP`
4. 解压下载好的 ZIP 文件
5. 进入解压后的文件夹
6. 双击 `index.html`
7. 浏览器打开后即可开始答题

### 方法二：用 Git 克隆

如果你熟悉 Git，可以使用：

```bash
git clone https://github.com/yingzhexu/-apple-person-quiz-system.git
cd -apple-person-quiz-system
```

然后直接打开：

```bash
open index.html
```

Windows 用户可以直接双击 `index.html`。

### 方法三：部署成在线网页

如果你想让别人不用下载，直接打开链接就能玩，可以用 GitHub Pages 部署。

如果你部署到了 GitHub Pages，也可以直接分享 Pages 链接给别人玩。

## 户晨风 / 苹果体系是什么？

“户晨风 / 户子 / 苹果体系”在这里指一种网络语境下的生活方式梗和判断框架。

它把“苹果”当成一种象征：标准化、少折腾、长期稳定、总成本更低、时间效率更高、现金流更健康。

它把“安卓”当成另一种象征：只看眼前便宜、忽略隐形成本、低效率、低标准、反复折腾。

注意：这里的“苹果 / 安卓”不是严格指手机品牌，也不是让人无脑买贵东西。这个系统真正想表达的是：

> 不只看标价，而是看长期总成本；不只看面子，而是看现金流、时间效率和可持续增长。

## 功能亮点

- 500 道普通题库
- 50 道固定顺序最终测试
- 支持 `10 / 20 / 50 / 100` 题随机抽题
- “我是苹果人”入口，进入最终测试
- 中英文切换，包括英文题库、英文 UI、英文语音播报、英文成就
- 每题选项自动打乱，避免答案集中在 A/B/C/D
- iOS 风格玻璃拟态界面
- Apple Pay 风格答对动画
- 答题音效和语音播报可独立开关
- 自动翻页，答完后进入结算页
- 正确率成就系统，答题中会弹出阶段成就
- 结算页展示称号、成就、正确率、最高连对、系统评级

## 怎么玩？

1. 打开 `index.html`
2. 选择题量：`10题 / 20题 / 50题 / 100题`
3. 点击 `开始`
4. 每题选择一个答案
5. 答对会出现类似 Apple Pay 的打勾动画和成功音效
6. 系统会自动进入下一题
7. 答完后进入结算页，查看你的称号和成就

## 最终测试

首页点击：

```text
我是苹果人
```

会进入最终测试提示页：

```text
既然你是苹果人了
请接受最终测试（50）道
```

最终测试固定 50 道，不随机抽题，适合做压轴挑战。

## 中英文切换

点击右上角 `EN / 中` 按钮即可切换语言。

英文模式会切换：

- 页面按钮
- 普通题库
- 最终测试题库
- 语音播报
- 成就系统
- 结算页文案

## 声音控制

右上角有两个独立按钮：

- 语音播报：控制答题语音
- 答题音效：控制点击、答对、答错、开始等音效

默认两个都开启。

## 成就系统

成就根据“答对比例”计算，只看正确率，不看题目数量。

例如：

- `0% - 9%`：系统绝缘体
- `10% - 19%`：轻度污染者
- `20% - 29%`：初级感染
- `30% - 39%`：入门玩家
- `40% - 49%`：稳定入门者
- `50% - 59%`：标准候选人
- `60% - 69%`：苹果人执行者
- `70% - 79%`：高阶候选人
- `80% - 89%`：高阶执行者
- `90% - 99%`：亲传级玩家
- `100%`：终极苹果人

答题过程中，如果正确率进入新的阶段，会自动弹出一个成就。结算页也会根据最终正确率展示对应称号。

## 部署到 GitHub Pages

1. 打开仓库 `Settings`
2. 找到 `Pages`
3. `Source` 选择 `Deploy from a branch`
4. `Branch` 选择 `main`
5. 文件夹选择 `/root`
6. 保存后等待 GitHub 生成访问链接

因为本项目是静态网页，所以不需要构建命令。

部署成功后，GitHub 会给你一个类似这样的链接：

```text
https://你的用户名.github.io/仓库名/
```

之后你把这个链接发给别人，对方就可以直接在线答题。

## 文件结构

```text
.
├── index.html                  # 页面结构
├── styles.css                  # iOS 风格界面与动画
├── app.js                      # 主逻辑、中文题库、成就系统
├── questions-en.js             # 英文题库 1-200 + 最终测试 1-3
├── questions-en-201-300.js     # 英文题库 201-300
├── questions-en-301-400.js     # 英文题库 301-400
├── questions-en-401-500.js     # 英文题库 401-500
├── questions-en-final.js       # 英文最终测试 4-50
├── README.md
└── LICENSE
```

## 二次开发

你可以直接修改：

- `app.js`：中文题库、答题逻辑、成就系统、声音逻辑
- `styles.css`：界面样式、动画、玻璃拟态效果
- `questions-en*.js`：英文题库内容
- `index.html`：页面结构和按钮

题库格式是：

```text
题号|题目|A选项|B选项|C选项|D选项|正确答案
```

例如：

```text
1|超市就去哪里？|菜市场|山姆|小区杂牌超市|路边小卖部|B
```

## 免责声明

本项目是一个粉丝向、梗文化、娱乐性质的开源网页项目，仅用于网页开发学习、互动娱乐、朋友测试、梗文化整理和 UI 设计练习。

本项目不是户晨风本人或其团队的官方作品，也不代表户晨风本人的真实观点、完整观点或任何商业授权关系。

本项目与 Apple、Tesla、Sam's Club、McDonald's、Haidilao、Xibei 等品牌或主体没有任何官方关系。项目中出现的品牌名称仅用于题目语境、互联网梗语境和示例表达，不代表品牌方参与、认可、赞助或背书。

题目中的“苹果 / 安卓”是网络语境下的象征化表达，不是对真实手机系统、真实品牌、真实用户群体或任何个人的客观评价，也不应被理解为歧视、贬低或攻击任何消费选择。

本项目中的题目、选项、成就称号和结算文案都带有夸张、戏谑、梗文化和娱乐化表达。请不要把它当成现实生活、职业选择、消费决策、城市选择、健康管理、投资理财或人际关系处理的绝对建议。

如果你基于本项目内容做任何现实决策，请结合自己的实际情况、预算、健康状况、家庭环境、职业阶段和专业意见独立判断。

如果你二次修改、转载、部署或传播本项目，请保留娱乐性质说明，避免将题目内容包装成严肃测评、商业诊断或现实价值评判工具。

## License

MIT

---

# English README

An iOS-style browser quiz app inspired by the internet meme culture around “Huchengfeng / Huzi / the Apple Person System.”

This project is not just about memorizing answers. It turns concepts such as total cost, efficiency, standardization, cash flow, tool thinking, city choice, social filtering, and realistic screening into multiple-choice questions, achievements, sound effects, animations, and a final test mode.

It is suitable for meme-culture teaching, friend challenges, livestream interaction, UI practice, and front-end learning.

## How to Download and Use

This is a pure static web project. It does not require a backend, package manager, build step, or dependency installation.

### Option 1: Download ZIP

1. Open this GitHub repository.
2. Click the green `Code` button.
3. Choose `Download ZIP`.
4. Unzip the downloaded file.
5. Open the extracted folder.
6. Double-click `index.html`.
7. The quiz will open in your browser.

### Option 2: Clone with Git

If you are familiar with Git:

```bash
git clone https://github.com/yingzhexu/-apple-person-quiz-system.git
cd -apple-person-quiz-system
```

Then open:

```bash
open index.html
```

On Windows, you can simply double-click `index.html`.

### Option 3: Deploy as a Website

If you want other people to play without downloading anything, deploy it with GitHub Pages.

## What Is the Huchengfeng / Apple Person System?

In this project, “Huchengfeng / Huzi / Apple Person System” refers to a meme-based lifestyle framework and internet joke system.

“Apple” is used as a symbol for:

- standardization
- less hassle
- long-term stability
- lower total cost
- higher time efficiency
- healthier cash flow

“Android” is used as a symbol for:

- only looking at short-term cheapness
- ignoring hidden costs
- low efficiency
- low standards
- repeated hassle

Important: “Apple / Android” here is not strictly about phone brands. It is not telling people to blindly buy expensive things. The core idea is:

> Do not only look at the sticker price. Look at long-term total cost, cash flow, time efficiency, and sustainable growth.

## Features

- 500 regular quiz questions
- 50 fixed final-test questions
- Random quiz modes: `10 / 20 / 50 / 100` questions
- “I’m an Apple Person” entry for the final test
- Chinese / English language switch
- English question bank, English UI, English voice, and English achievements
- Automatic option shuffling for every question
- iOS-style glassmorphism interface
- Apple Pay-style correct-answer animation
- Separate voice and sound-effect toggles
- Auto-next after answering
- Achievement system based on correct-answer percentage
- Result page with title, achievement, accuracy, best streak, and system rating

## How to Play

1. Open `index.html`.
2. Choose a quiz size: `10 / 20 / 50 / 100`.
3. Click `Start`.
4. Pick one answer for each question.
5. Correct answers trigger a checkmark animation and success sound.
6. The app automatically moves to the next question.
7. After the quiz ends, the result page shows your title and achievement.

## Final Test

On the home screen, click:

```text
I’m an Apple Person
```

You will enter the final-test intro:

```text
So you are an Apple Person
Take the final test: 50 questions
```

The final test always uses the same 50 questions in a fixed order. It is designed as the challenge mode.

## Language Switch

Click the `EN / 中` button in the top-right corner.

English mode switches:

- interface text
- regular question bank
- final test question bank
- voice narration
- achievements
- result page text

## Sound Controls

There are two separate buttons in the top-right corner:

- `Voice`: controls speech narration
- `Sound Effects`: controls clicks, correct/wrong feedback, and start sounds

Both are enabled by default.

## Achievement System

Achievements are calculated by correct-answer percentage, not by raw question count.

Examples:

- `0% - 9%`: System Insulator
- `10% - 19%`: Lightly Contaminated
- `20% - 29%`: Early Infection
- `30% - 39%`: Entry Player
- `40% - 49%`: Stable Beginner
- `50% - 59%`: Standard Candidate
- `60% - 69%`: Apple Person Operator
- `70% - 79%`: Advanced Candidate
- `80% - 89%`: Advanced Operator
- `90% - 99%`: Direct Disciple
- `100%`: Ultimate Apple Person

During the quiz, when your correct-answer percentage enters a new achievement tier, a single achievement toast appears. The final result page also displays the matching title and achievement.

## Deploy to GitHub Pages

1. Open repository `Settings`.
2. Go to `Pages`.
3. Set `Source` to `Deploy from a branch`.
4. Choose branch `main`.
5. Choose folder `/root`.
6. Save and wait for GitHub to generate the site URL.

No build command is needed because this project is fully static.

After deployment, GitHub will give you a URL like:

```text
https://your-username.github.io/repository-name/
```

Share that link and anyone can play online.

## File Structure

```text
.
├── index.html                  # Page structure
├── styles.css                  # iOS-style UI and animations
├── app.js                      # Main logic, Chinese questions, achievements
├── questions-en.js             # English questions 1-200 + final test 1-3
├── questions-en-201-300.js     # English questions 201-300
├── questions-en-301-400.js     # English questions 301-400
├── questions-en-401-500.js     # English questions 401-500
├── questions-en-final.js       # English final test 4-50
├── README.md
└── LICENSE
```

## Development

You can edit:

- `app.js`: Chinese question bank, quiz logic, achievements, sounds
- `styles.css`: UI, layout, animations, glass effects
- `questions-en*.js`: English question content
- `index.html`: page structure and buttons

Question format:

```text
id|question|option A|option B|option C|option D|correct answer
```

Example:

```text
1|Where should you go for groceries?|Wet market|Sam's Club|Random neighborhood supermarket|Roadside convenience store|B
```

## Disclaimer

This is a fan-made, meme-culture, entertainment-oriented open-source web project. It is intended for front-end learning, UI design practice, friend challenges, cultural archiving, and casual interaction.

This project is not an official work by Huchengfeng or any related team. It does not represent Huchengfeng’s real views, complete views, commercial authorization, or official endorsement.

This project has no official relationship with Apple, Tesla, Sam's Club, McDonald's, Haidilao, Xibei, or any other brand mentioned in the questions. Brand names appear only as part of meme context, quiz context, or example wording. Their appearance does not imply participation, approval, sponsorship, or endorsement.

The terms “Apple” and “Android” in this project are symbolic internet expressions. They are not objective evaluations of real phone systems, real brands, real user groups, or any individual. They should not be understood as discrimination, insult, or attack against any consumer choice.

The questions, options, achievement titles, and result texts are intentionally exaggerated, playful, and meme-driven. Do not treat them as serious real-life advice for career choices, consumer decisions, city selection, health management, investment, finance, or relationships.

If you make real-life decisions, consider your own budget, health, family context, career stage, environment, and professional advice.

If you modify, repost, deploy, or redistribute this project, please keep the entertainment disclaimer and avoid presenting it as a serious assessment, commercial diagnosis, or real-world value judgment tool.

## License

MIT
