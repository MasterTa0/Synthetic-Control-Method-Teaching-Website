<h1 align="center">
  <!-- 可选：把下方 logo 路径替换成你仓库里实际存在的图片（例如 ./assets/logo.png） -->
  <img src="./assets/logo.png" alt="SCM" width="128" />
  <br>
  合成控制法（Synthetic Control Method）教学网站
  <br>
</h1>

<h3 align="center">
因果推断课程 · 针对“单一/少数处理单位”的面板政策评估工具（SCM）
</h3>

<p align="center">
  在线访问：
  <a href="https://masterta0.github.io/Synthetic-Control-Method-Teaching-Website/">GitHub Pages</a>
</p>

<p align="center">
  模块导航：
  概览 · 形式化定义 · 公式推导 · 理论与证明 · 与其他方法对比 · 经典案例 · 参考文献
</p>

---

## Preview

| Overview（概览）                 | Applications（经典案例）              |
| -------------------------------- | ------------------------------------- |
| ![overview](./docs/preview_overview.png) | ![applications](./docs/preview_applications.png) |

> 说明：如果你仓库里还没有预览图，可以先把这两张占位图删掉，或把路径改成你实际放置的截图文件。

---

## Access

直接打开在线版本即可学习与引用：

- Web: https://masterta0.github.io/Synthetic-Control-Method-Teaching-Website/

---

## Course Outline

本项目以“一讲可用”的课程讲义为目标，建议按顺序学习；也可按需跳转到案例与实务部分。

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
   - DiD、Matching、ITS 等方法的典型场景与关键假设
   - SCM 与 DiD 的关系（“等权重 SCM”视角等）

6. **经典案例与练习示例**
   - 巴斯克恐怖主义与经济损失（教学用示例数据 + 步骤流程）
   - 加州控烟政策 Proposition 99（R / Python 通用思路 + 练习任务）

7. **实务要点与进一步阅读**
   - 拟合质量诊断、对照库选择
   - Placebo / 灵敏度分析的实务建议
   - 推荐阅读（经典文献清单）

---

## Learning Objectives

完成学习后，你应该能够：

- 解释 SCM 的适用场景、核心直觉与局限性
- 写出 SCM 的关键记号（潜在结果、权重约束、合成对照）
- 理解权重求解问题（目标函数、约束、V 矩阵含义）
- 用因子模型语言复述识别逻辑与证明思路
- 对比 SCM 与 DiD / Matching / ITS 的差异与联系
- 复述并复现实证经典案例的基本流程（含 placebo 思路）

---

## Local Preview

如果你想在本地浏览（不改代码也可用），推荐用“静态服务器”方式启动：

### Option A: Python（推荐）

```bash
python3 -m http.server 8000
# 然后浏览器打开：http://localhost:8000
