# AGENTS.md

Guidance for AI agents working in this repository.

## What this repo is

- **`c0202-bg.short-intro-to-stem`** — sample **handbook** for teaching the learner course **Кратък увод в STEM** (`C0102-BG`).
- **Course:** `C0202`. Language: **BG**.
- Educator tracks **`V21`** / **`V22`** are teacher handbooks for how to teach those two learner groups (**`V21`** → начинаещи читатели **`V11`**, **`V22`** → по-млади читатели **`V12`**), not a separate content path. There is no **`V23`** until `C0102` has a deeper learner track.

## Canonical spec

Authoritative layout rules: **`../../tcams/tcams-docs-shared`** (**STRUCTURE.md** wins on conflict).

## Content authoring (match C0042 / C2121)

- **Pairing:** each handbook track teaches the matching learner pages. Do not add extra science the learner pages do not use. In delivered prose, name the groups in plain words (начинаещи читатели, по-млади читатели) — do not expose `Vxy` codes.
- **Typed topics:** short chain with YAML **`topic_type`**: **`problem`**, **`info`**, **`assignment`**. Typical order: problem → info → assignment. A fourth topic may close the lesson (still typed). Do not put those words in **`tags`** — keep **`tags: []`** unless SEO keywords are added.
- **Keep handbook topics very short:** usually one paragraph, then a **`::: helper`** … **`:::`** aside. Helper text is for the teacher while they talk.
- **Lesson intros:** two or three sentences naming the group and reminding Проблем, Инфо, Задача. Do not write a second essay.
- **No Markdown tables** for teaching flow.
- Unset **`layout_type`** uses the Handbooks default **`stack`**.
- Do not put raw ids or level codes in reader-facing prose.

## Content images

Use the **same art and files** as `c0202-en.short-intro-to-stem`. Do not invent a separate Bulgarian visual style. When replacing a topic image here, copy the matching JPG from the English handbook (same lesson/media filename).

- Topic illustrations: **1920×960** (2:1) JPG. Markdown: `![descriptive alt](media/filename.jpg)`.
- **Do not touch** `media/course-cover.jpg` or `media/course-badge.jpg` unless explicitly asked.
- Leave the older **1376×768** photos in place unless asked to replace them. Do **not** use those older handbook files as style references.
- Full style and the copy-paste generation prompt: **`c0202-en.short-intro-to-stem/AGENTS.md`** (Content images). That look matches the learner course in `c0102-en.short-intro-to-stem/AGENTS.md`.

## Validation

```bash
bash tools/validate.sh /path/to/c0202-bg.short-intro-to-stem
```
