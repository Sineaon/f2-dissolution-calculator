# f2-dissolution-calculator
溶出曲线相似性 f₂ 计算 Excel 模板 / f2 Similarity Factor Calculator for Dissolution Profiles
# 溶出曲线 f₂ 相似因子计算模板

📊 **免费 Excel 模板，适用于制剂研发人员及药学专业学生**

## 功能介绍

- 输入各时间点参比制剂（Rt）与受试制剂（Tt）平均溶出量，自动计算 f₂ 值
- **标准 f₂**：按法规要求，超过 85% 溶出量的时间点最多纳入 1 个
- **扩展 f₂**：可手动选择纳入全部时间点或指定最多纳入点数，便于对比分析
- 自动绘制溶出曲线对比图（含 0 分钟起始点）
- 自动输出相似性判定结果（f₂ ≥ 50 判定为相似）

## 计算公式

$$f_2 = 50 \times \lg\left\{\left[1 + \frac{1}{n}\sum_{t=1}^{n}(R_t - T_t)^2\right]^{-0.5} \times 100\right\}$$

## 使用方法

1. 下载 `f2_dissolution_template.xlsx`
2. 在蓝色底色单元格填入时间点、参比溶出量（Rt）、受试溶出量（Tt）
3. 结果区自动显示 f₂ 值与判定结论，右侧自动生成溶出曲线图

## 判定标准

| f₂ 值 | 判定结果 |
|-------|---------|
| ≥ 50 | 溶出曲线相似 ✅ |
| < 50 | 溶出曲线不相似 ❌ |
| 特殊情形 | 15 min 时两曲线均值均 ≥ 85%，直接判定相似 |

## 参考依据

- 国家药品监督管理局《普通口服固体制剂溶出曲线测定与比较指导原则》
- FDA Guidance: *Dissolution Testing of Immediate Release Solid Oral Dosage Forms*

## License

MIT License — 自由使用、修改与分发
