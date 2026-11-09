# 新生入学适应计划示例

## 典型场景

8岁学生第一次参加线下集体英语课，家长担心分离和课堂参与。

## 具体示例

系统生成开课前参观、第一课座位与伙伴安排、家长接送确认和一周观察记录，不推断学生心理诊断。

## 脱敏输入示例

```json
{
  "contract_version": "1.2.0",
  "data_status": "confirmed",
  "contains_sensitive_data": false,
  "requested_output_language": "zh-CN",
  "student_age": "学生年龄或年级已核对（脱敏示例）",
  "program_and_class": "课程与班型已核对（脱敏示例）",
  "start_date": "2026-11-10",
  "logistics": "到校与设备信息已核对（脱敏示例）",
  "learning_history": "学习经历摘要已核对（脱敏示例）",
  "parent_concerns": [
    {}
  ],
  "staff_assignments": [
    {}
  ],
  "campus_rules": [
    {}
  ]
}
```

## 预期处理

1. 运行输入契约校验。
2. 逐项核对输入来源、版本和口径。
3. 按`references/PROFESSIONAL_PLAYBOOK.md`完成专业分析。
4. 输出新生适应计划、第一课流程、风险升级条件等核心成果。
5. 由业务负责人确认输入事实、关键假设和最终成果适用范围后才可作为正式业务结论。

## 不应出现的输出

- 虚构政策、价格、人员、课程或客户事实。
- 以“暂无”“待完善”等占位文本冒充完成。
- 无依据的确定性判断或伪造人工签批。
