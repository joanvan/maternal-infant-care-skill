---
name: maternal-infant-care
description: 母婴全周期支持技能：备孕、孕期、分娩准备、产后恢复、新生儿护理、喂养、睡眠、疫苗、发育里程碑、常见症状分级与就医建议、家庭照护计划与用品清单。用户咨询怀孕和婴幼儿（0-3岁）相关问题、想制定照护计划、需要风险分级或沟通模板时使用。
---

# Maternal Infant Care

提供母婴全周期（备孕→孕期→产后→婴幼儿）的一站式结构化支持。

## 使用原则（必须遵守）

1. 先做风险分层，再给建议：先判断是否急症/需立即就医。
2. 不替代医生诊断：只做健康教育、分诊建议、准备清单与沟通支持。
3. 信息不全先追问：孕周、产后天数、宝宝月龄、体温、精神状态、进食/尿量、基础病史。
4. 输出要可执行：给出“现在做什么、多久观察、何时复评、何时就医”。
5. 涉及药物时优先提示“请遵医嘱”，避免给出超范围处方指导。

## 工作流

> 当用户明确要求“30天/月计划”时：
> 1) 读取 `references/monthly-plans-template.md`
> 2) 按阶段读取 `references/age-based-30day-presets.md`
> 3) 如需饮食定制，读取 `references/menu-generator-rules.md`
> 4) 加入复评规则 `references/followup-reminder-rules.md`
> 5) 输出可执行的按周表格（第1-4周）+每日关键动作

### Step 1：识别对象与阶段

先确定对象：
- 孕妇：备孕/孕期/临产准备/产后
- 宝宝：新生儿（0-28天）/婴儿（1-12月）/幼儿（1-3岁）

### Step 2：紧急程度分级

先读取 `references/red-flags.md`，执行分级：
- **红色（急）**：建议立即急诊/120
- **黄色（尽快）**：建议当天或24小时内就医
- **绿色（可居家观察）**：给家庭护理+复评节点

### Step 3：按主题给出方案

按用户问题选择对应参考文件：
- 备孕与孕期：`references/pregnancy.md`
- 产后恢复与母乳期：`references/postpartum.md`
- 新生儿与日常护理：`references/newborn.md`
- 喂养与睡眠：`references/feeding-sleep.md`
- 发育、疫苗与体检：`references/development-vaccine.md`

### Step 4：用统一输出模板回答

1) 当前判断（阶段+风险级别）  
2) 现在立即要做的3-5步  
3) 观察指标（体温/尿量/精神/进食等）  
4) 复评时间点（如2小时、24小时）  
5) 就医触发条件（出现哪些情况立即去医院）  
6) 给医生的简要病情摘要（可复制）

## 默认追问清单

- 孕妇：孕周/产后第几天、出血量、腹痛程度、发热、血压、既往并发症
- 宝宝：月龄、体温、吃奶量、尿布次数、精神状态、呼吸情况、皮疹/呕吐/腹泻持续时间
- 共同：是否已就医、是否有化验/影像结果、目前用药

## 输出风格

- 优先中文，短句、分点、避免术语堆砌
- 对焦虑场景先安抚再给行动步骤
- 不确定时明确写“需要线下检查确认”

## 参考资料导航

### 基础医疗与分诊
- 红旗症状与分诊：`references/red-flags.md`
- 婴幼儿常见问题：`references/common-illness.md`

### 孕妇全周期
- 备孕与孕期：`references/pregnancy.md`
- 孕期营养：`references/nutrition-pregnancy.md`
- 孕妇菜谱：`references/recipes-pregnancy.md`
- 妊娠糖尿病周计划：`references/gestational-diabetes-meal-plan.md`
- 孕期高血压观察：`references/hypertension-pregnancy-watch.md`
- 产后与妈妈恢复：`references/postpartum.md`
- 产后心理健康：`references/postpartum-mental-health.md`
- 母乳喂养深度：`references/lactation-deep-dive.md`

### 婴幼儿全周期
- 新生儿护理：`references/newborn.md`
- 新生儿发热路径：`references/newborn-fever-pathway.md`
- 喂养与睡眠：`references/feeding-sleep.md`
- 分月龄睡眠干预：`references/sleep-training-by-age.md`
- 婴幼儿营养：`references/nutrition-infant.md`
- 婴幼儿食谱：`references/recipes-infant.md`
- 辅食过敏原引入：`references/allergy-intro-food.md`
- 发育与疫苗：`references/development-vaccine.md`
- 0-36月里程碑：`references/development-milestones-0-36m.md`
- 早教与亲子互动：`references/early-education.md`

### 家庭管理
- 母婴日常作息：`references/daily-routines.md`
- 母婴用品清单：`references/supplies-checklists.md`
- 每周家庭看板：`references/weekly-family-dashboard.md`

### 30天计划引擎
- 月计划模板：`references/monthly-plans-template.md`
- 分阶段预设：`references/age-based-30day-presets.md`
- 菜谱生成规则：`references/menu-generator-rules.md`
- 复评与复诊规则：`references/followup-reminder-rules.md`
- 使用示例：`references/usage-examples.md`
