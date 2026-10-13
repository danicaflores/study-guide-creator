# Study Guide Creator

A [Claude Code](https://claude.com/claude-code) skill that turns college course materials (lecture slides, class notes, textbook chapters, and study objectives) into organized, easy-to-understand study guides for exams.

## What you get

Every study guide includes:

- Key terms and definitions, with a plain-language version of each
- Main concepts with simple explanations and examples
- Formulas, each with its symbols defined and a step-by-step worked example
- Frameworks with real-world examples, for subjects like marketing or management
- Common mistakes and how to avoid them
- Practice questions labeled Easy, Medium, or Challenge
- An answer key that explains each answer
- A final review checklist
- "Gaps to check": anything your materials leave unclear

## How it adapts to your subject

| Subject type | Examples | What the guide focuses on |
|---|---|---|
| Quantitative | Statistics, economics, math, accounting | Formulas, step-by-step calculations, "which formula do I use?" guides |
| Conceptual | Marketing, management, psychology | Frameworks, comparisons, real-world examples |
| Memorization-heavy | Biology, history, languages | Grouped terms, timelines, memory aids |

## Ground rules the skill follows

- **Your materials come first.** It uses your course's wording and notation.
- **It never invents facts.** Anything not from your materials is labeled, and anything missing is listed under "Gaps to check."
- **It uses simple language.** Sentences are short, and jargon is explained.

## Installation

1. Download this repository. Click the green **Code** button, then **Download ZIP**, and unzip it.
2. Move the `study-guide-creator` folder into your Claude Code skills folder:
   - **Mac or Linux:** `~/.claude/skills/`
   - **Windows:** `C:\Users\<you>\.claude\skills\`

   On a Mac, `.claude` is a hidden folder. In Finder, press **Cmd + Shift + G** and type `~/.claude/skills` to open it. Create the `skills` folder if it doesn't exist yet.
3. Start a new Claude Code session. The skill loads when a session starts.

When you're done, the folder should look like this:

```
~/.claude/skills/study-guide-creator/
├── SKILL.md
├── README.md
├── templates/
│   └── study-guide-template.md
└── references/
    └── subject-formats.md
```

## How to use it

Attach or point to your materials and ask in plain words. For example:

- "Make me a study guide for my STAT 2011 exam from lecture8-notes.md"
- "Help me study for my econ midterm. Here are my slides." (with a PDF attached)
- "Turn my chapter 3 notes into a review sheet"

The guide is saved as a Markdown file (for example, `study-guide-econ-2035-elasticity.md`) next to your materials. Claude also tells you what it covers and what gaps it found.

The skill doesn't run for unrelated requests, such as coding, answering one quick question, summarizing an article, or proofreading an essay.

## Files

| File | Purpose |
|---|---|
| `SKILL.md` | The instructions Claude follows: when to activate, the rules, the step-by-step process, and a quality check |
| `templates/study-guide-template.md` | The reusable study guide layout |
| `references/subject-formats.md` | How to adapt the guide for each subject type |

## Testing

The skill was tested on sample statistics notes (z-scores and the normal distribution) and sample economics notes (supply, demand, and elasticity). Every calculation in the generated guides was checked with Python. A routing check confirmed that it activates for study guide requests and stays off for unrelated tasks.

## Tips for best results

- Include your exam objectives or review sheet if you have them. The guide will follow them in order.
- Use the practice questions before you look at the answer key.
- Ask for follow-ups like "more practice on elasticity" or "turn this into flashcards."
