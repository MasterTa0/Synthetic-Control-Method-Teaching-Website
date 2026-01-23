<div align="center">

# 合成控制法（Synthetic Control Method, SCM）教学网站

因果推断课程 · 针对“单一/少数处理单位”的面板政策评估工具（SCM）
- Web（GitHub Pages）：
<p>
  <a href="https://masterta0.github.io/Synthetic-Control-Method-Teaching-Website/">
    <img alt="GitHub Pages" src="https://img.shields.io/badge/GitHub%20Pages-Online-blue" />
  </a>
</p>

在线访问：
<a href="https://masterta0.github.io/Synthetic-Control-Method-Teaching-Website/">https://masterta0.github.io/Synthetic-Control-Method-Teaching-Website/</a>

</div>

---

## 目录

- [Access](#access)
- [Course Outline](#course-outline)
- [Learning Objectives](#learning-objectives)
- [Local Preview](#local-preview)
- [Deployment (GitHub Pages)](#deployment-github-pages)
- [References](#references)
- [Contributing](#contributing)
- [License](#license)

---

## Access


> 说明：你之前 README 里引用了 `./assets/logo.png`、`./docs/preview_*.png`，但仓库中未提供对应文件，GitHub 会显示“破图”。
> 本版本 README 默认不引用本地图片，避免渲染失败；如需展示截图，可在 `docs/` 下补充图片后再加回引用。

---

## Course Outline

网站内容以“从直觉到推导再到实证”的学习路径组织，建议按顺序阅读；也可按需跳转到案例与实务部分。

1. **直观理解与适用场景**
   - 直觉：合成“影子世界”
   - 典型适用场景（单一处理单位 + 多对照单位 + 较长干预前面板）

2. **形式化定义与记号**
   - 面板结构与潜在结果
   - 合成控制的数学定义与处理效应目标

3. **权重求解与优化**
   - 特征向量与加权距离（V 矩阵）
   - 带约束二次规划的权重求解
   - 得到权重后的效应估计（路径图 / 缺口图）

4. **理论基础与证明思路**
   - 因子模型下的识别逻辑
   - 理想权重与识别条件
   - 证明框架梳理（教学版）

5. **与其他方法对比**
   - DiD、Matching、ITS 等方法的关键假设与适用边界
   - SCM 与 DiD 的联系与差异

6. **经典案例与练习**
   - 巴斯克恐怖主义与经济损失
   - 加州控烟政策 Proposition 99

7. **实务要点与进一步阅读**
   - 拟合质量诊断、对照库选择
   - Placebo / 灵敏度分析
   - 推荐阅读与扩展方向

---

## Learning Objectives

完成学习后，你应能够：

- 解释 SCM 的适用场景、核心直觉与局限性
- 写出 SCM 的关键记号（潜在结果、权重约束、合成对照）
- 理解权重求解问题（目标函数、约束、V 矩阵含义）
- 用因子模型语言复述识别逻辑与证明思路
- 对比 SCM 与 DiD / Matching / ITS 的差异与联系
- 复述并复现实证经典案例的基本流程（含 placebo 思路）

---

## Local Preview

本项目为静态网页，建议用本地静态服务器预览：

### Option A: Python

```bash
python3 -m http.server 8000
# 浏览器打开：http://localhost:8000
