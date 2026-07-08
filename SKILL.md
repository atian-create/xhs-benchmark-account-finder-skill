---
name: xhs-benchmark-account-finder
description: "Open Skill for finding active, stage-fit Xiaohongshu / RedNote benchmark accounts without recommending stale, oversized, or unlearnable references. Use when the user asks for Xiaohongshu benchmark account, RedNote competitor research, XHS benchmark creator, creator account research, 小红书对标账号, 对标博主, 同赛道账号, 同级账号. This Skill uses user-provided material and public-safe reasoning only; it does not publish automatically, scrape private data, copy creators, or promise growth."
---

# Xiaohongshu Benchmark Account Finder

## Purpose

帮创作者筛选仍在更新、阶段接近、值得学习的小红书 / RedNote 对标账号。

This is a lightweight standalone open Skill. It turns a repeated creator task
into a clear Agent workflow with inputs, checks, output shape, and boundaries.

## Use This For

- up to 3-5 recommended benchmark accounts
- label for each account: main benchmark, adjacent reference, single-note sample, or not recommended
- reason why each account is learnable
- what not to copy
- recent update or proof signals when provided
- next research action

## Do Not Use This For

- automatic publishing
- private account login
- private data extraction
- guaranteed traffic, growth, sales, or viral outcomes
- copying another creator's exact wording, identity, images, or claims
- making claims that the user's material does not support

## Inputs

- target platform: Xiaohongshu / RedNote
- track, topic, audience, city, or content format
- desired follower range or creator stage
- known accounts the user likes or wants to avoid
- manual profile links, screenshots, or search results
- user goal: growth, saves, leads, sales, ads, or positioning

If the input is incomplete, proceed with a first-pass version and mark
assumptions. Ask only the smallest necessary follow-up when the missing detail
would materially change the result.

## Workflow

Read `references/workflow-rules.md` when the task needs the full rule set.

- Confirm the track, stage, follower range, and platform.
- Filter out stale, oversized, mismatched, or low-proof accounts.
- Prefer active accounts with recent high-performing works.
- Separate account-level references from single-note samples.
- Explain what can be learned and what should not be copied.
- Return a small first-round list, then expand only if the user asks.

## Output Contract

```markdown
## 1. Scope And Assumptions

## 2. Input Reading

## 3. Main Judgment

## 4. Working Table Or Checklist

## 5. Recommended Next Action

## 6. Boundaries
```

## Quality Bar

- Be specific and operational.
- Prefer a small usable output over a broad lecture.
- Explain why each recommendation fits the user's material.
- Mark weak evidence instead of pretending certainty.
- Do not promise results.
- Do not copy another creator's protected expression or personal story.

## Tone

Write in the user's language. For Chinese creator tasks, default to clear,
practical Chinese.

## Public Boundary

Keep examples generic. Do not include internal thread IDs, private file paths,
unpublished customer material, private account data, or internal product notes.
