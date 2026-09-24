# 可打印 3D 建模 Skill

将照片、平面图、草图、标志图或现有模型转化为经过审核的 3D 打印设计，并交付 STEP、3MF 和最终模型 PNG 预览。

## 一句话安装

把下面这句话发给 Codex：

```text
帮我安装这个 Skill：https://github.com/TheAatroxking1/ai-agent-developers-workflow-skill/tree/main/building-printable-3d-models
```

安装完成后，在下一条消息中即可使用。若当前网络无法下载 GitHub ZIP，可让 Codex 改用 Git 模式重试。

## 使用方法

```text
$building-printable-3d-models

以附件图片为原型制作可 3D 打印模型，最终需要 STEP、3MF 和 PNG 预览图。
```

也可以直接描述需求；当请求涉及参考图、现有模型、STEP、3MF 或可打印 CAD 时，Codex 可以自动匹配此 Skill。

## 工作流程

1. **阶段一：原型图**——确认视觉规格和计划，使用 ImageGen 生成一张仅保留物体、去除背景、手绘风格的 3D 原型图，并等待用户明确审核。
2. **阶段二：制造模型**——收集尺寸、厚度、孔位、公差和打印约束，审批规格与计划后建立参数化 CAD，验证并交付一个 STEP、一个 3MF 和一个由最终制造几何渲染的 PNG。

已交付版本不会被静默覆盖；外观变化返回阶段一，尺寸或制造参数变化返回阶段二。

## 环境与依赖

- 需要可用的 ImageGen 图像生成能力。
- 需要能够创建并导出 STEP、3MF 的 CAD 工具或运行环境；本仓库不捆绑 FreeCAD、CadQuery 或其他 CAD 引擎。
- Skill 会引用 `$test-driven-development` 和 `$verification-before-completion`。目标 Codex 环境未安装这些辅助 Skill 时，需要安装它们或执行等效的测试与交付验证。

## 仓库结构

```text
building-printable-3d-models/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── parameter-checklist.md
    └── verification-checklist.md
```

该 Skill 已通过官方结构校验和契约测试，并已使用 Git 模式完成远程安装验证。

## 许可证

本仓库目前未提供许可证。
