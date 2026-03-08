---
name: methodology-matcher
description: |
  Task methodology matcher for complex long-term projects.
  任务方法论匹配器，为复杂长期任务自动匹配适配的方法论框架。
metadata:
  version: "1.0.0"
  languages: ["zh-CN", "en-US"]
  categories: ["planning", "methodology", "productivity"]
---

# Methodology Matcher / 任务方法论匹配器

[English](#english) | [中文](#中文)

---

## <a id="english"></a>English

### Overview

Before executing complex long-term tasks (domain learning, systematic study, project construction, etc.), this skill automatically matches appropriate methodology frameworks based on task type and complexity.

### Core Philosophy

**Simple Tasks** → Direct Execution
**Complex Tasks** → Methodology Matching → Configuration → Execution

### Task Classification

| Task Type | Complexity | Execution Mode | Examples |
|-----------|------------|----------------|----------|
| **Simple** | Low | Direct | News search, single reminder, quick query |
| **Medium** | Medium | Light methodology | Multi-step research, weekly summary |
| **Complex** | High | Full methodology | Domain learning, systematic study, project build |

### Methodology Library

#### Modern Methodologies

| Methodology | Best For | Core Steps |
|-------------|----------|------------|
| **Feynman Technique** | Learning & Teaching | Concept → Teach → Review → Simplify |
| **PDCA Cycle** | Continuous Improvement | Plan → Do → Check → Act |
| **OKR** | Goal Management | Objectives → Key Results → Tracking |
| **Agile/Scrum** | Project Development | Sprint → Daily → Review → Retro |
| **Design Thinking** | Innovation | Empathize → Define → Ideate → Prototype → Test |
| **GTD** | Task Management | Capture → Clarify → Organize → Reflect → Engage |

#### Chinese Classical Methodologies

| Methodology | Best For | Core Principles |
|-------------|----------|-----------------|
| **格物致知** (Investigation of Things) | Research & Learning | Investigate → Knowledge → Sincerity → Rectification |
| **知行合一** (Unity of Knowledge and Action) | Practice | Knowledge ↔ Action, Theory + Practice |
| **循序渐进** (Step by Step) | Systematic Learning | Foundation → Progress → Mastery |
| **温故知新** (Review Old, Learn New) | Memory & Review | Review → Connect → Innovate |
| **学以致用** (Apply Learning) | Skill Building | Learn → Practice → Apply → Improve |

### Usage

```
# Before complex task
I want to systematically learn computer science for graduate exam

# Skill analyzes and recommends
Task Type: Complex (Systematic Learning)
Recommended Methodology: Feynman Technique + 循序渐进
Configuration: Daily push with concept → teach → review cycle

# Then executes with methodology
```

### Integration

```yaml
# In workflow configuration
pre_execution:
  - skill: methodology-matcher
    config:
      enable_for_complex: true
      default_methodology: feynman
      allow_user_override: true
```

---

## <a id="中文"></a>中文

### 概述

在执行复杂长期任务（领域学习、系统学习、项目构建等）前，本技能根据任务类型和复杂度自动匹配适配的方法论框架。

### 核心理念

**简单任务** → 直接执行
**复杂任务** → 方法论匹配 → 配置 → 执行

---

## 📊 任务分类体系

### 任务复杂度评估

| 维度 | 简单 | 中等 | 复杂 |
|------|------|------|------|
| **时间跨度** | <1 天 | 1-7 天 | >7 天 |
| **步骤数量** | 1-2 步 | 3-5 步 | >5 步 |
| **知识深度** | 表面查询 | 理解应用 | 系统掌握 |
| **资源需求** | 单一来源 | 多来源 | 跨领域整合 |
| **反馈周期** | 即时 | 短期 | 长期迭代 |

### 任务类型分类

#### 1️⃣ 简单任务（直接执行）

| 任务类型 | 示例 | 执行方式 |
|---------|------|---------|
| **信息查询** | 查天气、查新闻、查定义 | 直接调用搜索技能 |
| **单次提醒** | 10 分钟后提醒我 | 直接创建定时任务 |
| **简单计算** | 100*25=？ | 直接计算 |
| **文件操作** | 发送文件、下载图片 | 直接执行 |

**判断标准**：
- ✅ 时间跨度 < 1 天
- ✅ 步骤数量 ≤ 2
- ✅ 无需系统性规划
- ✅ 无需方法论支撑

---

#### 2️⃣ 中等任务（轻量方法论）

| 任务类型 | 示例 | 推荐方法论 |
|---------|------|-----------|
| **多步研究** | 调研竞品、写分析报告 | PDCA 循环 |
| **周期性任务** | 每周总结、月度报告 | GTD 简化版 |
| **短期学习** | 学习一个知识点 | 费曼技巧简化版 |

**判断标准**：
- ⚠️ 时间跨度 1-7 天
- ⚠️ 步骤数量 3-5 步
- ⚠️ 需要一定规划
- ⚠️ 可选轻量方法论

---

#### 3️⃣ 复杂任务（完整方法论）

| 任务类型 | 示例 | 推荐方法论 |
|---------|------|-----------|
| **系统学习** | 408 考研备考、学习新产品经理知识 | 费曼技巧 + 循序渐进 |
| **项目构建** | 搭建博客系统、开发技能 | Agile/Scrum |
| **长期目标** | 减肥计划、职业发展规划 | OKR + PDCA |
| **创新设计** | 新产品设计、营销方案 | 设计思维 |
| **知识体系** | 建立市场营销知识框架 | 格物致知 + 温故知新 |

**判断标准**：
- 🔴 时间跨度 > 7 天
- 🔴 步骤数量 > 5 步
- 🔴 需要系统规划
- 🔴 需要方法论支撑

---

## 📚 方法论库

### 现代方法论

#### 1️⃣ 费曼学习法 (Feynman Technique)

**适用场景**：学习新知识、准备考试、技能掌握

**核心步骤**：
```
1. 选择概念 → 2. 教授他人 → 3. 回顾简化 → 4. 内化应用
```

**配置参数**：
```yaml
feynman:
  concept_card: true      # 概念卡片
  teach_output: true      # 输出教学
  review_cycle: 7         # 7 天回顾
  simplify_ratio: 0.8     # 简化到 80%
```

---

#### 2️⃣ PDCA 循环

**适用场景**：持续改进、质量管理、任务优化

**核心步骤**：
```
Plan(计划) → Do(执行) → Check(检查) → Act(处理)
```

**配置参数**：
```yaml
pdca:
  plan_duration: 1        # 计划 1 天
  do_duration: 5          # 执行 5 天
  check_duration: 1       # 检查 1 天
  act_duration: 1         # 处理 1 天
  cycle_repeat: 4         # 重复 4 轮
```

---

#### 3️⃣ OKR 目标管理

**适用场景**：目标设定、绩效管理、长期规划

**核心结构**：
```
Objectives(目标) → Key Results(关键结果) → Tracking(跟踪)
```

**配置参数**：
```yaml
okr:
  objectives_count: 3     # 3 个目标
  key_results_per_o: 4    # 每个目标 4 个关键结果
  review_frequency: weekly # 每周回顾
  confidence_threshold: 0.7 # 信心指数阈值
```

---

#### 4️⃣ Agile/Scrum 敏捷开发

**适用场景**：项目开发、产品迭代、团队协作

**核心流程**：
```
Sprint 规划 → 每日站会 → Sprint 评审 → 回顾会
```

**配置参数**：
```yaml
scrum:
  sprint_duration: 14     # 14 天一个冲刺
  daily_standup: true     # 每日站会
  review_enabled: true    # 评审会
  retro_enabled: true     # 回顾会
```

---

#### 5️⃣ 设计思维 (Design Thinking)

**适用场景**：产品创新、问题解决、用户体验

**核心步骤**：
```
Empathize(同理心) → Define(定义) → Ideate(构思) → Prototype(原型) → Test(测试)
```

---

#### 6️⃣ GTD 任务管理

**适用场景**：任务管理、时间管理、工作效率

**核心流程**：
```
Capture(收集) → Clarify(理清) → Organize(整理) → Reflect(反思) → Engage(执行)
```

---

### 中国古代方法论

#### 1️⃣ 格物致知

**出处**：《大学》

**适用场景**：研究学习、知识探索

**核心步骤**：
```
格物 (探究事物) → 致知 (获取知识) → 诚意 (真诚意念) → 正心 (端正心态)
```

---

#### 2️⃣ 知行合一

**出处**：王阳明心学

**适用场景**：实践应用、技能转化

**核心理念**：
```
知是行之始，行是知之成
学习 ↔ 实践，理论 + 实战
```

---

#### 3️⃣ 循序渐进

**出处**：《论语》

**适用场景**：系统学习、知识构建

**核心理念**：
```
基础 → 进阶 → 精通
不积跬步，无以至千里
```

---

#### 4️⃣ 温故知新

**出处**：《论语》

**适用场景**：记忆巩固、知识创新

**核心理念**：
```
温故 (复习旧知) → 知新 (获得新理解)
艾宾浩斯遗忘曲线应用
```

---

#### 5️⃣ 学以致用

**出处**：传统治学思想

**适用场景**：技能培养、能力提升

**核心理念**：
```
学 → 习 → 用 → 精
学习的目的是应用
```

---

## 🔧 使用方法

### 基本调用

```
# 复杂任务前调用
我想系统学习计算机 408 考研知识

# 技能分析并推荐
任务类型：复杂（系统学习）
推荐方法论：费曼技巧 + 循序渐进
配置：每日推送概念→教授→回顾循环
```

### 配置示例

```yaml
# 默认配置
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
```

---

## 📋 任务分类决策树

```
开始
  ↓
任务时间跨度？
  ├─ <1 天 → 简单任务 → 直接执行 ✅
  ├─ 1-7 天 → 中等任务 → 轻量方法论 ⚠️
  └─ >7 天 → 继续判断 ↓
  
任务步骤数量？
  ├─ ≤2 步 → 简单任务 → 直接执行 ✅
  ├─ 3-5 步 → 中等任务 → 轻量方法论 ⚠️
  └─ >5 步 → 继续判断 ↓
  
是否需要系统规划？
  ├─ 否 → 简单/中等 → 直接/轻量
  └─ 是 → 复杂任务 → 完整方法论 🔴
  
任务类型？
  ├─ 学习类 → 费曼技巧 + 循序渐进
  ├─ 项目类 → Agile/Scrum + PDCA
  ├─ 目标类 → OKR + PDCA
  ├─ 创新类 → 设计思维
  └─ 知识体系 → 格物致知 + 温故知新
```

---

## 🎯 应用示例

### 示例 1：408 考研备考

```
任务：我想备考计算机 408 考研

分析：
- 时间跨度：6 个月 → 复杂 🔴
- 步骤数量：>10 步 → 复杂 🔴
- 需要系统规划：是 → 复杂 🔴

推荐方法论：
1. 费曼技巧（核心学习方法）
2. 循序渐进（知识构建顺序）
3. 温故知新（定期回顾）

配置：
- 每日推送：概念卡片 → 教授输出 → 回顾简化
- 每周回顾：艾宾浩斯遗忘曲线
- 每月模拟：真题测试 + 错题整理
```

---

### 示例 2：搭建博客系统

```
任务：我想搭建一个技术博客

分析：
- 时间跨度：2 周 → 中等/复杂 ⚠️
- 步骤数量：6 步 → 复杂 🔴
- 需要系统规划：是 → 复杂 🔴

推荐方法论：
1. Agile/Scrum（开发流程）
2. PDCA（持续改进）

配置：
- Sprint: 14 天
- 每日站会：进度同步
- 评审会：功能演示
- 回顾会：改进点
```

---

### 示例 3：查天气（简单任务）

```
任务：北京今天天气怎么样？

分析：
- 时间跨度：<1 天 → 简单 ✅
- 步骤数量：1 步 → 简单 ✅
- 需要系统规划：否 → 简单 ✅

执行方式：直接调用 weather skill ✅
无需方法论
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

## 🔗 相关技能

- **domain-mentor** - 领域学习导师
- **planning-with-files** - 文件化任务规划
- **self-improving-agent** - 自我改进代理

---

**Version**: 1.0.0  
**Author**: 黑猫 🐈‍⬛  
**Created**: 2026-03-08
