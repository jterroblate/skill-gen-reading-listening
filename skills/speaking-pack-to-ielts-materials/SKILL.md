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

- “根据口语题库生成阅读材料和题目”
- “根据 speaking-topic pack 生成教师版答案”
- “补做同主题听力材料 + 仿 IELTS 听力题”
- “把口语文档转成阅读 / 听力课堂材料”
- “输出 student version / teacher version / transcript”
- “导出 DOCX / PDF / ZIP”

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
2. **Extract the pack’s internal structure and teaching line.**
3. **Map topics to suitable reading and/or listening task types.**
4. **Decide the output architecture before writing.**
5. **Draft the texts/scripts to fit the target question types.**
6. **Write questions that are naturally supported by the texts/scripts.**
7. **Produce teacher versions with concise explanations and speaking-transfer language.**
8. **Create separate student / teacher / transcript files as required.**
9. **Run the quality checklist before final output.**

If the result fails the checklist, revise the material before returning it.

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

Do not write short classroom paragraphs of 300 to 500 words unless the user explicitly asks for short texts.

### Difficulty progression
Default progression:

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
- three passages that all sound like “I remember…”
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

### Suggested reading question load
Default: around **10 to 13 questions per passage**

### Teacher version for reading
The teacher version must contain:
- full questions
- correct answers
- concise explanations
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
- simple service dialogue

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
**Form**: monologue

**Common scene types**:
- introduction
- guide talk
- orientation talk
- course / event description
- workshop introduction
- experience-sharing monologue
- museum / gallery / exhibition / club / activity explanation

**Target question style**:
- mostly multiple choice
- choose two / choose more than one
- small amount of matching where appropriate

**Core requirement**:
The script must support questions about:
- reason
- purpose
- evaluation
- viewpoint
- contrast
- important information
- priorities

Do not turn Section 2 into a disguised fill-in section.

### Section 3
**Form**: two-person discussion

**Common scene types**:
- project planning
- workshop planning
- review and comparison
- activity selection
- content evaluation
- proposal comparison
- cultural / social / product evaluation
- task preparation

**Target question style**:
- multiple choice
- choose two / choose more than one
- matching

**Core requirement**:
The script must naturally contain:
- agreement and disagreement
- comparison and trade-off
- decision criteria
- attitude shifts
- classification or evaluation of several options

**Speaker rule**:
- dialogue only
- exactly **two speakers**
- no multi-speaker group discussion

**Avoid**:
- turning Section 3 into detail-only note completion
- making the speakers merely exchange facts
- using options that are not meaningfully contrasted

### Section 4
**Form**: academic-style monologue / lecture

**Common lecture lines**:
- definition
- causes
- stages
- categories
- effects
- comparison
- implications
- recommendations

**Target question style**:
- note completion
- summary completion
- sentence completion
- table / flow-chart completion only when structure truly supports it

**Important rule**:
Section 4 should mainly behave like a **structured fill-in lecture**.

It should not mainly rely on multiple choice.

The fill-in layout for Section 4 should normally be presented as **embedded lecture notes / structured bullets**, not as a wide table that disconnects blanks from the note flow.

**Duration target**:
- roughly at least **3 minutes**
- enough length to sustain lecture structure

**Avoid**:
- random fact lists with no logical structure
- huge tables where the student cannot feel the lecture progression
- vocabulary trivia disguised as note completion

---

## Listening script-question co-design rules

This is the most important listening principle.

Before drafting any section, decide:

1. what the main question type will be
2. what information structure the script must have in order to support that question type naturally

Then draft the script accordingly.

### Required alignment
- Section 1 script must naturally support **form / note completion**
- Section 2 script must naturally support **multiple choice + some matching**
- Section 3 script must naturally support **choice + comparison + matching**
- Section 4 script must naturally support **structured fill-ins**

If a draft script does not support the target question type naturally, revise the script before writing the questions.

Do not patch the problem later by writing weak or unnatural questions.

### Listening question design rules
- keep question order aligned to script order
- language should feel close to IELTS style
- do **not** use True / False / Not Given
- avoid excessive reliance on tiny factual details
- balance:
  - detail
  - understanding
  - reasoning
  - comparison
  - purpose
  - attitude
  - structure

### What to avoid in listening questions
Avoid:
- all questions being “what time / where / how much”
- purely mechanical detail filling
- weak distractors
- answer wording copied too directly from script
- sections whose question type does not fit the script
- forcing a table layout when notes would be clearer

### What to do more of
Include questions that test:
- speaker purpose
- reason and evidence
- shared agreement
- comparison and trade-off
- evaluation of options
- lecture structure
- main implications

### Teacher version for listening
The teacher version must contain:
- full questions
- correct answers
- concise explanation for each answer
- explanation of wrong options when useful
- explanation of matching logic where relevant
- location of support in the script
- a **speaking-transfer language** section for each section

### Speaking-transfer language for listening
Select expressions that help students talk about:
- preference
- interest
- evaluation
- comparison
- expectation and disappointment
- habit and routine
- social influence
- cultural judgment
- convenience vs drawback
- online vs offline communication
- personal feeling and wider impact

Keep the list selective. It should be pedagogically useful, not decorative.

### Transcript rules
Create a standalone transcript document.

Requirements:
- mark **Section 1 to Section 4**
- if it is a monologue, do **not** force speaker labels
- if it is a dialogue, keep only **two speakers**
- format clearly so it can be used for TTS
- keep punctuation and paragraphing clean

---

## Layout and formatting rules

## General
- produce clean classroom-friendly formatting
- use clear section headings
- leave enough white space
- separate student and teacher materials
- do not make the final output look like a chat transcript

## Reading layout
### Student version
- cover page
- theme overview
- passage
- questions
- no answers

### Teacher version
- similar structure to student version
- answers and explanations added in the question area or immediately after
- speaking-transfer expressions clearly highlighted

## Listening layout
### Student version
- section heading
- optional short section info block such as:
  - format
  - main focus
  - approximate audio length
- questions only
- no answers

### Teacher version
- same question structure
- answers and concise explanations added
- speaking-transfer expressions added

### Transcript document
- section heading
- clean script body
- dialogue sections: exactly two speakers
- monologues: no fake speaker tags

### Critical fill-in layout rule
For **Section 1** and **Section 4**, if the task is note / form / summary completion, present it in a way that preserves the note flow.

Default preference:
- embedded notes
- short bullet structures
- form-style lines
- sentence-style completion

Avoid:
- wide grid tables that make it unclear where the blank sits in the text logic

Tables may be used only when they improve clarity and still preserve order. They are **not** the default for fill-ins.

---

## File outputs

When file creation is available, prioritize:

### Reading package
- `<theme_slug>_reading_student.docx`
- `<theme_slug>_reading_student.pdf`
- `<theme_slug>_reading_teacher.docx`
- `<theme_slug>_reading_teacher.pdf`

### Listening package
- `<theme_slug>_listening_student.docx`
- `<theme_slug>_listening_student.pdf`
- `<theme_slug>_listening_teacher.docx`
- `<theme_slug>_listening_teacher.pdf`
- `<theme_slug>_listening_transcript.docx`
- `<theme_slug>_listening_transcript.pdf`

### Combined bundle
- `<theme_slug>_ielts_materials_pack.zip`

If the user requests only one package, only generate the files relevant to that package.

---

## Quality checklist before output

Do not deliver until all relevant checks pass.

### Source relevance
- Is the material clearly anchored to the uploaded speaking-topic pack?
- Would the package still make sense if the source theme were different?
- Have you avoided generic filler content?

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

### Final file checks
- student / teacher / transcript are separate when required
- filenames are clear
- DOCX / PDF / ZIP are included when appropriate
- the final response gives direct download links

---

## Revision protocol

If the user gives feedback such as:
- “文体太单一”
- “不要全是第一人称”
- “长度要更像雅思”
- “Section 1 和 4 的填空不要做成表格”
- “Transcript 单独输出”
- “教师版多加可迁移表达”
- “听力题型要更贴近 section 结构”

then revise the affected files directly rather than rewriting the entire approach from scratch.

Preserve:
- the source theme cluster
- the material architecture
- the file separation logic

Only change what is necessary to fix the user’s concern.

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

This skill is not a generic “write some IELTS material” instruction.

It is a **conversion workflow**:

**speaking-topic pack -> theme analysis -> task architecture -> reading/listening generation -> question design -> teacher support -> file packaging**

The generated materials must be:
- tightly linked to the uploaded pack
- structurally appropriate for IELTS
- useful in class
- useful for later speaking output
- clearly formatted
- easy to revise
