# 个人 Agent Skills

这里收录四个用于 Codex 的技能，覆盖中文写作、专利调研、学术检索和 HTML 幻灯片制作。

| 技能 | 用途 | 来源 |
| --- | --- | --- |
| [`natural-chinese-writing`](skills/natural-chinese-writing/SKILL.md) | 润色中文报告和组内材料，按要求保留原文、术语和证据，统一 Word 正文、表格和公式格式。 | 个人工作流。外部写作参考见[来源说明](skills/natural-chinese-writing/references/external-adoption.md)。 |
| [`cnipa-patent-workflow`](skills/cnipa-patent-workflow/SKILL.md) | 编写 CNIPA 检索式，筛选题录，核验全文并分类归档。 | 个人工作流。用 `$cnipa-patent-workflow` 显式调用。 |
| [`academic-search`](skills/academic-search/SKILL.md) | 学术检索前先判断研究阶段。问题还不明确时，先读已有材料，形成具体问题，再用补充检索和 Zotero 注释推进下一轮。 | 基于 [ustc-ai4science/academic-search](https://github.com/ustc-ai4science/academic-search) 的本地 `1.2.2` 改版，保留[原 MIT 许可证](skills/academic-search/LICENSE)。 |
| [`frontend-slides`](skills/frontend-slides/SKILL.md) | 创作固定 16:9 的单文件 HTML 幻灯片，或将 PPT/PPTX 转为网页。单文件可以按需引用在线字体、图片和 CDN。 | 基于 [zarazhangrui/frontend-slides](https://github.com/zarazhangrui/frontend-slides) 的改版，收窄了触发范围并调整了单文件交付规则。保留[原 MIT 许可证](skills/frontend-slides/LICENSE)。 |

## 在 Codex 中使用

克隆本仓库，把所需的 `skills/<名称>/` 整个目录复制到目标项目的 `.agents/skills/`，然后在 Codex 中输入 `$<名称>` 选择技能。需要跨项目使用时，可以放到用户目录的 `.agents/skills/` 下。对于已安装的同名技能，先确认要使用的版本。`academic-search` 的脚本从其技能目录运行。

```bash
git clone https://github.com/luojiafish/personal-skills.git
```
