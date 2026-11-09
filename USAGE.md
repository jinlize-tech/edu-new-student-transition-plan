# 使用说明

## 适用任务

8岁学生第一次参加线下集体英语课，家长担心分离和课堂参与。

## 准备输入

学生年龄段、课程与班型、开课日期、交通/设备、学习经历、家长关注点、教师安排、机构规则。使用前先脱敏姓名、联系方式和与任务无关的敏感信息。

## 操作步骤

1. 确认目标与边界
2. 生成入学前资料
3. 设计第一课适应任务
4. 分配家长/教师动作
5. 设置观察与回访节点
6. 输出首月复盘表

## 校验命令

```powershell
node scripts/validate_input.js examples/typical_input.json
node scripts/validate_output.js examples/typical_output.json
```

## 状态使用

- `completed`：核心成果完整。
- `completed_with_limits`：只完成可验证部分，并说明受阻范围。
- `needs_input`：缺少关键输入。
- `needs_confirmation`：资料冲突或需人工确认。
- `failed`：工具或计算失败，提供恢复动作。

## 人工确认

业务负责人复核输入事实、关键假设和最终成果适用范围后，成果才可进入正式业务使用。
