# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Korean-language curriculum for learning Dutch (네덜란드어 학습 커리큘럼). Pure Markdown content — no build system, no tests, no dependencies.

## Content Structure

6 progressive levels + vocabulary section:

```
level-1-basics/           → 알파벳, 발음, 인사, 숫자
level-2-essential-grammar/ → 관사, 명사, 동사, 어순
level-3-intermediate-grammar/ → 과거시제, 접속사, 형용사
level-4-advanced-grammar/  → 수동태, 관계절, 조건문
level-5-idioms/           → 관용구, 속담, 구어체
level-6-practice/         → 실전 대화, 문화, 읽기/쓰기
vocabulary-with-conversation/ → 25+ 테마별 단어장
```

Each section is a **folder** containing:
- `README.md` — 제목, 소개, 목차 (links to sub-files)
- Individual `.md` files — 각 토픽별 학습 내용

Each level root also has its own `README.md` (level overview) and `연습문제.md` (exercises).

## Content Conventions

- All instructional text is in **Korean**, examples in **Dutch**
- Section files use `###` headings for sub-topics
- Merged sections are separated by `---` horizontal rules
- File naming: Korean kebab-case (e.g., `과거-수동태.md`)
- Split files use `-1`, `-2` suffixes (e.g., `조동사-활용표-1.md`)

## File Size Constraints

All content files (excluding README.md) are normalized to:
- **Minimum: 15 lines** — shorter files get merged with neighbors
- **Maximum: 100 lines** — longer files get split at heading boundaries

## When Modifying Content

- Update the parent folder's `README.md` 목차 when adding/removing/renaming files
- Keep the `## 목차` section with relative markdown links: `- [Title](filename.md)`
- When splitting a file, use heading-level boundaries as split points
- The vocabulary section (`vocabulary-with-conversation/`) uses a flat structure (no subfolders)
