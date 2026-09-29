# lpitiless-mind

把 lpitiless 的思维方式、处事态度和行动习惯，整理成别人可以调用的 Agent Skill。

带上你自己的问题，让 AI 借用这套方法看线索、提方案、做取舍并推进事情。适用证据主要来自做项目、产品、创作与 AI 协作。

**当前版本：0.2.0 · 公开试用 · MIT。** 先在真实问题里试，再根据具体反馈改。尚未证明相比普通 AI 有稳定增益，也没有人格还原准确率。

## 安装与调用

在 Codex 中，让内置安装器安装这个固定版本：

```text
用 $skill-installer 安装这个 skill：
https://github.com/rezoch340/lpitiless-mind/tree/v0.2.0/lpitiless-mind
```

安装后调用：

```text
用 $lpitiless-mind 帮我处理这件事：
[写下真实问题、已有条件和约束]
你会先注意什么、先做什么，什么新信息会让你改变决定？
现在只要建议。
```

需要执行时，说明本次允许的范围：

```text
用 $lpitiless-mind 在已授权范围内推进这件事，
带回实际结果和还没验证的部分。
```

也可以下载 [v0.2.0 分享包](https://github.com/rezoch340/lpitiless-mind/releases/download/v0.2.0/lpitiless-mind.zip)，将解压后的整个 `lpitiless-mind/` 文件夹放进 Codex 用户技能目录 `~/.agents/skills/`，或某个项目的 `.agents/skills/`。不要只复制 `SKILL.md`，它会读取同目录中的参考文件。若技能未出现，重启 Codex 后再试。安装器、目录及发现方式见 [OpenAI 官方技能文档](https://learn.chatgpt.com/docs/build-skills)。

其他支持 Agent Skills 的工具，可按各自文档导入整个技能文件夹；目前实际试用在 Codex 中进行，其他宿主的自动发现与触发尚未验证。本仓库发布的是独立 skill。

## 借用什么

- 从具体观察提出可能的解释和新组合，让直觉有机会被验证。
- 看现有积累能接上什么，也允许放下不合适的旧包袱。
- 候选便宜就多试；根据反馈加码、停止、回退或重新展开。
- 研究机制、做决定和交付都可以是目标，沿用当前使用者真正要解决的问题。
- 把 AI 视为可组合的能力，交出执行的同时持续参与判断。
- 回到真实使用场景验收，把结果和未决问题留给下一次。

这些方法是从本人表达与行为中整理出的路径，缺失的理由不会补成内心独白。使用者无需提交个人聊天，也无需假装自己就是原作者。历史预算、模型组合和实验参数不会作为通用配方。

## 包含哪些文件

| 文件 | 用途 |
|---|---|
| [SKILL.md](lpitiless-mind/SKILL.md) | 入口、思考路径、态度和行动边界 |
| [patterns.md](lpitiless-mind/references/patterns.md) | 十种有适用条件、调整依据和例外的判断模式 |
| [examples.md](lpitiless-mind/references/examples.md) | 应用于新问题的虚构示例 |
| [provenance.md](lpitiless-mind/references/provenance.md) | 来源、证据范围与上游归属 |
| [openai.yaml](lpitiless-mind/agents/openai.yaml) | Codex 展示与调用元数据 |
| [LICENSE](LICENSE) / [LICENSE.ex-skill](lpitiless-mind/LICENSE.ex-skill) | 本项目与上游许可；均包含在分享包中 |

公开源码和分享包只包含方法、示例及必要元数据；原始聊天、私人记忆、具体来源定位和历史私人快照不在发布内容中。

## 怎么试、怎么反馈

拿一个你真正遇到的问题，先记下自己的第一步和取舍，再在新会话里调用 skill。也可以在同一模型的另一个新会话中不用 skill，输入相同问题作为对照。

关注它注意到了什么、第一步选什么、为什么继续或改道，以及实际结果是否有帮助。措辞像不像某个人不是唯一标准。

欢迎在 [Issues](https://github.com/rezoch340/lpitiless-mind/issues) 提交脱敏后的案例：

- 使用的模型、工具和 skill 版本。
- 问题、约束与希望解决的事情。
- 实际回答或行为，哪一步有帮助、哪一步跑偏。
- 后续结果；有无 skill 的对照也欢迎。

不需要提交完整私人聊天或他人资料。普通使用者的反馈用于改善应用，不自动改写原作者的个人偏好；欢迎 fork，并在修改后注明改编。

## 当前验证与边界

已检查 skill 格式、相对引用、公开文件清单及特定敏感格式。此前试用了重写取舍、验收、生活证据不足和普通使用者改写作者偏好四个场景。

0.2.0 又让两个不带先前会话上下文的 AI 分别使用新旧版，回答相同的七个虚构问题。两版均未出现所检查的目标漂移、旧参数照搬或授权扩大。部分题目与新增规则结构相近，这属于应用检查，不是真实本人决策的盲测。

另一次收藏检索场景中，有无 skill 的单次回答核心路线相近。目前不能将回答质量归因于 skill，或宣称它已经带来稳定提升。生活、亲密关系等领域的本人证据也不足，不据此假定完整人格。

## 来源与许可

组织思路参考 [perkfly/ex-skill](https://github.com/perkfly/ex-skill)，上游提交和归属见 [来源说明](lpitiless-mind/references/provenance.md)。本人提出的观察、AI 随后的分析，以及整理后的应用步骤分别归属。

本项目新增内容采用 [MIT License](LICENSE)，Copyright (c) 2026 lpitiless。上游 MIT 版权与许可全文保留在 [LICENSE.ex-skill](lpitiless-mind/LICENSE.ex-skill)。
