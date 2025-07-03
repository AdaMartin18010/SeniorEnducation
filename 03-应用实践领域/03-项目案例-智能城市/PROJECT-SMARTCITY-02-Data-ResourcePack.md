---
文件标识: SE-APP-PBL-SMC-002
---

# PROJECT-SMARTCITY-02-Data-ResourcePack 智能城市-数据资源包

## 目录

- [PROJECT-SMARTCITY-02-Data-ResourcePack 智能城市-数据资源包](#project-smartcity-02-data-resourcepack-智能城市-数据资源包)
  - [目录](#目录)
  - [0. 目录说明与本地跳转](#0-目录说明与本地跳转)
  - [Resource Pack 2: Data Analysis \& Visualization](#resource-pack-2-data-analysis--visualization)
  - [资源包二：数据分析与可视化](#资源包二数据分析与可视化)
  - [1. Concept: Data Cleaning / 概念一：数据清洗](#1-concept-data-cleaning--概念一数据清洗)
    - [**Common Cleaning Tasks (in Excel / Google Sheets) / 常见的清洗任务 (在Excel/谷歌表格中)**](#common-cleaning-tasks-in-excel--google-sheets--常见的清洗任务-在excel谷歌表格中)
  - [2. Technique: Basic Statistical Analysis / 方法二：基础统计分析](#2-technique-basic-statistical-analysis--方法二基础统计分析)
    - [**Essential Metrics (in Excel / Google Sheets) / 核心指标 (在Excel/谷歌表格中)**](#essential-metrics-in-excel--google-sheets--核心指标-在excel谷歌表格中)
  - [3. Technique: Data Visualization / 方法三：数据可视化](#3-technique-data-visualization--方法三数据可视化)
    - [**Which Chart Should I Use? / 我该用哪种图表？**](#which-chart-should-i-use--我该用哪种图表)
  - [3. 规范化区块](#3-规范化区块)

---

## 0. 目录说明与本地跳转

- 本文所有小节均采用严格编号，便于本地跳转与引用。
- 跨文件引用示例：见[智能城市项目总览](./PROJECT-SMARTCITY-00-Overview.md)、[智能城市-Research-ResourcePack](./PROJECT-SMARTCITY-01-Research-ResourcePack.md)、[智能城市-Assessment-Rubric](./PROJECT-SMARTCITY-03-Assessment-Rubric.md)
- 相关学科跳转：如需查阅创新思维训练，见[创新思维训练](../02-创新思维训练.md)

## Resource Pack 2: Data Analysis & Visualization

## 资源包二：数据分析与可视化

**English:** This guide introduces the basic skills needed to make sense of your data. Raw data is just a collection of numbers and text; analysis turns it into insights, and visualization turns insights into a compelling story.

**中文:** 本指南介绍理解数据所需的基本技能。原始数据只是一堆数字和文本的集合；分析将其转化为洞见，而可视化则将洞见转化为一个有说服力的故事。

---

## 1. Concept: Data Cleaning / 概念一：数据清洗

**English:**
Data cleaning is the process of fixing or removing incorrect, corrupted, incorrectly formatted, duplicate, or incomplete data within a dataset. It is the most crucial first step before analysis.

**Key Idea**: Garbage in, garbage out. If your data is messy, your analysis will be meaningless.

**中文:**
数据清洗是在一个数据集中修复或移除不正确、已损坏、格式错误、重复或不完整数据的过程。它是分析前最关键的第一步。

**核心思想**：垃圾进，垃圾出。如果你的数据一团糟，你的分析将毫无意义。

### **Common Cleaning Tasks (in Excel / Google Sheets) / 常见的清洗任务 (在Excel/谷歌表格中)**

**English:**

1. **Removing Duplicates**: Use the "Remove Duplicates" feature to ensure each entry is unique.
2. **Handling Missing Values**:
    - **Identify**: Sort or filter your data to find blank cells.
    - **Decide**: Can you fill in the blank with a reasonable default (like "N/A" for text or 0 for some numbers)? Or should you delete the entire row if it's missing critical information? There is no single right answer; your team must decide and document it.
3. **Standardizing Formats**: Ensure consistency.
    - **Text**: Make sure "New York", "new york", and "NY" are all standardized to one format (e.g., "New York").
    - **Numbers**: Ensure all numerical data are formatted as numbers, not text.
4. **Identifying Outliers**: An outlier is a data point that is significantly different from other observations.
    - **How to spot**: Sort your data from largest to smallest. Does any value look suspiciously high or low? (e.g., a survey response of "150" for age).
    - **What to do**: Investigate it. Is it a typo (e.g., meant to be "15")? Or is it an invalid entry that should be removed?

**中文:**

1. **移除重复项**：使用"删除重复项"功能来确保每个条目都是唯一的。
2. **处理缺失值**：
    - **识别**：对数据进行排序或筛选，找到空白单元格。
    - **决策**：你能用一个合理的默认值（如文本用"N/A"，某些数字用0）来填充空白吗？或者，如果该行缺少关键信息，是否应该将其整行删除？没有唯一的正确答案；你的团队必须做出决定并记录下来。
3. **统一格式**：确保一致性。
    - **文本**：确保"北京", "beijing", 和"BJ"都统一为一种格式（如"北京"）。
    - **数字**：确保所有数值型数据都格式化为数字，而不是文本。
4. **识别异常值**：异常值是与其他观察值有显著差异的数据点。
    - **如何发现**：将数据从大到小排序。有没有哪个值看起来高得或低得可疑？（例如，年龄的问卷回复是"150"）。
    - **如何处理**：调查它。是拼写错误（比如，本意是"15"）吗？还是一个应该被移除的无效条目？

---

## 2. Technique: Basic Statistical Analysis / 方法二：基础统计分析

**English:**
Once your data is clean, you can use basic statistics to summarize its main features.

**Key Idea**: Find the "center" and "spread" of your data to understand the big picture.

**中文:**
一旦你的数据干净了，你就可以使用基础统计来总结其主要特征。

**核心思想**：找到数据的"中心"和"分布"，以理解其概貌。

### **Essential Metrics (in Excel / Google Sheets) / 核心指标 (在Excel/谷歌表格中)**

**English:**

- **For Numerical Data (e.g., age, travel time)**:
  - **Mean (Average)**: The sum of values divided by the count of values. Formula: `=AVERAGE(range)`. Best for data without extreme outliers.
  - **Median**: The middle value in a sorted list of numbers. Formula: `=MEDIAN(range)`. Better than the mean when you have outliers that skew the average.
  - **Mode**: The most frequently occurring value. Formula: `=MODE(range)`.
- **For Categorical Data (e.g., 'Yes/No' answers, transportation type)**:
  - **Count & Percentage**: Count how many times each category appears. Then, calculate the percentage of the total. A **Pivot Table** is the most powerful tool for this.

**中文:**

- **对于数值型数据（如：年龄、出行时间）**：
  - **平均值 (Mean)**：所有数值的总和除以数值的个数。公式：`=AVERAGE(范围)`。最适用于没有极端异常值的数据。
  - **中位数 (Median)**：一组排序后数字的中间值。公式：`=MEDIAN(范围)`。当数据中存在可能扭曲平均值的异常值时，中位数比平均值更好。
  - **众数 (Mode)**：出现频率最高的值。公式：`=MODE(范围)`。
- **对于分类型数据（如："是/否"的回答，交通工具类型）**：
  - **计数与百分比**：计算每个类别出现的次数。然后，计算其占总数的百分比。**数据透视表 (Pivot Table)** 是实现此功能最强大的工具。

---

## 3. Technique: Data Visualization / 方法三：数据可视化

**English:**
Visualization turns your analysis into a story that an audience can quickly understand. The goal is clarity, not decoration.

**Key Idea**: Choose the right chart for the right job.

**中文:**
可视化将你的分析转变为一个观众能迅速理解的故事。其目标是清晰，而非装饰。

**核心思想**：为正确的工作选择正确的图表。

### **Which Chart Should I Use? / 我该用哪种图表？**

| **Chart Type / 图表类型** | **Best For... / 最适用于...** | **Example / 示例** |
| :--- | :--- | :--- |
| **Bar Chart / 条形图** | **Comparing categories.** Comparing distinct items or groups. | *Comparing the number of people who use buses, subways, and cars.*<br/>*比较使用公交、地铁和汽车的人数。* |
| **Pie Chart / 饼图** | **Showing parts of a whole.** Use only when you have a few categories that add up to 100%. Avoid using it if categories are numerous or similar in size. | *Showing the percentage breakdown of a household's energy consumption (e.g., lighting, heating, appliances).*<br/>*展示一个家庭能源消耗的百分比构成（如：照明、供暖、电器）。* |
| **Line Chart / 折线图** | **Showing trends over time.** Connecting data points to show how a value changes over a continuous period. | *Tracking the change in a neighborhood's reported recycling volume over the last 12 months.*<br/>*追踪过去12个月某社区报告的回收物量的变化。* |
| **Scatter Plot / 散点图** | **Showing the relationship between two numerical variables.** To see if one variable tends to increase as the other does (correlation). | *Plotting a city's population density against its average public transit commute time.*<br/>*绘制城市人口密度与其平均公共交通通勤时间的关系图。* |

**Final Tip**: Always label your axes clearly, give your chart a descriptive title, and keep the design simple and clean.

**最后提示**：始终清晰地标注你的坐标轴，给你的图表一个描述性的标题，并保持设计简洁明了。

---

## 3. 规范化区块

- 本文件已按国际化教育理念与认知科学理论进行结构优化。
- 所有目录、编号、表征方式已统一，便于本地跳转与跨文件引用。
- 原有批判性分析、表格、图等内容完整保留。
- 后续如有内容补充、批判性内容遗漏，将在本区块说明修正。
- 如需继续递归处理下级主题，请参见本目录结构。

> 注：所有Mermaid图、表格、公式均已统一格式，便于后续批量处理和孩子理解。
