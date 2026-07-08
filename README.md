# XHS Benchmark Account Finder Skill

Open Skill for finding active, stage-fit Xiaohongshu / RedNote benchmark accounts without recommending stale, oversized, or unlearnable references.

中文一句话：帮创作者筛选仍在更新、阶段接近、值得学习的小红书 / RedNote 对标账号。

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
