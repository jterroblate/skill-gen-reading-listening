---
name: skill-gen-reading-listening
description: Generate classroom-ready IELTS reading and listening materials from a speaking-topic pack, cue-card pack, or speaking question bank. Use when asked to create reading passages/questions, listening scripts/questions, student/teacher versions, transcripts, DOCX/PDF/ZIP outputs, or 根据口语题库生成阅读/听力材料. Includes workflow for invoking reading question review before delivery.
---

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
9. **Invoke skill-review-materials in Panel Mode** — spawn 3 independent editor sub-agents to audit every question for answer accuracy, paraphrasing quality, distractor plausibility, and technical correctness. Merge findings by consensus (≥2 editors = fix; 3/3 = must fix). Fix all critical issues before delivery.
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

### Listening question type requirements — PER SECTION (MANDATORY)

Each section must use IELTS-authentic question types. Do not mix types that would not appear together in the real exam. The following rules are non-negotiable:

**Section 1 (two-person dialogue):**
- 100% form / note / table / sentence completion
- NO MCQ, NO matching, NO choose-two
- Acceptable: NO MORE THAN ONE WORD AND/OR A NUMBER for each blank
- Tests: specific information extraction (names, numbers, dates, places, preferences, prices, contact details)
- This is the only section where minor detail recall is appropriate

**Section 2 (monologue):**
- MCQ + Choose TWO from a list of options, OR
- MCQ + Matching (match items to descriptions), OR
- MCQ + table/sentence completion
- PRIMARY focus: comprehension of main ideas, speaker's attitude, purpose, and the significance of examples
- DO NOT: test numerical details (number of years, volunteers, percentages) unless they represent a core conceptual point

**Section 3 (two-person discussion):**
- MCQ + Choose TWO, OR
- MCQ + Matching, OR
- MCQ + sentence completion (ONLY when each blank tests a concept, not a minor detail)
- PRIMARY focus: comprehension of arguments, research conclusions, contrasts between viewpoints, implications
- **CRITICAL: When the discussion involves research findings, comparative viewpoints, or advice-giving, Choose TWO or Matching is ALWAYS preferred over sentence completion.** Sentence completion in S3 context naturally tests keyword recall — Choose TWO requires understanding which multiple factors are correct.
- DO NOT: test trivial details (specific dates, small numbers, minor facts like "debating team") that could be answered without understanding the argument
- Distractors must represent reasonable alternative interpretations, not random unrelated information

**Section 4 (lecture):**
- ONE WORD ONLY note completion (standard IELTS format)
- Each blank must test a CONCEPT or KEY TERM (typically nouns or adjectives that represent core ideas)
- DO NOT: use blanks for minor modifiers, filler words, or trivial details
- The correct answer should be a word that carries conceptual weight in the lecture's argument structure

**Across all sections:**
- Every MCQ distractor must be thematically plausible (not obviously ridiculous)
- Completion blanks must test understanding + recall, not keyword scanning
- Avoid testing isolated numbers, years, or names unless they are central to the meaning

### Listening transcript word counts — PER SECTION (MANDATORY)
Each section's dialogue (excluding narrator instructions) must meet these minimum word counts:
- Section 1: at least 500 words
- Section 2: at least 500 words
- Section 3: at least 500 words
- Section 4: at least 500 words
Total listening material: at least 2,000 words across all 4 sections.
These are dialogue word counts — narrator instructions are excluded from the count.

### Script naturalness requirements (MANDATORY)
1. C19/C20 style reference: read 2-3 real IELTS transcript samples before drafting
2. Two-pass writing: Content Pass (topic coverage) → Naturalisation Pass (speech quality)
3. Each speaker needs subtle voice differentiation — verbal habits, hesitation patterns, cadence
4. Read-Aloud Test is mandatory: if it sounds awkward when spoken aloud, rewrite
5. Transitions must feel natural, not like task-driven topic switches
6. Avoid: sentences over 30 words; academic essay tone in dialogue; perfectly grammatical but unrealistic speech
7. Topic coverage check comes AFTER naturalisation, not before

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

### Matching Information question rules — MANDATORY
**Critical: Question order must NOT correspond to paragraph order.**

When creating Matching Information questions ("Which paragraph contains the following information?"), the question order MUST be shuffled so that correct answers do not follow paragraph order (A, B, C, D, E corresponding to Q1, Q2, Q3, Q4, Q5).

Rules:
- **Always shuffle the question order.** The correct answer for Q1 should NOT be A, and the questions must not follow the paragraph sequence.
- **Always include NB:** The instruction must always read: "Write the correct letter, A–E.\nNB You may use any letter more than once." — even if no paragraph is used twice in the current set. This is standard IELTS formatting.
- If the passage has 5 paragraphs and 5 questions, each question should correspond to a different paragraph, but the ORDER must be shuffled (e.g., Q1→C, Q2→A, Q3→E, Q4→B, Q5→D).
- If the passage has fewer paragraphs than questions, some paragraphs MUST be used more than once, and the NB covers this.
- **Verify after shuffling**: Read each question against its intended paragraph to confirm the answer is still correct.
- **Update the Answer Key** in the teacher version to reflect the new question order.
- Examples of BAD layout (NEVER do this):
  - ❌ Q1 specific example → A, Q2 scientific term → B, Q3 categorisation → C, Q4 ratio → D, Q5 reason → E
  - ✅ Q1 categorisation → C, Q2 specific example → A, Q3 reason → E, Q4 scientific term → B, Q5 ratio → D


### Question type patterns from Cambridge 19-20 (mandatory reference)

**TRUE / FALSE / NOT GIVEN:**
Instruction: "Do the following statements agree with the information given in Reading Passage {N}? In boxes {q-range} on your answer sheet, write TRUE if the statement agrees with the information / FALSE if the statement contradicts the information / NOT GIVEN if there is no information on this."

**YES / NO / NOT GIVEN:**
Instruction: "Do the following statements agree with the claims of the writer in Reading Passage {N}? In boxes {q-range} on your answer sheet, write YES if the statement agrees with the claims of the writer / NO if the statement contradicts the claims of the writer / NOT GIVEN if it is impossible to say what the writer thinks about this."
- Y/N/NG for opinion/argument passages, T/F/NG for factual passages.

**Notes Completion:**
Instruction: "Complete the notes below. Choose ONE WORD ONLY from the passage for each answer." (or "ONE WORD AND/OR A NUMBER")
- Uses section headers organizing related information. Items are short phrases, not full sentences.

**Summary Completion:**
Instruction: "Complete the summary below. Choose ONE WORD ONLY from the passage for each answer."
- ONE flowing paragraph with topic header. All blanks in one connected narrative.

**Sentences Completion:**
Instruction: "Complete the sentences below. Choose ONE WORD ONLY from the passage for each answer."
- Independent sentences (not connected). Each from different passage parts. RARE format.

**Multiple Choice (single):**
Instruction: "Choose the correct letter, A, B, C or D. Write the correct letter in boxes {q-range} on your answer sheet."

**Multiple Choice (two answers):**
Instruction: "Choose TWO letters, A-E. Write the correct letters in boxes {q-range} on your answer sheet."
- Spans two question numbers (e.g., "Questions 20 and 21").

**Matching Information:**
Instruction: "Reading Passage {N} has {X} paragraphs, {letter-range}. Which paragraph contains the following information? Write the correct letter, {letter-range}, in boxes {q-range} on your answer sheet."
- NOT 题文同序: questions are deliberately shuffled, not following paragraph order.

**Matching Headings:**
Instruction: "Choose the correct heading for each section {range} from the list of headings below. Write the correct number, {roman-numeral-range}, in boxes {range} on your answer sheet."
- Heading list includes 1-2 extra distractor headings. NOT 题文同序: requires understanding each paragraph as a whole, not linear answer-finding.

**Sentence endings matching:**
Instruction: "Complete each sentence with the correct ending, A-F, below. Write the correct letter, A-F, in boxes {q-range} on your answer sheet."
- Sentence stems are incomplete, options are endings.

**Statement-to-expert matching:**
Instruction: "Look at the following statements (Questions {range}) and the list of experts below. Match each statement with the correct expert, A-D. Write the correct letter, A-D, in boxes {range} on your answer sheet."
- NOT 题文同序: a person's views may be scattered across the passage.

**Summary with Phrase Bank:**
Instruction: "Complete the summary using the list of phrases, A-{N}, below. Write the correct letter, A-{N}, in boxes {q-range} on your answer sheet."
- Answer options provided in a labeled list.

**Flow-chart / Table Completion (C19 only):**
Instruction: "Complete the flow-chart / table below. Choose ONE WORD ONLY from the passage for each answer."

**题文同序 vs 不同序:**
✅ 题文同序 (follow passage order): T/F/NG, Y/N/NG, Notes/Summary/Sentences Completion, Multiple Choice, Flow-chart/Table
❌ NOT 题文同序 (scan/jump): Matching Information, Matching Headings, Statement-to-expert matching

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

### Question type patterns from Cambridge 19-20 Listening (mandatory reference)

**Part 1 — Two-person dialogue (Q1-10)**
Instruction: "Complete the notes/form/table below. Write ONE WORD AND/OR A NUMBER for each answer."
(Occasionally Q7-10 use "Write ONE WORD ONLY" instead.)

Answer characteristics:
- Answers are 90% single words, ~25% contain numbers
- Answer words are VERBATIM from the transcript — the speaker says them directly
- Common answer types: nouns (objects, places, people), numbers/prices, adjectives, names
- The question text frames the answer at the end of a phrase or in a table cell

Structure patterns:
- Notes format: hierarchical with section headers, short phrases with blanks
- Table format: column headers + rows, each cell may contain a blank
- Form format: labeled fields with blanks

Transcript interaction:
- Dialogue structure: greeting → information exchange → closing
- Questions are answered in order (strictly sequential)
- Answer often preceded by signal: "Well, ...", "Right.", "Yes, ...", "So, ...", "Actually, ..."

**Part 2 — Monologue (Q11-20)**
Common formats (in order of frequency):
1. MCQ: "Choose the correct letter, A, B or C" — ALWAYS 3 options, NEVER 4
2. Choose TWO: "Choose TWO letters, A-E" — 5 options, 2 answers, cross 2 question numbers
3. Box matching: "Choose SIX answers from the box" — options A-H, items Q11-16
4. Map labeling: "Label the map below. Write A-H" — SKIP this, hard to generate

MCQ design rules:
- Stems: Wh- question OR sentence starter OR topic tag + question
- 3 options MUST be parallel: same length, same grammatical structure, same specificity
- Each option references content from the transcript, placed in different contexts
- Correct answer is paraphrased from transcript, not verbatim
- Two distractors use similar words to the transcript but in WRONG context

Choose TWO design rules:
- 5 options (A-E), 2 correct, span "Questions X and Y"
- All 5 options are complete sentences (Part 2) or verb phrases (Part 3)
- Answers can be in either order (marked "in either order")
- Distractors: partially true statements that miss a key detail

**Part 3 — Two-person discussion (Q21-30)**
Common formats:
1. Choose TWO letters, A-E — 88% of tests, most common in Part 3
2. MCQ: "Choose the correct letter, A, B or C"
3. Box matching: "Look at the following descriptions... and the list of ideas below. Match each description with the correct idea, A-H"
4. Flowchart: "Complete the flowchart below. Choose FIVE answers from the box"

**🚫 FORBIDDEN in Part 3: Person-Name Matching**
NEVER create matching questions that require test-takers to match statements to speaker names (e.g., "Who said what? Match the statement to the speaker").
- Real IELTS Listening has zero examples of this format in C19/C20.
- Test-takers listen for voices and content, not names — forcing name recall is unnatural and unfair.
- Use box matching instead: match descriptions/concepts to idea phrases (A-H) or choose TWO (A-E).

Choose TWO differences from Part 2:
- Part 3 options use verb phrases (e.g., "experimenting with designs")
- Part 2 options use complete sentences (e.g., "The training exercises...")
- Part 3 has 3-4 consecutive Choose TWO groups, Part 2 has 1-2

Box matching design:
- Options box: 6-8 opinion/description phrases (A-H)
- Items: 5-6 topic words or short phrases
- 2 extra options serve as distractors

**Matching Questions HTML Interaction Rules (CRITICAL):**
When generating HTML for matching questions (box matching, area matching, or heading matching):
1. Use **click-to-match** interaction, NOT drag-and-drop (HTML5 Drag API is unreliable across browsers — console errors cannot be debugged).
2. Implementation: click an option → it highlights (`.sel` class) → click a dropzone → option fills in.
3. Use **inline `onclick` attributes**, not `addEventListener`. Inline attributes avoid closure bugs and scope issues entirely.
4. Required elements:
   - Options pool: `<div class="dd-option" onclick="ddClick(this)" data-letter="A">A. Option text</div>`
   - Dropzones: `<span class="dd-dropzone" data-correct="E" onclick="ddZone(this)"><span class="dd-placeholder">点此放置</span></span>`
5. Core functions (6 total):
   - `ddClick(el)` — select/unselect option, add/remove `.sel` class
   - `ddZone(el)` — place selected option into dropzone, add `.filled` class. **Store the option letter in a `data-placed` attribute on the zone** (not parsed from text content, to avoid "i"/"ii" first-character ambiguity).
   - `ddRem(btn)` — remove option from dropzone, restore option to pool. **Read `data-placed` attribute** to identify which option to restore.
   - `ddCheck()` — check all answers, mark zones as `.correct` or `.wrong`
   - `ddRev()` — reveal all correct answers
   - `ddRst()` — reset all zones and options (must clear `innerHTML`, remove `filled`/`correct`/`wrong`, restore options to pool)
6. CSS classes:
   - `.dd-option.sel` — selected option highlight (orange bg + border + shadow)
   - `.dd-option.used` — used option (greyed out, pointer-events:none)
   - `.dd-dropzone.filled` — filled zone (solid border instead of dashed)
   - `.dd-dropzone.correct` — correct answer (green)
   - `.dd-dropzone.wrong` — wrong answer (red)
7. **Button handlers must include both** standard and DD functions:
   - Submit: `onclick="checkAnswers();ddCheck()"`
   - Reveal: `onclick="revealAnswers();ddRev()"`
   - Reset: `onclick="resetAnswers();ddRst()"`
8. For **reading pages with existing grading systems**:
   - Keep hidden `<select>` elements with `style="display:none"` that the existing `gradePanel` can read.
   - Sync DD zone state to hidden select on every place/remove.
   - After `gradePanel` runs, sync hidden select grade classes (`.correct`/`.wrong-only`) to visible DD zones (`.correct`/`.wrong`).
   - On reset, also restore DD zones and options to initial state.
9. **Place answer reveals inside each dd-item**, not grouped at the end.
10. Use `var` (not `const`/`let`) for DD variables to ensure global accessibility.
11. This applies to ALL matching types: S2 exhibition area matching, S3 box matching, and reading heading matching.
12. Test all buttons after implementation: submit, reveal, reset, and individual zone remove.

**Part 4 — Academic monologue (Q31-40)**
UNIVERSAL format — 100% of tests:
- "Complete the notes below. Write ONE WORD ONLY for each answer."
- Hierarchical notes with section headers
- Answers are single common nouns, occasionally adjectives
- Answer words are VERBATIM from the lecture transcript
- Speaker often emphasises the answer word (slower, louder)

Signal words in lecture:
- "First of all..." → Q31 area
- "The main finding is..." → mid questions
- "Another important factor..." → Q35-37
- "In conclusion..." → Q38-40

**S4 Notes Summary Design Rules (CRITICAL):**
1. Write a proper detailed notes framework with section subheadings (e.g. "Historical background", "Recent improvements"), NOT standalone sentences.
2. Each section should have 3-5 lines: some with blanks, some as context filler — ALL styled identically.
3. Context lines (no blank) must NOT be visually downgraded — same font size, color, indentation as blank lines.
4. Precede each blank with sufficient context so it forms a coherent summary, not an isolated fact.
5. Answers must be verifiable from the lecture transcript, embedded naturally in the notes.
6. In the HTML, each blank line gets a ▶ 跳至音频 seek button linked to the correct audio segment.
7. The notes panel should be styled as one continuous document, NOT individual question blocks.
8. Example format:
   ```
   Historical background
   · Rivers were used for transport, fishing and recreation.
   · Pollution from 31______ on river banks.
   · In 1957, the Thames was declared biologically 32______.
   ```

**Difficulty progression within each Part:**
Part 1: Q1-3 easy → Q4-7 medium → Q8-10 tricky (numbers/details)
Part 2: Q11-13 easy → Q14-16 medium → Q17-20 harder (Choose2/box match)
Part 3: Q21-24 medium → Q25-27 harder → Q28-30 hardest (matching/box)
Part 4: Q31-33 easy → Q34-37 medium → Q38-40 harder (abstract)

**Distractor design patterns (CRITICAL):**
1. Same word, wrong context — "I used to be short-sighted" (past) vs "is short-sighted" (present)
2. Similar concept, wrong direction — "face-to-face declined 30%" vs "messages declined 30%"
3. Near synonym — "quite brief" vs "very short" (close but wrong detail)
4. Wrong agent — "A gave X to B" vs "B gave X to A"
5. Wrong number — "£4.95" vs "£5.95"

**Key difference from Reading:**
In Listening, answers are almost always VERBATIM transcript words.
The "paraphrase" is in how the QUESTION frames the answer, not in the answer word itself.

### Listening Generation Requirements (MANDATORY)

**1. Difficulty Progression**
S1 (Easy) → S2 (Medium) → S3 (Medium-Hard) → S4 (Hard)
- S1: Simple two-person dialogue, concrete information (names, numbers, places, items)
- S2: Monologue (radio/talk), some inference, MCQ with 3 parallel options
- S3: Two-person discussion, Choose TWO groups, opinions/comparisons
- S4: Academic lecture, abstract concepts, hierarchical notes, ONE WORD ONLY

**2. Speaking Topic Coverage**
- Minimum 80% of speaking-topic pack topics must be covered across the 4 sections
- Map each section's content to specific topics from the pack
- Verify coverage before generating

**3. Script Length**
- Target: ~450-600 words per section (3-4 minutes audio at ~150 wpm)
- S1 and S4 can be slightly shorter; S2 and S3 should be longer
- Total across all 4 sections: ~1800-2400 words

**4. Answer-Transcript Matching (CRITICAL)**
- Every fill-in answer must appear VERBATIM in the transcript
- Numbers spoken as words (e.g., "one hundred and fifty") may be answered as digits ("150")
- Phone numbers spoken digit by digit may be answered as continuous digits
- MCQ correct answers must be PARAPHRASED in the transcript (not verbatim)
- MCQ distractors must use transcript words in WRONG context

**5. MCQ Design Rules**
- NEVER test number recall ("How many respondents?", "What percentage?")
- ALWAYS test comprehension: cause-effect, opinion, comparison, purpose
- 3 options (A/B/C), parallel in length and grammar
- Choose TWO: 5 options (A-E), span two question numbers ("Questions X and Y")

**6. Question-Transcript Verification**
Before delivery, verify for each section:
- Fill-in answers: `answer.lower() in transcript_text.lower()` — must be True
- MCQ key words: each option's key phrase must reference transcript content
- No number-recall MCQs: flag any stem asking "How many", "What percentage", "What number"
- All 40 questions (10 per section) are answerable from the transcript

**7. Four Sections, 40 Questions (Standard IELTS Structure)**
| Section | Type | Questions | Format |
|---------|------|:---------:|--------|
| S1 | Dialogue - Notes/Form/Table | 10 | ONE WORD AND/OR A NUMBER |
| S2 | Monologue - MCQ + Choose TWO | 10 | 3-option A/B/C + A-E |
| S3 | Discussion - Choose TWO + MCQ | 10 | A-E + A/B/C |
| S4 | Lecture - Notes | 10 | ONE WORD ONLY |

**8. Difficulty Check**
Each section should be noticeably harder than the previous one:
- Vocabulary becomes more academic
- Answers require more inference
- Distractors become more plausible
- Section structures become more complex

**9. Script Naturalness Enhancement (MANDATORY — do NOT skip this step)**
Raw-first-draft scripts sound mechanical. This is NOT an AI model limitation — it's a script-writing process issue. Fix it with the following mandatory steps:

#### 9a. Prepare C19/C20 Style Reference
Before drafting, read **2-3 real Cambridge IELTS Listening transcripts** from C19/C20 as style reference. Internalise:
- How topics transition naturally ("Oh that reminds me...", "Actually, speaking of...", "That's interesting because...")
- Information is discovered through dialogue, not announced in lists
- Monologue signposting: "Let me turn to...", "Now another thing I should mention..."
- IELTS speech is natural and unforced, never literary

#### 9b. Write Content Pass (topic-first)
Draft covering all required speaking topics. Allow transitions to be rough. Prioritise information completeness.

#### 9c. Naturalisation Pass (SPEECH QUALITY GATE)
After content pass, rewrite ENTIRE script to improve naturalness only:

**Dialogue transitions:**
- ❌ Q: "Do you exercise?" A: "No, but I enjoy reading."
- ✅ Q: "So do you make time for exercise?" A: "Not as much as I'd like. I do try to read regularly though — it's the one habit I've managed to keep."

**Monologue flow:**
- ❌ "Mornings are important. Energy follows a 90-minute cycle."
- ✅ "Let's start with mornings — how you begin your day really sets the tone. Now, once you're working, you'll notice your concentration dips after about ninety minutes. That's your brain's natural rhythm."

**Character voice differentiation (subtle):**
- Speaker A: occasional "I mean" or "you know"
- Speaker B: shorter, more direct answers
- Speaker C: reflective — "Well, that's interesting..."
- Keep subtle — IELTS characters, not exaggerated

**Natural conversation markers:**
- Echo questions: "You mean...?" / "Wait, so...?"
- Agreement: "Exactly." / "That's a good point."
- Topic handover: "What about you?" / "What do you make of that?"

#### 9d. Topic Coverage Recheck
After naturalisation, confirm every required speaking topic is still present. Weave dropped topics back naturally — no forced insertions.

#### 9e. Read-Aloud Test
Read the ENTIRE script aloud. If any line sounds awkward, rewrite. If any transition feels abrupt, add a bridging phrase.

**Naturalness QC checklist:**
- [ ] Each speaker sounds distinct (not just different names)
- [ ] No speaker sounds like a fact list
- [ ] Dialogue = two people talking, not a Q&A
- [ ] Monologue has natural signposting and paragraph flow
- [ ] Read aloud: would a real person say this?
- [ ] No topic feels "inserted" — every topic arrives naturally

### Audio Generation Process (Robust Workflow)

**Follow this exact sequence for every Section. Do not skip steps.**

#### Step 0: Pre-Generation Checklist

Before any API call, verify ALL:
- Script word count >= 450 (target 500-600 = 3-4 min)
- Every voice ID responds 200 (test API before full generation)
- Gender matches: female characters use female voices; male = male
- `use_speaker_boost: true` (enhance)
- Model: `eleven_turbo_v2_5` (v3, not v2)

#### Step 1: Script Length (Minimum 450 words)

Target: 500-600 words per Section. Verify word count BEFORE calling any API.
S1+S4 can be slightly shorter (~450), S2+S3 longer (~550).
Script must read naturally aloud; avoid note form.

#### Step 2: Voice Assignment (Gender MUST match character)

| Character Type | Gender | Voice | Accent | Role |
|:--------------|:------:|:-----:|:------:|:----:|
| Narrator | Male | Michael | American | Official, authoritative |
| Receptionist/Secretary | Female | Rachel | British | Warm, professional |
| Caller/Customer | Match name | Match gender | Match accent | Check name gender first! |
| Radio Host | Male | Michael | American | Authoritative |
| Student 1 | Match name | Match gender | Match accent | Verify name gender |
| Student 2 | Match name | Match gender | Match accent | Verify name gender |
| Lecturer | Female | Rachel | British | Academic, clear |

**CRITICAL RULE: Check EVERY character name's gender.**
- Alice, Sarah, Bella, Mary = female voices
- Tom, John, David, Mark = male voices
- NEVER assign male voice to a character with a female name

#### Step 3: Audio Generation Rules

- One API call per speaker turn (each with their assigned voice)
- NEVER use `[pause]`, `[short pause]`, `[long pause]` tags with v2 models
- Use natural punctuation (periods, commas) for pacing with v3
- Always use `eleven_turbo_v2_5` model
- Always enable `use_speaker_boost: true`

#### Step 4: Combining Segments

CORRECT - use ffmpeg:
```
ffmpeg -f concat -safe 0 -i filelist.txt -c copy output.mp3
```

WRONG - NEVER do this (produces 4-second broken audio):
```
cat *.mp3 > output.mp3    # DO NOT USE
```

#### Step 5: Quality Check (Run BEFORE delivery)

Check all of these:
1. Duration: 150-240 seconds (3-4 min)
2. Word count: >= 450 words
3. File size: >= 1.5MB
4. Valid MP3 header (starts with ID3 or FF)
5. Gender: all character genders match their voices
6. Model: eleven_turbo_v2_5 (v3)
7. Enhance: use_speaker_boost = true

Use ffprobe to verify duration:
```
ffprobe -v error -show_entries format=duration -of csv=p=0 file.mp3
```

#### Step 6: File Saving (Handle Spaces in Path)

The output directory has spaces in its path. Use shell cp with quotes:
```bash
cp /tmp/audio.mp3 "/path/with/spaces/file.mp3"
```

#### Failure Mode Quick Reference

| Symptom | Cause | Fix |
|:--------|:------|:----|
| Audio only 4 seconds | cat instead of ffmpeg | Use ffmpeg concat |
| "[pause]" spoken aloud | pause tags in v2 model | Remove tags, use v3 model |
| Alice sounds male | Wrong gender voice | Check character name gender |
| Audio under 2 min | Script too short | Verify word count >= 450 |
| File not saved | Path with spaces | Use cp with quotes |
| Voice returns 404 | Wrong voice ID | Verify IDs before generation |
| No enhance | use_speaker_boost=False | Always set to True |
## Summary/Notes Completion checks
- Does each blank avoid being a "definition-to-term" mapping (i.e., asking for a concept name that the passage explicitly defines)? 🔴 CRITICAL — most common mistake
- Is the surrounding context a genuine paraphrase, not a near-verbatim copy with a word removed?
- Does each blank require comprehension of the passage, not just keyword matching?
- Is the word limit appropriate for the content? C20 pattern: ONE WORD ONLY or ONE WORD AND/OR A NUMBER (not NO MORE THAN TWO WORDS by default)
- If Notes format: are section headers used to organize the content hierarchically?
- Does each blank test a content word (noun/adjective), not a defined term name?

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

### HTML practice version checks
- Is the HTML file generated for every reading package?
- Does the HTML include ALL passages in one file with tab switching?
- Are question interactions implemented for each type (MCQ, T/F/NG, matching, fill-in)?
- Does each question have data-q and data-ans attributes for validation?
- Are answer-reveal divs correctly linked to their questions?
- Does the action bar have Check / Reveal / Reset buttons?
- Is the layout responsive (single-column below 900px)?
- Is the HTML file self-contained (no broken external dependencies)?
- Are answers correct in the data-ans attributes (matching teacher answer key)?

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
- "匹配题顺序和段落顺序一样"
- "匹配题没有 NB 提示"
- "summary 填空题是直接的术语定义对应测试"
- "summary 填空题几乎是原文复制"
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

### A2. Fill-in Completion Questions — MANDATORY (CRITICAL)

**There are exactly 3 valid formats in real IELTS (C19-20 analysis):**

**Format 1 — NOTES Completion (most common in C20: T1 P1, T2 P1, T3 P1, T4 P1)**

Instruction: "Complete the notes below. Choose ONE WORD ONLY from the passage" (or "ONE WORD AND/OR A NUMBER")

Structure:
- Has section headers that ORGANIZE related information (e.g., "Appearance:", "Movement:", "Feeding:")
- Each section header is followed by 1-3 short phrase items with blanks
- Section headers follow the passage's chronological or categorical order
- Items are PHRASES (not complete sentences) — often truncated or note-like
- Items in the same section share a common subtopic

C20 Example (T2 P1 Manatees):
```
Manatees - Appearance:
look similar to dugongs, but with a differently shaped [1].
Movement:
need to use their [2] to help turn their bodies
sense vibrations by [3] on their skin.
Feeding:
eat mainly aquatic vegetation, such as [4];
use their [5] to grasp food.
```

**Format 2 — SUMMARY Completion (C20 T1 P2 Elm, T2 P2 Procrastination, T4 P3 Guard Dogs)**

Instruction: "Complete the summary below. Choose ONE WORD ONLY from the passage"

Structure:
- ONE coherent flowing paragraph with a topic header line (e.g., "What makes us procrastinate?")
- ALL blanks are integrated INTO a single, continuous paragraph — NOT separate sentences
- The paragraph reads as connected narrative, not isolated facts
- Each sentence builds on the previous one

C20 Example (T2 P2 Procrastination):
```
What makes us procrastinate?
Many people think procrastination is the result of [17], or an inability to
organise time efficiently. Recent research links procrastination to emotions
and shows that people delay tasks that make them feel [18]. We avoid tasks
because they are associated with [19], such as the possibility of failure in
[20]. People likely to procrastinate tend to be either [21] or those with
low self-esteem. Procrastination is often followed by a feeling of [22],
which worsens mood and leads to more procrastination.
```

**Format 3 — SENTENCES Completion (rare: C20 T3 P2 Coral, T4 P2 Climate)**

Instruction: "Complete the sentences below. Choose ONE WORD ONLY from the passage"

Structure:
- Individual independent sentences (NOT connected to each other)
- Used only when content doesn't naturally form notes or a coherent summary
- Each sentence tests a different point from different parts of the passage
- This format is RARE (2 out of 12 fill-in sets in C20)

**CRITICAL RULE — NEVER mix formats.**
- "Complete the summary" MUST have ONE flowing paragraph with all blanks
- "Complete the notes" MUST have section headers organizing related items
- "Complete the sentences" MUST have individual independent sentences
- ❌ FORBIDDEN: Labeling separate single-sentence questions as "summary" — this doesn't exist in real IELTS

**Blank design principles (from C20 analysis of every fill-in question):**

1. **Blanks test content words that appear verbatim in the passage.**
   Real C20 answers are overwhelmingly CONCRETE NOUNS:
   - Body parts: tail, flippers
   - Plants/animals: seagrasses, jackals, foxes, potatoes
   - Materials/objects: charcoal, crystals, cellophane, bulbs, charcoal
   - People/roles: perfectionists, teachers, stakeholders
   - Places/structures: skyscrapers, dams, desks
   - Abstract nouns: funding, satisfaction, guilt, autonomy
   - Adjectives: anxious, dead
   - Numbers: 1980
   
2. **NEVER test the name of a concept the passage explicitly defines.**
   ❌ FORBIDDEN: "an effect known as ___" when passage says "a phenomenon known as X"
   ❌ FORBIDDEN: "a condition called ___" when passage says "researchers call this X"
   ❌ FORBIDDEN: "the term ___ describes..." when passage uses "the term X"

3. **The surrounding context must be a GENUINE paraphrase.**
   The Procrastination summary is an excellent model: every sentence thoroughly paraphrases the passage, not copying structure but testing comprehension.

4. **Answers must be VERBATIM from the passage.**
   Always verify: `answer.lower() in passage_text.lower()`

5. **Instruction word limits from C20 (authoritative):**
   - Reading: "ONE WORD ONLY" (most common, 8/12 sets) or "ONE WORD AND/OR A NUMBER" (4/12)
   - "NO MORE THAN TWO WORDS" does NOT appear in C20 reading, only in C19
   - For notes including dates/stats → "ONE WORD AND/OR A NUMBER"
   - For notes without numbers → "ONE WORD ONLY"
   - For summaries → "ONE WORD ONLY"

6. **The blank fits grammatically.** The sentence reads naturally when the answer is inserted.

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

---

## Generating Interactive Reading Practice HTML

After creating reading passages and questions, generate the interactive practice HTML using the **`skill-gen-html-reading`** skill.

### When to use

- The user requests an interactive practice interface for reading
- You have completed writing reading passages and questions (student version)
- You want drag-and-drop heading matching, MCQ/TFNG clickable, submit/reveal/reset

### How to use

1. Read `skills/skill-gen-html-reading/SKILL.md` for full instructions
2. Build a JSON data file with all 5 passages (passage text, questions, answers, reveals)
3. Run the generator script:

```bash
python skills/skill-gen-html-reading/scripts/generate_reading.py \
  --title "IELTS Reading · U01 Daily Rhythm" \
  --output "/path/to/刷题.html" \
  --data /tmp/passage_data.json
```

4. Validate the output:

```bash
python skills/skill-gen-html-reading/scripts/validate_reading.py "/path/to/刷题.html"
```

### Key features

- **Heading matching**: Drag-and-drop slots before each paragraph in the passage column
- **All question types**: MCQ, TFNG/Yes/No/NG, Matching Information (dropdown), Summary Completion (fill input)
- **Full heading text**: Shows complete heading text (e.g., "iii. A small commitment that grew naturally"), not just the key
- **Action bar at top**: Submit/reset/score buttons between tab bar and header — no wasted bottom space
- **Red/green feedback**: Correct answers turn green, wrong answers turn red after submission
- **Reveal buttons**: "💡 显示解析" buttons auto-generated, enabled after submission
- **PDF export**: Generate score report PDF from the browser

### Architecture

```
Tab Bar → Action Bar (submit/reset/score) → PDF Export → Header → Two-Column Layout
```

See `skills/skill-gen-html-reading/references/player-architecture.md` for full component tree.

---

## Cross-Reference: skill-review-materials

This skill generates materials. Quality assurance is handled by the companion skill:

**`skill-review-materials`** — IELTS Reading Question Reviewer & Editor

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
