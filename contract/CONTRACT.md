# 输入输出契约

## 输入字段

| 键 | 名称 | 类型 | 必填 |
|---|---|---|---|
| `student_age` | 学生年龄或年级 | string | 是 |
| `program_and_class` | 课程与班型 | string | 是 |
| `start_date` | 开课日期 | string | 是 |
| `logistics` | 到校与设备信息 | string | 是 |
| `learning_history` | 学习经历摘要 | string | 否 |
| `parent_concerns` | 家长关注点 | array | 否 |
| `staff_assignments` | 教师与教务安排 | array | 是 |
| `campus_rules` | 校区规则 | array | 是 |

## 状态

- `completed`：核心成果完整，关键结论人工确认要求满足。
- `completed_with_limits`：至少一项实质成果，说明限制、已完成和受阻范围。
- `needs_input`：必填字段缺失。
- `needs_confirmation`：资料冲突或人工确认未完成。
- `failed`：计算或工具失败。

## 输出

- `新生适应计划`：结构化条目数组，不允许空壳或占位文本。
- `家长知情清单`：结构化条目数组，不允许空壳或占位文本。
- `第一课流程`：结构化条目数组，不允许空壳或占位文本。
- `教师观察表`：结构化条目数组，不允许空壳或占位文本。
- `回访节点`：结构化条目数组，不允许空壳或占位文本。
- `风险升级条件`：结构化条目数组，不允许空壳或占位文本。

完整机器契约见`contract/input.schema.json`、`contract/output.schema.json`和`contract/runtime_contract.json`。
