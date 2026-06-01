# 🐻 CS61A: The Ultimate Visual Guide & Survival Kit (UC Berkeley)

> 🌐 **[⚡ EN: Click here to start the ultra-fast interactive reading experience in your browser!](https://sirizhao.github.io/CS61A-Visual-Survival-Guide/)**
> 🌐 **[⚡ 中文: 点击这里，直接在浏览器中开启极速视觉交互阅读体验！](https://sirizhao.github.io/CS61A-Visual-Survival-Guide/)**

[![GitHub stars](https://img.shields.io/github/stars/SiriZhao/CS61A-Visual-Survival-Guide?style=flat-square&logo=github)](https://github.com/SiriZhao/CS61A-Visual-Survival-Guide)
[![Python](https://img.shields.io/badge/Python-3.9%2B-yellow?style=flat-square&logo=python)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

---

## 🎨 Why This Repository? / 为什么选择本仓库？

### 🇬🇧 English
Most CS61A repositories are just messy code dumps or plain texts. This project is built to **productize and visualize abstract computer science concepts**:
* **👁️ Immersive HTML Interactive Experience**: Native HTML5+CSS3 responsive design, featuring the gorgeous *Atom One Dark* dark mode and elegant modern typography.
* **🔍 Step-by-Step Trace Blocks**: For mind-boggling concepts like `Environment Diagrams`, `Closures`, and `Lambda expressions`, we designed exclusive **[🔍 Trace]** visual guides to unpack every single line of code execution.
* **🚀 Long-term Evolution**: Currently fully synchronized with **Midterm 1 (Lectures 2-8)**. Future tough topics (Recursion, Trees, OOP, Scheme Interpreters) will be 100% covered.

### 🇨🇳 中文
网上的 CS61A 资料千篇一律，要么是枯燥的纯文本，要么是直接丢作业答案。本仓库的核心理念是 **"把抽象的逻辑完全具象化"**：
* **👁️ 沉浸式 HTML 交互体验**：笔记原生采用 HTML5+CSS3 响应式设计，内置精致的暗黑模式（Atom One Dark）、现代非对称字体和高亮代码块。
* **🔍 逐步追踪 (Trace) 视觉框**：针对最玄学的 `Environment Diagrams`（环境图）、`Closure`（闭包陷阱）和 `Lambda`，独创了 **[🔍 Trace / 逐步追踪]** 引导模块，像老师在黑板上拆解一样厘清底层流转。
* **🚀 长期动态进化**：本库目前已完美收录 **Midterm 1 核心串讲（Lecture 2 - 8）**。后续将随着课程推进，100% 还原并可视化后续所有硬核章节（递归、数据抽象、OOP、Scheme 解释器）。

---

## 🗺️ Roadmap & Progress / 动态路线图与进度

- [x] **📦 Part 1: Functional Programming & Environments (Midterm 1 / Lec 2-8)** `[🎉 100% Done]`
  - *Highlights / 亮点: Generalization, `make_adder` closure, `delay`, `pirate`, and `horse` trick questions breakdown*
- [ ] **🌿 Part 2: Data Abstraction, Sequences & Recursion (Midterm 2 / Lec 9+)** `[🚧 In Progress...]`
- [ ] **🏛️ Part 3: Object-Oriented Programming & Mutation** `[⏳ Planned]`
- [ ] **🚀 Part 4: Scheme Language, Interpreters & SQL** `[⏳ Planned]`

---

## 📂 Navigation / 黄金目录导航

| Phase / 课程阶段 | 📝 Visual Notes (Click to preview) / 核心笔记（在线直达） | 💡 Visual Highlights / 视觉看点 |
| :--- | :--- | :--- |
| **Midterm 1 Sprint** | [📖 HTML Visual Notes (Lec 2-8)](https://sirizhao.github.io/CS61A-Visual-Survival-Guide/) | **Environment Diagram Six-Step Rules**, `delay()`, `pirate()`, `horse()` walkthroughs |
| **Midterm 2 Attack** | 🚧 Constructing... (Star to get notified!) | Coming soon... |

---

## 💡 Showcase & Preview / 精彩内容快照

### 1️⃣ Golden Rule of Environment Diagrams / 环境图绝对铁律
⚠️ **The parent link of a new frame ALWAYS points to the environment where the function was DEFINED, NOT where it was CALLED!**

⚠️ **新帧的父链接 (Parent Link) 永远指向该函数「定义时」的环境，而非「调用时」的环境！**

### 2️⃣ The Infamous `horse()` Question Breakdown / 杀手题 `horse()` 视觉拆解

```python
def horse(mask):
    horse = mask              # 1. Local 'horse' bound to external lambda
    def mask(horse):          # 2. Local 'mask' shadows the parameter
        return horse
    return horse(mask)        # 3. 'horse' here is still the external lambda!
```

**Core Insight:** Line 1 executes before Line 2's definition. Therefore, `horse` firmly locks the original lambda closure, successfully bypassing the subsequent shadowing trap. The evaluation result is `2`.

**核心精髓：** 第一行在第二行定义前执行。因此 `horse` 牢牢锁定了原始 lambda 闭包，最终巧妙避开了后续的覆盖陷阱，求值结果为 `2`。

---

## 🤝 Contribution & Academic Honesty / 贡献声明与学术诚信

**Contribution:** Issues and Pull Requests are highly welcome! Let's build the best CS61A companion guide together.

**Academic Honesty:** This repository is for educational and self-study purposes only. If you are currently enrolled in UC Berkeley or any other university, please strictly adhere to your school's Academic Honesty guidelines. DO NOT copy code directly for project submissions.

---

❤️ If these visualized HTML notes helped you, please give this repository a Star 🌟! It drives me to update the remaining parts!

❤️ 如果这些网页可视化笔记理清了你的思绪，请帮我点一个 Star 🌟，这是对我持续更新最大的鼓励！
