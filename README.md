# 小红书对标账号筛选 Skill

这是一个给创作者和内容运营者用的开源轻量 Skill：当你想找小红书 / RedNote 对标账号时，它不会随便给你一堆“看起来很厉害”的大号，而是帮你筛出真正适合学习的账号。

很多人找对标账号时最容易踩三个坑：

- 找到的是很久不更新的账号，已经没有当前参考价值。
- 找到的是几十万、几百万粉的大号，普通创作者学不了。
- 只看到一条爆过的内容，就误以为整个账号都值得学习。

这个 Skill 解决的就是这个问题：它会先判断账号是否还在更新、赛道是否接近、阶段是否匹配、近期有没有可观察的高表现内容，再把结果分成 `主对标账号`、`相邻参考账号`、`单条内容样本` 和 `暂不推荐`。

## 你下载后可以用它做什么

- 找 3-5 个真正值得学习的小红书 / RedNote 对标账号。
- 按粉丝区间筛选同阶段账号，比如 1000-5000、5000-3w、5w-15w。
- 过滤断更账号、过大账号、不可模仿账号、只有单条内容偶然表现好的账号。
- 判断每个账号具体能学什么：标题、封面、内容结构、更新节奏、评论需求、商业入口。
- 标出哪些地方不能照搬：人设、经历、城市、资源、产品、粉丝基础。
- 把“找对标账号”变成一个可复用的判断流程，而不是凭感觉收藏一堆链接。

## 适合谁

- 刚开始做小红书，不知道该看哪些账号的新手。
- 已经发了一段时间，但不知道自己和同赛道账号差在哪里的创作者。
- 想找同粉丝区间、同赛道、同城市、同内容形式参考账号的运营者。
- 给客户做账号分析、赛道观察、内容规划的人。
- 想让 Agent 帮自己做公开账号研究，但不希望输出一堆泛泛而谈名单的人。

## 为什么这个 Skill 值得单独装

普通搜索只会告诉你“这些账号看起来相关”。这个 Skill 更关心“你能不能学”。

它会强制检查：

1. 账号是不是还在更新。
2. 账号阶段是否和你接近。
3. 有没有近期高表现内容，而不是只靠历史爆过。
4. 是否有账号级别的稳定信号，而不是单条内容偶然爆。
5. 你能学的是结构、选题、标题、封面还是评论需求。
6. 哪些部分不适合你学，避免把自己带偏。

## 3 分钟上手

把这个仓库里的 `SKILL.md` 放到你的 Agent Skill 目录，然后这样问：

```text
用 xhs-benchmark-account-finder 帮我找小红书对标账号。
赛道：AI 工具 / 一人公司 / 内容工作流
阶段：希望找 3000-30000 粉之间的账号
形式：图文和录屏教程都可以
目标：想知道哪些账号适合学习标题、封面和内容栏目
```

如果你已经有账号链接或截图，也可以直接给它，让它判断这些账号是不是值得学。

## 你会拿到什么结果

默认输出会包括：

- 推荐账号列表。
- 每个账号的阶段判断。
- 它为什么值得看。
- 它适合学什么。
- 哪些地方不要照搬。
- 它是主对标、相邻参考、单条内容样本，还是暂不推荐。
- 下一步应该继续看哪一类内容。

## 公开版边界

这个开源版只处理你提供的公开信息、链接、截图或手动整理材料。它不登录账号，不读取私密数据，不自动发布，也不承诺涨粉或爆款。它的价值是帮你把“找对标”变成更清楚、更少走弯路的判断流程。

## Search Keywords

English keywords:

`Xiaohongshu benchmark account`, `RedNote competitor research`, `XHS benchmark creator`, `creator account research`, `same stage creator`, `social media competitor analysis`, `benchmark account finder`, `creator workflow`, `AI skill for creators`.

中文关键词：

`小红书对标账号`, `对标博主`, `同赛道账号`, `同级账号`, `竞品账号分析`, `小红书账号研究`, `创作者工具`, `对标账号筛选`, `不要断更账号`.

## Why This Exists


Creators often ask for benchmark accounts, but a bad reference can be worse than no reference. Huge celebrity accounts, stale accounts, and one-off viral notes usually do not help an ordinary creator decide what to publish next.
This Skill turns benchmark discovery into a quality-gated workflow: stage, track, update recency, account-level proof, recent high-performing works, and learnable parts.

## What It Can Do

- up to 3-5 recommended benchmark accounts
- label for each account: main benchmark, adjacent reference, single-note sample, or not recommended
- reason why each account is learnable
- what not to copy
- recent update or proof signals when provided
- next research action

## Best Inputs

- target platform: Xiaohongshu / RedNote
- track, topic, audience, city, or content format
- desired follower range or creator stage
- known accounts the user likes or wants to avoid
- manual profile links, screenshots, or search results
- user goal: growth, saves, leads, sales, ads, or positioning

## Workflow

- Confirm the track, stage, follower range, and platform.
- Filter out stale, oversized, mismatched, or low-proof accounts.
- Prefer active accounts with recent high-performing works.
- Separate account-level references from single-note samples.
- Explain what can be learned and what should not be copied.
- Return a small first-round list, then expand only if the user asks.

## Output Contract

Default output:

1. Scope and assumptions
2. Input reading
3. Main judgment
4. Structured table or checklist
5. Recommended next action
6. Boundary notes

For detailed rules, see `references/workflow-rules.md`.

## Example Prompt

```text
Use $xhs-benchmark-account-finder for this task:
Track: AI tools for solo creators
Follower target: 3k-30k
Format: graphic notes and screen-recording tutorials
Goal: find accounts I can learn from without copying them
```

## Example Output Shape

See `examples/sample-output.md` for a short sample.

## Open-Source Boundary

This standalone open version includes:

- reusable creator workflow instructions
- input and output contracts
- workflow rules
- example output
- Agent metadata
- MIT license

This standalone open version does not include:

- private platform credentials
- automatic publishing
- private analytics connectors
- scraping or monitoring
- guaranteed traffic, growth, sales, or viral outcomes
- copying another creator's content
- internal operating notes or private project context

## Repository Map

- `SKILL.md`: Agent entrypoint and workflow rules
- `agents/openai.yaml`: Agent display metadata
- `references/workflow-rules.md`: detailed workflow and quality rules
- `examples/sample-output.md`: sample input and output shape
- `LICENSE`: MIT license

## Recommended GitHub Description

> Open Skill for finding active, stage-fit Xiaohongshu / RedNote benchmark accounts without recommending stale, oversized, or unlearnable references.

## Suggested GitHub Topics

`benchmark-account`, `competitor-research`, `xiaohongshu`, `rednote`, `creator-tools`, `content-workflow`, `social-media`, `ai-skill`, `open-source`

## License

MIT
