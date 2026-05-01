# Skill: Convert a Speaking-Topic Pack into IELTS Reading + Listening Teaching Materials

## Purpose

Use this skill when the user uploads a **speaking-topic pack / cue-card pack / speaking question bank** and wants it turned into **classroom-ready IELTS materials** rather than a loose summary of topics.

This skill converts the uploaded source into one or both of the following:

1. **IELTS-style reading package**
   - reading passages
   - reading questions
   - teacher answer version with concise explanations
   - speaking-transfer expressions

2. **IELTS-style listening package**
   - listening scripts / transcripts
   - IELTS-style listening questions
   - teacher answer version with concise explanations
   - standalone transcript document

The source topic can be **any theme**. Do not preset the topic. Always read the uploaded pack first and let the pack determine the thematic range, scene types, and reusable content lines.

---

## When to use this skill

Use this skill when the user asks for tasks such as:

- "根据口语题库生成阅读材料和题目"
- "根据 speaking-topic pack 生成教师版答案"
- "补做同主题听力材料 + 仿 IELTS 听力题"
- "把口语文档转成阅读 / 听力课堂材料"
- "输出 student version / teacher version / transcript"
- "导出 DOCX / PDF / ZIP"

This skill is especially useful when the user wants materials that do **both** of the following:

- stay tightly linked to the uploaded speaking-topic pack
- function as **real IELTS-style input materials**, not just expanded speaking answers

---

## Default assumptions

If the user does not narrow the request, use these defaults:

### Reading default
- create **3 reading passages**
- create **student version** and **teacher version**
- export **DOCX + PDF**
- if multiple files are created, also export **ZIP**

### Listening default
- create **4 IELTS-style listening sections**
- create **40 questions total** (**10 per section**)
- create **student version**, **teacher version**, and **transcript**
- export **DOCX + PDF** for each
- if multiple files are created, also export **ZIP**

### Combined-task default
If the user asks for both reading and listening:
- keep one shared theme cluster
- avoid repeating the exact same subtopic coverage in both packages
- let the listening package cover areas that were not fully exploited in the reading package
- keep the overall teaching line coherent

---

## Non-negotiable workflow

Do not skip steps. Do not jump straight into drafting passages or scripts.

1. **Read the uploaded speaking-topic pack completely.**
2. **Extract the pack's internal structure and teaching line.**
3. **Map topics to suitable reading and/or listening task types.**
4. **Decide the output architecture before writing.**
5. **Draft the texts/scripts to fit the target question types.**
6. **Write questions that are naturally supported by the texts/scripts.**
7. **Produce teacher versions with concise explanations and speaking-transfer language.**
8. **Create separate student / teacher / transcript files as required.**
9. **Invoke skill-ielts-reviewer in Panel Mode** — spawn 3 independent editor sub-agents to audit every question for answer accuracy, paraphrasing quality, distractor plausibility, and technical correctness. Merge findings by consensus (≥2 editors = fix; 3/3 = must fix). Fix all critical issues before delivery.
10. **Run the quality checklist before final output.**

If the result fails the reviewer panel or the checklist, revise the material before returning it.

---

## Stage 1: Analyze the source pack

Before generating anything, build an internal analysis of the uploaded pack.

### Extract from the source
Identify:

- the **main theme cluster**
- the **subtopics** under Part 1 / Part 2 / Part 3 / extension prompts
- the **scene candidates** suggested by the pack
- the **reusable content lines** that could support input-to-output teaching
- the **mother themes** that appear across several prompts

### Look for recurring teaching lines such as
- habits and routines
- past vs present change
- preferences and evaluation
- memory and growth
- social influence
- restrictions and rules
- storytelling
- technology and communication
- attention and distraction
- traditional vs modern media
- decision-making
- cultural judgment
- personal feeling vs wider impact

### Build a conversion map
Sort the source material into the following buckets where relevant:

- suitable for **descriptive reading**
- suitable for **narrative reading**
- suitable for **case-based feature article**
- suitable for **expository / analytical reading**
- suitable for **daily-life listening dialogue**
- suitable for **monologue introduction**
- suitable for **two-person discussion**
- suitable for **lecture / academic listening**

### Important principle
Do not treat each speaking prompt as an isolated prompt.

Instead, identify:
- the **theme cluster**
- the **scene family**
- the **idea family**
- the **language-transfer potential**

The final materials should feel like one coordinated teaching package, not a pile of unrelated mini-tasks.

---

## Stage 2: Decide the material architecture

The architecture must be chosen **before** drafting.

### If the user requests reading materials
Default architecture:

- **Article 1**: easier entry text
- **Article 2**: mid-level text
- **Article 3**: more abstract / denser text

They must belong to the **same theme family**, but differ in:
- perspective
- genre
- discourse structure
- information density

### If the user requests listening materials
Default architecture:

- **Section 1**: everyday-life two-person dialogue
- **Section 2**: monologue
- **Section 3**: two-person discussion
- **Section 4**: lecture / academic monologue

The four sections must feel like a **coherent thematic cluster**, but must also differ in:
- communicative purpose
- speaker relationship
- task demands
- information structure
- cognitive load

### If the user requests both reading and listening
Use the same overarching theme cluster, but distribute the content strategically:

- reading can take the more text-rich, reflective, descriptive, or analytical angles
- listening can take the more scene-driven, process-driven, decision-driven, or lecture-driven angles
- do not simply recycle one passage into one listening script
- cover underused but relevant source prompts in the second package

---

## Reading package specification

## Reading mission
Turn the speaking-topic pack into **classroom-ready IELTS-style reading materials** that also feed later speaking output.

The reading package should not sound like three expanded speaking answers.

It must sound like **real reading material**.

### Required number of passages
Default: **3 passages**

### Passage length
Each passage should usually be **700 to 950 words**, unless the user explicitly requests a shorter length.

The target is to stay broadly close to the length of a single IELTS reading passage.

Do not write short classroom paragraphs of 300 to 500 words.

### Difficulty progression (5-passage system) 
For a 5-passage set, use:
- P1: Band 5.5–6.0 (accessible entry text)
- P2: Band 6.0–6.5  
- P3: Band 6.5–7.0  
- P4: Band 7.0–7.5  
- P5: Band 7.5–8.0

Progression should appear in: vocabulary load, sentence complexity, abstraction level, inference demand, discourse density.

### Genre diversity (mandatory)
All passages in one pack must not share the same genre or narrative voice.

Rules:
- **No more than one passage** may be mainly first-person narrative
- At least **one passage** must be a **third-person observation / case study / feature article**
- At least **one passage** must be an **analytical / expository / academic-style article**
- Acceptable genres: social observation, magazine feature, case study, reflective narrative, expository essay, analytical article, academic analysis, argumentative essay

Avoid:
- All passages written as first-person stories
- All passages with the same paragraph structure
- Passages that read like expanded speaking answers

### Question types and count
Each passage must have **at least 10 questions**. Mix at least 2 different question types per passage.

Acceptable IELTS question types:
- Multiple Choice (single answer)
- Multiple Choice (multiple answers)
- True / False / Not Given
- Yes / No / Not Given
- Matching Headings
- Matching Information
- Sentence Completion
- Summary Completion
- Note / Table / Flow-chart Completion
- Short Answer Questions

Let the passage content determine the best-fitting question types.

### Speaking input mapping
For each passage, explicitly state which speaking topics it provides input for. Include this mapping in the overview page of the document.

### Difficulty progression (3-passage system)
For a 3-passage set:
- **Article 1**: roughly Band 5.5 to 6
- **Article 2**: roughly Band 6.5 to 7
- **Article 3**: roughly Band 7.5 to 8

Difficulty progression should appear in:
- vocabulary load
- sentence complexity
- abstraction
- inference demand
- discourse density

### Genre and perspective diversity
This is mandatory.

Do **not** write all three passages in first person.

#### Hard rule
- **No more than one passage** may be mainly first-person.
- At least **one passage** should be written as a **third-person case / observed scenario / feature article**.
- At least **one passage** should be written as an **expository / analytical / magazine-style article**.

Acceptable passage types include:
- first-person narrative
- third-person narrative
- case-based feature article
- descriptive article
- reflective article
- explanatory article
- analytical article
- social observation article

### What to avoid in reading generation
Avoid:
- three passages that all sound like "I remember..."
- three passages that all read like Part 2 cue-card answers
- identical paragraph structures across all passages
- shallow topic repetition without development
- generic articles that could fit any theme

### Reading question types
Select from the following according to passage fit:

- Multiple Choice
- True / False / Not Given
- Sentence Completion
- Matching Information
- Summary Completion
- Matching Headings

Do not force every type into every passage.

Question type choice should follow what the passage naturally supports.

### Reading question design rules
- keep **question order** natural and close to IELTS expectations
- cover main idea, detail, inference, paragraph function, implication
- avoid trivial questions that only test one repeated keyword
- if needed, revise the passage slightly to improve question quality
- do not make the teacher version do all the interpretive work that the question should already test

### Paragraph labeling for Matching questions
**Critical rule**: Whenever a passage contains **Matching Information** questions ("Which paragraph contains...") or **Matching Headings** questions ("Choose the correct heading for paragraphs..."), **each paragraph must be labeled with a visible letter** at the beginning.

Label format: `[A]`, `[B]`, `[C]` ... placed at the start of each paragraph in the passage text.

Rules:
- Use consecutive letters starting from `[A]`
- Each distinct paragraph gets its own letter
- The letter must appear **in the passage text where the student reads it** — not just in a reference table
- Do **not** write "(not labelled below)" in the question instruction; delete this phrase since labels are now visible
- Do **not** use quoted excerpts from paragraphs as reference in Matching Headings questions (e.g., avoid `Paragraph A ("Every purchase...")`) — with visible labels, students can find the paragraph themselves
- Parapgraphs that are very short (e.g., a one-sentence conclusion) and are **not** referenced by any Matching question may remain unlabeled

### Suggested reading question load
Default: around **10 to 13 questions per passage**

### Student version vs Teacher version
**Strict separation required:**

The **student version** must contain:
- passage text (with paragraph labels where required)
- all questions (with blanks, options, etc.)
- **NO answers, answer keys, hints, or explanations anywhere**

The **teacher version** must contain:
- passage text (same as student version)
- all questions (same as student version)
- correct answers with concise explanations
- clear support for T/F/NG judgments
- brief justification for why incorrect options are wrong when useful
- a **speaking-transfer language** section for each passage

### Speaking-transfer language for reading
For each passage, select a small number of expressions that are:
- natural
- reusable in speaking
- not overly literary
- not too academic
- genuinely teachable

Explain:
- what idea the expression helps express
- which kinds of speaking topics it can transfer to
- why it is more useful than a flat student-like expression

---

## Listening package specification

## Listening mission
Turn the speaking-topic pack into a **full IELTS-style listening package** whose sections really behave like IELTS Listening sections.

Do not write four unrelated scripts.

Do not write scripts first and then force questions onto them.

Scripts and questions must be designed together.

### Required number of sections
Default: **4 sections**
Default total: **40 questions**
Default per section: **10 questions**

### Theme cohesion across the four sections
All sections must belong to the same broad theme cluster drawn from the source pack.

However, the four sections must not feel repetitive.

They should show progression in:
- formality
- abstraction
- density
- task type
- reasoning demand

### Section 1
**Form**: two-person everyday-life dialogue

**Common scene types**:
- enquiry
- booking
- registration
- workshop sign-up
- activity registration
- timetable discussion
- course arrangement
- simple service dialogue (e.g., returns/exchanges at a shop)

**Target question style**:
- form completion
- note completion
- simple table / form logic where truly helpful

**Important rule**:
The fill-in layout for Section 1 should normally be presented as **embedded form / note completion**, not as a wide empty table that hides the answer order.

The student should be able to feel where each blank belongs in the flow of the notes.

**Do not** use a table merely because it looks tidy.

**Speaker rule**:
- dialogue only
- exactly **two speakers**
- no multi-speaker scenes

**Duration target**:
- roughly at least **3 minutes**
- longer is acceptable if the section remains natural and teachable

**Avoid**:
- making the whole section only about time / place / money
- turning it into meaningless clerical detail
- overpacking it with random numbers

### Section 2
**Form**: monologue (one speaker)

**Common scene types** (use these as a guide, do not default to the same one every time):
- **radio programme** — presenter talks about a local event/service/initiative
- **welcome/orientation talk** — e.g., for new members, new students, new volunteers
- **introduction to a facility or service** — e.g., community centre, library, shop
- **talk about a local event** — e.g., a festival, market, workshop series
- **guide talk / tour** — e.g., a guided walk, museum floor guide (when truly appropriate to the theme)
- **announcement** — e.g., about a change in service, new opening hours, etc.

**Critical: vary the scene type across different units.** Do not default to "exhibition guide talk" for every unit's Section 2. Choose the scene type that best fits the theme cluster of the source pack. For example:
- For "Consumption, Objects and Choices": a radio programme about a community sharing initiative
- For "Learning and Skills": an introduction to a science workshop
- For "Relationships": a short talk about a community helping initiative
- For "Technology": a talk introducing a new app or digital service

**Target question styles** (mix and match as appropriate):
- multiple choice (most common)
- matching (e.g., match features to locations, people, or zones)
- map/plan labelling (e.g., label a floor plan, site map, or facility layout)
- note/table completion (less common but acceptable)
- sentence completion

**Core requirement**:
The script must naturally support questions about:
- reason
- purpose
- evaluation
- viewpoint
- contrast
- important information
- priorities
- locations and spatial relationships (if map/plan labelling is used)

**Duration target**:
- roughly at least **3 minutes**

### Section 3
**Form**: two-person discussion

**Common scene types**:
- project planning
- workshop planning
- review and comparison of options
- student discussion about an assignment or presentation
- evaluation of experiences (courses, events, trips)

(Full scenarios list from original — keep as is)

### Section 4
**Form**: academic monologue / lecture

**Common scene types**:
- lecture (most common)
- academic talk / presentation
- structured explanation of a concept or framework

(Full details from original — keep as is)

### Table rule for fill-in sections (Section 1 & 4)
Default preference:
- embedded notes
- short bullet structures
- form-style lines
- sentence-style completion

Avoid:
- wide grid tables that make it unclear where the blank sits in the text logic

Tables may be used only when they improve clarity and still preserve order. They are **not** the default for fill-ins.

---

## File outputs and naming

### File naming convention
Use the following naming pattern to match the existing unit structure:

```
U{number}_{theme}_{skill_type}_{content_type}_{version}.docx
```

Examples:
- `U08_消费与选择_阅读_练习_学生版.docx`
- `U08_消费与选择_阅读_练习_教师版.docx`
- `U08_消费与选择_听力_练习_学生版.docx`
- `U08_消费与选择_听力_练习_教师版.docx`
- `U08_消费与选择_听力_文本脚本.docx`
- `U08_消费与选择_教学材料包.zip`

Where:
- `{number}` = unit number with leading zero (e.g., U00, U01, U08)
- `{theme}` = theme name in Chinese (e.g., 消费与选择, 日常节奏)
- `{skill_type}` = `阅读` or `听力`
- `{content_type}` = `练习` for question sets, `文本脚本` for transcripts
- `{version}` = `学生版` or `教师版`

If the older naming pattern was used (e.g., `consumption_reading_student.docx`), rename to match this convention before delivery.

### DOCX layout requirements
Generated DOCX files must follow Cambridge IELTS paper-style formatting:

**Page setup:**
- A4 paper size
- Margins: top/bottom 2cm, left/right 2.5cm
- Font: Calibri (or similar clean sans-serif)
- Body text size: 11pt
- Line spacing: 1.5

**Document structure:**
- **Overview page** at the beginning with:
  - Theme description in Chinese + English
  - Passage overview table (columns: Passage, Level, Genre, Speaking Topics)
  - Difficulty path indicator
  - Suggested use instructions
- Each passage starts on a **new page** (page break)

**In-text formatting:**
- Main title: 20pt bold centred
- Subtitle: 14pt italic centred, grey (#555555)
- Section headers: 16pt bold
- Subsection headers: 13pt bold
- Body text: 11pt
- Paragraph labels `[A]`, `[B]`, `[C]`... must be **bold** and visible before each paragraph

**Teacher version formatting:**
- Same layout as student version
- Answer indicators in **red bold** (`#CC0000`)
- Answer explanations in **grey italic** (`#777777`, 10pt)
- Speaking-Transfer section at the end of each passage

### PDF generation
Both student and teacher versions must be provided as **both DOCX and PDF**.
- PDF preserves the exact layout for distribution to students
- PDF generation method: use Word \"Save As → PDF\" or a DOCX-to-PDF converter

### Reading package
- `U{number}_{theme}_阅读_练习_学生版.docx`
- `U{number}_{theme}_阅读_练习_学生版.pdf`
- `U{number}_{theme}_阅读_练习_教师版.docx`
- `U{number}_{theme}_阅读_练习_教师版.pdf`

### Listening package
- `U{number}_{theme}_听力_练习_学生版.docx`
- `U{number}_{theme}_听力_练习_学生版.pdf`
- `U{number}_{theme}_听力_练习_教师版.docx`
- `U{number}_{theme}_听力_练习_教师版.pdf`
- `U{number}_{theme}_听力_文本脚本.docx`
- `U{number}_{theme}_听力_文本脚本.pdf`

### Combined bundle
- `U{number}_{theme}_教学材料包.zip`

If the user requests only one package, only generate the files relevant to that package.

---

## Quality checklist before output

Do not deliver until all relevant checks pass.

### Source relevance
- Is the material clearly anchored to the uploaded speaking-topic pack?
- Would the package still make sense if the source theme were different?
- Have you avoided generic filler content?

### Student vs Teacher separation
- Does the student version contain **zero answers, answer keys, or hints**?
- Does the teacher version include **both questions and answers**?
- Are answer explanations concise and useful for classroom use?

### Paragraph labeling checks
- If Matching Information or Matching Headings questions exist, are paragraphs labeled with `[A]`, `[B]`, `[C]`... in the passage text?
- Is "(not labelled below)" removed from instructions?
- Are quoted excerpts removed from Matching Headings question references?

### Reading checks
- Are there **3 passages** by default unless user requested otherwise?
- Are the passages broadly close to IELTS reading length?
- Is there a clear difficulty progression?
- Are the three passages genuinely different in voice and genre?
- Is there **no more than one** mainly first-person passage?
- Do the questions actually match what each passage supports?
- Does the teacher version include useful speaking-transfer expressions?

### Listening checks
- Do the four sections fit IELTS section roles?
- Is Section 2's scene type varied and appropriate for the theme (not defaulting to "exhibition")?
- Are Section 1 and Section 3 exactly **two-speaker dialogues**?
- Does each section support its designated question types naturally?
- Are questions in script order?
- Is there **no T/F/NG**?
- Are Section 1 and Section 4 fill-ins laid out as notes/forms rather than defaulting to wide tables?
- Does the teacher version explain answers briefly but clearly?
- Is the transcript clean and TTS-friendly?

### Package cohesion checks
- If both reading and listening are generated, do they feel like one teaching line?
- Has the listening package covered angles that the reading package did not fully use?
- Is there classroom usability, not just content volume?

### DOCX layout checks
- Does each new passage start on a **separate page**?
- Is there an **overview page** at the beginning (theme description + passage table)?
- Are page margins correct (2cm top/bottom, 2.5cm left/right)?
- Is the font Calibri 11pt for body text?
- Are paragraph labels `[A]`, `[B]` **bold** in the passage?
- Are teacher version answers in **red bold** with **grey italic** explanations?

### PDF checks
- Is a PDF version generated for both student and teacher versions?
- Does the PDF preserve the DOCX layout?

### Final file checks
- student / teacher / transcript are separate when required
- filenames follow the `U{number}_{theme}_{skill_type}_{content_type}_{version}.docx` convention
- DOCX + PDF are **both** generated
- ZIP is included when appropriate (if multiple files)
- the final response gives direct download links

---

## Revision protocol

If the user gives feedback such as:
- "文体太单一"
- "不要全是第一人称"
- "长度要更像雅思"
- "Section 1 和 4 的填空不要做成表格"
- "Transcript 单独输出"
- "教师版多加可迁移表达"
- "听力题型要更贴近 section 结构"
- "段落没有编号不方便匹配"
- "学生版里怎么有答案"
- "Section 2 的场景不对"

then revise the affected files directly rather than rewriting the entire approach from scratch.

Preserve:
- the source theme cluster
- the material architecture
- the file separation logic

Only change what is necessary to fix the user's concern.

---

## Output behavior

When returning the final result:
- clearly say what was produced
- group links by **student / teacher / transcript / zip**
- keep the explanation brief
- do not paste the whole generated content into chat if files were created
- if no files were created, present the output in clean sections

---

## Summary

This skill is not a generic "write some IELTS material" instruction.

It is a **conversion workflow**:

**speaking-topic pack -> theme analysis -> task architecture -> reading/listening generation -> question design -> teacher support -> file packaging**

The generated materials must be:
- tightly linked to the uploaded pack
- structurally appropriate for IELTS
- useful in class
- useful for later speaking output
- clearly formatted
- easy to revise
- correctly named per convention
- properly separated into student/teacher versions
- paragraph-labeled for Matching-type questions
- varied in listening Section 2 scenario types

---

## Appendix A: Question Design Principles (2026-04-30)

These principles were refined through iterative review and must be applied to EVERY question generation or modification.

### A1. MCQ Design — MANDATORY

1. **NEVER test number recall.** Questions like "How much time did the writer spend sitting? A. 5h B. 10h C. 15h D. 2h" are FORBIDDEN.
2. **ALWAYS paraphrase** the stem AND all 4 options. If an option contains the same words as the passage, it's wrong.
3. **Distractors must be plausible.** Every wrong option must reference content actually found in the passage, but in a context that makes it wrong for THIS question.
4. **Options must be parallel** in length, grammatical form, and level of specificity.

Example of GOOD paraphrasing:
- Passage: "ten hours every single day sitting"
- ❌ Bad: "About 10 hours" (direct copy)
- ✅ Good: "He spent the overwhelming majority of his waking hours inactive at a desk"

### A2. Summary Completion — MANDATORY

1. **Must be a coherent paragraph,** NOT isolated sentences each with a blank.
2. Format: a flowing text with numbered blanks integrated into the narrative.
3. Instruction: "Complete the summary below. Choose NO MORE THAN TWO WORDS from the passage for each answer."
4. Answers must appear verbatim in the passage.

### A3. Question Type Diversity — MANDATORY

Each unit (5 passages) should use at least 4 different question types across passages:
- MCQ (single answer, 4-option) — ALL passages
- TRUE/FALSE/NOT GIVEN — at least 3 passages
- Summary Completion — at least 3 passages
- Matching Information — at least 2 passages
- Matching Headings — at least 2 passages

### A4. Question Count — MANDATORY

- Minimum 10 questions per passage. DO NOT reduce question count when modifying.
- Maximum 13 questions per passage.

### A5. Teacher Version — MANDATORY

1. RED BOLD (#CC0000) answers marked ON each question (not just in answer key)
2. Grey italic (#777777, 10pt) explanations for every answer
3. Speaking topic mapping ("Linked Speaking Topics: ...") before each passage
4. Answer Key section after questions with detailed explanations

### A6. DOCX Technical — MANDATORY

1. NEVER use `&apos;` entity — it's not supported by DOCX format. Replace with literal `'` character post-generation.
2. NEVER use `HighlightColor.GREEN` (dark green) — if highlighting, use shading `{type:'clear',fill:'C6EFCE'}`.
3. NEVER modify passage text when applying formatting. Keep original text intact.
4. Always run verification: check XML for correct entity encoding, answer counts, and formatting.

### A7. Modification Protocol

When making ANY changes to existing materials:
1. Read the full original content first (from 过时文档 if needed)
2. Make targeted edits — do NOT regenerate from scratch unless necessary
3. Preserve question count and structure
4. Verify answers remain correct against passage text
5. Run post-generation verification before delivering

The golden rule: **Improve paraphrasing and distractor quality. Never reduce question count. Never remove speaking topic mappings.**

---

## Cross-Reference: skill-ielts-reviewer

This skill generates materials. Quality assurance is handled by the companion skill:

**`skill-ielts-reviewer`** — IELTS Reading Question Reviewer & Editor

Use it after every generation run:
- **Panel Mode** (`--panel`): Spawn 3 independent editor agents to audit all questions
- **Single-review mode**: One editor does a structured review report
- **Consensus merge**: ≥2 editors flag → fix; 3/3 → critical fix

Contains:
- Answer verification logic (T/F/NG, completion, MCQ)
- Question design quality rubrics (paraphrasing, distractors, trivial-detail avoidance)
- Technical checks (&apos; entities, word limits, student/teacher alignment)
- Structured review report format
- Grading framework (A/B/C/D for answer accuracy and question quality)

Always run the reviewer before delivering final materials.
