This repo holds weekly English lesson plans ("giáo án") for Phụng Kim, teaching Grade 2 and Grade 3 (Global Success curriculum). Follow this when drafting or editing any `Tuan N - Giao an.docx`.

## Source material — never invent activity content

Per-activity teaching content (objectives, input/pictures, answer keys, procedure steps) already exists in the official sample lesson plans. Always pull from these before writing anything yourself:

- `TA3-Global Success-GIAO AN MAU/Unit N.docx` — Grade 3, one file per unit, each with "Lesson 1 – Period 1/2", "Lesson 2 – Period 3/4", "Lesson 3 – Period 5/6" sections. Also `Review N & Fun time N.docx` for review/fun-time weeks.
- `TA2-Global Success-GIAO AN MAU/Unit N.docx` or `Fun time N.docx` / `Review N.docx` — Grade 2 equivalents.
- `HSKT/` — accommodation wording for named disabled students (`Danh_sach_ma_hoa_chuan_HSKT.docx` maps skill type → accommodation sentence; `HSKT_goc.docx` has the base text). Use this to fill the "For disable student (<names>)" block, not invented wording.
- `LBG/LBG T<week>.docx` — the week's teaching schedule table: which class gets which Unit/Lesson/Period on which date. Cross-reference this to know exactly which Lesson/Period section of the MAU file to pull for a given week.

If a MAU source section is itself a stub (header only, no steps — this happens for some Grade 2 Fun Time activities), it's fine to compose reasonable content, but say so explicitly to the user rather than presenting it as official. Mistake made once already: inventing an "Activity 6. Project" (poster design) for Unit 7 Lesson 3 instead of using the MAU's actual mechanic (write instructions on paper, fold into a box, draw one and act it out) — always check the MAU file first.

## Canonical lesson-plan structure

Confirmed with the user via the reference file `PHỤNG-TA3-TUẦN 12.docx` (hand-edited by them) — apply this to every period in every week's docx:

- `I. OBJECTIVES` — plain paragraphs: lead-in "By the end of this lesson, pupils will be able to:", then `1. Knowledge and skills` (bullets), `2. Competences` (bullets — merge what used to be separate "Core competencies" + "General competencies" into one list), `3. Attributes` (bullets). If the class has an accommodated pupil, append `4. For disable student (<names>)` + its own lead-in + bullets, styled in blue (RGB `4472C4`), sourced from `HSKT/`.
- `II. MATERIALS` — plain bulleted list (book page, audio tracks if any, teacher's guide pages, website, flashcards, computer/projector).
- `III. PROCEDURES` — **one single table** for the whole period. Columns: `TEACHER'S ACTIVITIES | PUPILS' ACTIVITIES | CONTENT`, header row once. Then for Warm-up and each numbered Activity, exactly **3 rows**:
  1. Merged across all 3 columns: the bold activity header (e.g. "2. ACTIVITY 1: EXPLORATION (8 minutes)"), then `a. Objectives` (bold) + bullets, `b. Content` (bold) + bullets, `c. Expected outcomes` (bold) + bullets (+ the blue `*For disable student: ...` line if applicable).
  2. Merged across all 3 columns: just a short title, e.g. "Activity 1. Look, listen and repeat. 8 minutes" or "Warm-up and review".
  3. Normal row, 3 distinct columns: teacher's steps | pupils' steps (a synthesized summary of what pupils do — the MAU source doesn't provide this column, so it must be written) | content/materials used.
  Do **not** add a `d. Organisation` label or an `e. Assessment` section — an earlier draft had both and the user explicitly removed them.
- Final part: `5. FUN CORNER AND WRAP-UP (X minutes)` (or `4. HOME LINK (X minutes)` for non-unit lessons like Fun Time) — plain paragraphs only, no a/b/c breakdown: bold `* Option N: <title>` lines each followed by plain `-` bullets.

When building this, prefer cloning an already-correct period's paragraph/table XML and editing text in place (preserves fonts/bold/color) over hand-authoring new runs from scratch.

## Other repo conventions

- `LBG/LBG T<week>.docx` must stay in sync with the schedule table embedded on page 1 of `Tuan <week> - Giao an.docx` (same table content, both places).
- Grade 3 classes: 3B6, 3B7, 3B8, 3B9, 3B10. Grade 2 classes: 2B7, 2B10 (2B10 alone sometimes gets an extra period, e.g. Fun Time).
