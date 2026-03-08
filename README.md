# 🧭 Methodology Matcher / 任务方法论匹配器

**Version**: 1.0.0  
**Author**: 黑猫 🐈‍⬛  
**License**: MIT

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://github.com/GIS-blackCaat/methodology-matcher)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![OpenClaw](https://img.shields.io/badge/OpenClaw-Skill-orange.svg)](https://openclaw.ai)

---

## 📋 概述

**任务方法论匹配器** - 为复杂长期任务自动匹配适配的方法论框架。

**核心理念**：
- **简单任务** → 直接执行 ✅
- **复杂任务** → 方法论匹配 → 配置 → 执行 🔴

---

## 🎯 核心功能

| 功能 | 说明 |
|------|------|
| **📊 任务分类** | 自动检测任务复杂度（简单/中等/复杂） |
| **🧠 现代方法论** | 费曼技巧、PDCA、OKR、Agile、设计思维、GTD |
| **📜 中国古代方法论** | 格物致知、知行合一、循序渐进、温故知新、学以致用 |
| **🎯 自动匹配** | 根据任务类型推荐最适合的方法论 |
| **⚙️ 可配置** | 支持用户自定义方法论偏好 |

---

## 📊 任务分类体系

### 复杂度评估维度

| 维度 | 简单 (0 分) | 中等 (1 分) | 复杂 (3 分) |
|------|-----------|-----------|-----------|
| **时间跨度** | <1 天 | 1-7 天 | >7 天 |
| **步骤数量** | ≤2 步 | 3-5 步 | >5 步 |
| **知识深度** | 表面查询 | 理解应用 | 系统掌握 |
| **资源需求** | 单一来源 | 多来源 | 跨领域整合 |

### 执行决策

```
总分 ≤ 3  → 简单任务 → 直接执行 ✅
总分 4-6  → 中等任务 → 轻量方法论 ⚠️
总分 > 6  → 复杂任务 → 完整方法论 🔴
```

---

## 📚 方法论库

### 现代方法论

| 方法论 | 适用场景 | 核心步骤 |
|--------|---------|---------|
| **🎓 费曼技巧** | 学习新知识、准备考试 | 概念→教授→回顾→简化 |
| **🔄 PDCA** | 持续改进、质量管理 | Plan→Do→Check→Act |
| **🎯 OKR** | 目标管理、长期规划 | Objectives→Key Results |
| **🚀 Agile/Scrum** | 项目开发、产品迭代 | Sprint→Daily→Review→Retro |
| **💡 设计思维** | 产品创新、问题解决 | Empathize→Define→Ideate→Prototype→Test |
| **✅ GTD** | 任务管理、时间管理 | Capture→Clarify→Organize→Reflect→Engage |

### 中国古代方法论

| 方法论 | 出处 | 适用场景 | 核心理念 |
|--------|------|---------|---------|
| **格物致知** | 《大学》 | 研究学习、知识探索 | 探究事物→获取知识 |
| **知行合一** | 王阳明心学 | 实践应用、技能转化 | 知是行之始，行是知之成 |
| **循序渐进** | 《论语》 | 系统学习、知识构建 | 基础→进阶→精通 |
| **温故知新** | 《论语》 | 记忆巩固、知识创新 | 复习旧知→获得新理解 |
| **学以致用** | 传统治学 | 技能培养、能力提升 | 学→习→用→精 |

---

## 🚀 快速开始

### 安装

```bash
# 使用 ClawHub 安装
npx clawhub@latest install methodology-matcher

# 或手动安装
git clone https://github.com/GIS-blackCaat/methodology-matcher.git
cp -r methodology-matcher/skills/methodology-matcher ~/.openclaw/skills/
```

### 使用

```
# 复杂任务前调用
用户：我想系统学习计算机 408 考研知识

系统分析：
- 时间跨度：6 个月 → 复杂 🔴
- 步骤数量：>10 步 → 复杂 🔴
- 需要系统规划：是 → 复杂 🔴

推荐方法论：
1. 费曼技巧（核心学习方法）
2. 循序渐进（知识构建顺序）
3. 温故知新（定期回顾）

配置：
- 每日推送：概念→教授→回顾循环
- 每周回顾：艾宾浩斯遗忘曲线
- 每月模拟：真题测试 + 错题整理
```

---

## 📋 使用示例

### 示例 1：408 考研备考（复杂任务）

```
任务：我想备考计算机 408 考研

分析：
- 时间跨度：6 个月 → 3 分
- 步骤数量：>10 步 → 3 分
- 知识深度：系统掌握 → 2 分
- 资源需求：跨领域整合 → 2 分
总分：10 分 → 复杂任务 🔴

推荐方法论：
1. 费曼技巧（核心学习方法）
2. 循序渐进（知识构建顺序）
3. 温故知新（定期回顾）

推送配置：
- 每日：概念卡片 + 教授输出 + 回顾简化
- 每周：真题测试 + 错题整理
- 每月：模拟考试 + 知识体系回顾
```

---

### 示例 2：竞品分析（中等任务）

```
任务：分析一下 TCL 和三星在印度市场的竞争

分析：
- 时间跨度：3 天 → 1 分
- 步骤数量：4 步 → 1 分
- 知识深度：理解应用 → 1 分
- 资源需求：多来源 → 1 分
总分：4 分 → 中等任务 ⚠️

推荐方法论：
- PDCA 简化版（Plan→Do→Check）

推送配置：
- 第 1 天：Plan（确定分析框架）
- 第 2 天：Do（收集数据、分析）
- 第 3 天：Check（总结报告）
```

---

### 示例 3：查天气（简单任务）

```
任务：北京今天天气怎么样？

分析：
- 时间跨度：<1 天 → 0 分
- 步骤数量：1 步 → 0 分
- 知识深度：表面查询 → 0 分
- 资源需求：单一来源 → 0 分
总分：0 分 → 简单任务 ✅

执行方式：直接调用 weather skill
无需方法论
```

---

## 🔧 配置说明

### 默认配置

```yaml
methodology:
  default: feynman              # 默认费曼技巧
  enable_for_complex: true      # 复杂任务启用
  allow_user_override: true     # 允许用户覆盖
  auto_detect_complexity: true  # 自动检测复杂度
  
# 方法论选择
methodologies:
  learning: feynman + 循序渐进   # 学习类
  project: scrum + PDCA          # 项目类
  goal: okr + pdca              # 目标类
  innovation: design_thinking   # 创新类
  knowledge: 格物致知 + 温故知新  # 知识体系
```

---

## 📊 复杂度评分算法

```python
def calculate_complexity(task):
    score = 0
    
    # 时间跨度 (0-3 分)
    if task.duration < 1:
        score += 0
    elif task.duration < 7:
        score += 1
    else:
        score += 3
    
    # 步骤数量 (0-3 分)
    if task.steps <= 2:
        score += 0
    elif task.steps <= 5:
        score += 1
    else:
        score += 3
    
    # 知识深度 (0-2 分)
    if task.depth == "surface":
        score += 0
    elif task.depth == "understand":
        score += 1
    else:
        score += 2
    
    # 资源需求 (0-2 分)
    if task.resources == 1:
        score += 0
    elif task.resources <= 3:
        score += 1
    else:
        score += 2
    
    # 判断复杂度
    if score <= 3:
        return "simple"
    elif score <= 6:
        return "medium"
    else:
        return "complex"
```

---

## 📁 文件结构

```
methodology-matcher/
├── SKILL.md                  # 技能说明（必需）
├── README.md                 # 本文件
├── LICENSE                   # MIT 许可证
└── .gitignore                # Git 忽略文件
```

---

## 🎯 应用案例

### 案例 1：系统学习

```
场景：学习新产品经理知识
任务类型：复杂 🔴
方法论：费曼技巧 + 循序渐进
周期：45 天
推送：每日概念卡片 + 教授输出 + 实战练习
```

### 案例 2：项目构建

```
场景：搭建技术博客系统
任务类型：复杂 🔴
方法论：Agile/Scrum + PDCA
周期：2 周
Sprint: 14 天
每日站会：进度同步
评审会：功能演示
```

### 案例 3：长期目标

```
场景：减肥计划
任务类型：复杂 🔴
方法论：OKR + PDCA
周期：3 个月
Objectives: 减重 10kg
Key Results: 每周运动 3 次、每日热量控制
每周回顾：进度跟踪
```

---

## 🔄 版本历史

### v1.0.0 (2026-03-08)

**初始版本**：
- ✅ 任务复杂度自动检测
- ✅ 现代方法论库（6 种）
- ✅ 中国古代方法论库（5 种）
- ✅ 自动匹配推荐
- ✅ 用户配置接口

---

## 🤝 贡献

欢迎贡献！请查看贡献指南。

### 贡献方式

1. Fork 本仓库
2. 创建功能分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启 Pull Request

---

## 📄 许可证

MIT License - 查看 [LICENSE](LICENSE) 文件

---

## 🔗 相关链接

- **OpenClaw 官方文档**: https://docs.openclaw.ai
- **ClawHub**: https://clawhub.com
- **黑猫技术博客**: https://gis-blackcaat.github.io/
- **相关 Skill**:
  - [domain-mentor](https://github.com/GIS-blackCaat/domain-mentor) - 领域学习导师
  - [chat-memory-keeper](https://github.com/GIS-blackCaat/chat-memory-keeper) - 群聊记忆管家

---

## 📞 联系方式

- **GitHub**: [@GIS-blackCaat](https://github.com/GIS-blackCaat)
- **博客**: https://gis-blackcaat.github.io/

---

**最后更新**: 2026 年 3 月 8 日  
**维护者**: 黑猫 🐈‍⬛
