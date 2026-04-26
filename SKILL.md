---
name: wuxi-bd-ppt-playbook
description: Use this skill whenever the user asks to analyze, reverse-engineer, design, outline, or generate a WuXi AppTec-style biopharma BD presentation, market understanding report, target landscaping deck, Singapore-style report, PPT screenshot analysis, target profile, key stakeholder map, enabler/VC mapping, or high-density consulting deck for life-science business development. This skill is especially important when the user provides PPT screenshots, a .pptx deck, company dossiers, investor lists, APAC market notes, or asks to turn research into a WuXi-style deck. It supports both analysis of existing slides and generation of reusable deck blueprints; use the separate pptx skill as well when an actual .pptx file must be read, edited, or created.
---

# WuXi BD PPT Playbook

## Purpose

Use this skill to work in the style of the WuXi AppTec Singapore Market Understanding Report: a high-density, blue, consulting-grade BD deck that moves from market logic to target landscaping to actionable company, enabler, VC, and stakeholder profiles.

The goal is not generic slide design. The goal is to make biopharma market and target research readable, comparable, evidence-aware, and actionable for WuXi-style BD, SMG, strategy, or management audiences.

## Load These References

Load only the files needed for the task:

| Need | Reference |
|---|---|
| Visual rules, palette, layout grammar | `references/style-guide.md` |
| Deck storyline and consulting logic | `references/storyline-blueprint.md` |
| Reusable page templates | `references/page-templates.md` |
| Observed Singapore screenshot patterns | `references/singapore-screenshot-observations.md` |

If the task touches a real `.pptx`, also use the `pptx` skill. If the task requires evidence checking or citations, keep provenance explicit and use appropriate research/source tools.

## Choose The Mode

Start by identifying which mode applies. If the user wants both, run analysis first and generation second.

### Analysis Mode

Use when the user provides screenshots, thumbnails, a deck, or asks to "learn", "analyze", "reverse engineer", "总结风格", "提炼框架", or "沉淀成模板".

Output:

1. `Deck Goal And Audience`
2. `Chapter Logic`
3. `Page Role Table`
4. `Visual System`
5. `Reusable Page Templates`
6. `Evidence And Confidence Gaps`
7. `Reusable Playbook`

Every material observation must be labeled:

- `观察`: directly visible in the screenshots/deck.
- `推断`: analytical inference from visible structure.
- `低置信度`: text or design detail is unclear, cropped, or only partially visible.

Do not convert blurry screenshot text into precise facts unless it is readable. Do not treat the screenshot deck as source verification for company-specific claims.

### Generation Mode

Use when the user asks to create an outline, slide-by-slide plan, market understanding report, target landscape, company profile, enabler/VC map, or a new WuXi-style deck.

Output:

1. `Deck Objective`
2. `Storyline`
3. `Slide-By-Slide Blueprint`
4. `Evidence Input Requirements`
5. `Target Profile Template`
6. `Stakeholder Mapping Template`
7. `Visual Rules`
8. `Open Data Gaps And Assumptions`

If the user asks for an actual `.pptx`, create or edit the file using the `pptx` skill after the blueprint is stable.

## Core Story Logic

Default to this consulting chain:

`Executive Summary -> Country / Market Overview -> Industry Insights -> Target Profile -> Target Enabler / VC -> Appendix`

The reasoning should move from:

1. Why this market matters.
2. Why this market creates BD demand.
3. What constraints shape the opportunity.
4. Which targets are worth attention.
5. Who to contact and how WuXi can enter.
6. What evidence still needs monitoring.

Use conclusion-first slide titles. A good title makes the judgment clear before the reader studies the chart or table.

## Evidence Discipline

This skill handles strategic BD material, so keep the boundary between fact and interpretation clear.

- Do not invent market numbers, company financing, pipeline status, contact identity, or relationship claims.
- For screenshots, separate `观察` from `推断`.
- For sourced research, distinguish direct support from combined inference.
- If a claim needs a source, say what source type is required: official company page, press release, investor announcement, clinical registry, regulator filing, LinkedIn, government agency page, or source workbook.
- If text is not readable, mark it as `低置信度` and do not fill gaps from memory.
- Strategic implications may be inferred, but label them as interpretation and tie them to the visible or sourced evidence.

## Required Target Profile Fields

Every BD target profile should cover at least:

- Organization intro.
- Platform or product focus.
- Pipeline, program, or service stage.
- Financing, partnership, or milestone timeline.
- Core capability.
- Key stakeholders and likely owner of the relationship.
- Potential WuXi entry point.
- Risk or uncertainty.
- Source needs.

For enablers and VCs, adapt fields to:

- Institution role.
- Portfolio or ecosystem reach.
- Decision makers.
- Relationship pathway.
- Evidence of activity in the relevant market.
- BD value to WuXi.

## Output Style

Write in the user's requested language. If unspecified and the prompt is Chinese, write in Chinese.

Use compact consulting prose. Prefer tables for page role maps, slide blueprints, target profiles, and evidence gaps. Avoid generic summaries such as "the deck is professional"; explain the design or logic pattern that makes it work.

When generating deck plans, include page types and visual rules for each slide, not just chapter names.

## Quality Bar

The result is acceptable only if it:

- Recovers or defines the business question and audience.
- Shows the chapter logic, not just a list of slides.
- Reuses WuXi-style visual grammar: blue/gray system, white dense content pages, dark-blue chapter covers, top section tabs, bottom brand bar, blue module headers.
- Produces BD-actionable next steps: priority, entry path, key stakeholder, trigger event, or required source.
- Keeps observation, inference, and evidence gaps visibly separate.
