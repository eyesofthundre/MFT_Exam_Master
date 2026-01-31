# MFT Exam Master - Project Context

## Overview
A single-page web application to help Marriage and Family Therapy students prepare for the AMFTRB national licensing exam. Built with pure HTML/CSS/JavaScript (no dependencies), fully offline-capable.

**Live Site:** https://eyesofthundre.github.io/MFT_Exam_Master/

## Current Status (Jan 2026)
- **470 questions** across 6 domains
- All questions include detailed explanations, academic citations, and study links
- Rating system implemented for question feedback
- Enhanced navigation with visual question palette
- WCAG AAA accessibility compliant

## Project Structure
```
/MFT_Exam_Master/
├── index.html                    # Complete single-file application (~163KB)
├── questions/                    # Question database (JSON files)
│   ├── domain1_systemic_therapy.json   # 60 questions
│   ├── domain2_assessment.json         # 60 questions
│   ├── domain3_treatment.json          # 65 questions
│   ├── domain4_evaluation.json         # 95 questions
│   ├── domain5_crisis.json             # 95 questions
│   └── domain6_ethics.json             # 95 questions
├── README.md, SETUP.md, LICENSE
└── docs/                         # (reserved for future documentation)
```

## Question Format
```json
{
  "id": 101,
  "domain": "Practice of Systemic Therapy",
  "difficulty": "easy|medium|hard|phd",
  "tags": ["Bowen", "differentiation", "theory"],
  "question": "Main question text",
  "vignette": "Optional clinical scenario",
  "options": ["Option A", "Option B", "Option C", "Option D"],
  "correct": 0,
  "explanation": "150-250 word detailed explanation",
  "citation": "Author (Year). Title. Publisher.",
  "studyUrls": ["https://..."],
  "memoryTip": "Optional memory aid"
}
```

**ID Convention:** Domain number + question number (e.g., 301 = Domain 3, Question 1)

**Difficulty Distribution:** easy (~35%), medium (~40%), hard (~20%), phd (~5%)

## The 6 AMFTRB Domains
1. **Domain 1** - Practice of Systemic Therapy (Bowen, Minuchin, SFBT, EFT, Narrative)
2. **Domain 2** - Assessing, Hypothesizing, Diagnosing (DSM-5-TR, case conceptualization)
3. **Domain 3** - Designing and Conducting Treatment (interventions, techniques)
4. **Domain 4** - Evaluating Process and Terminating (outcomes, relapse prevention)
5. **Domain 5** - Managing Crisis Situations (suicide, DV, mandated reporting, Tarasoff)
6. **Domain 6** - Ethical, Legal, Professional Standards (AAMFT ethics, HIPAA, boundaries)

## Study Modes
- **Practice Mode** - Instant feedback, explanations, citations after each answer
- **Exam Simulation** - 200 questions, 6-hour limit, no feedback until end
- **Custom Sessions** - Select domains, difficulty, question count

## Key Features
- Question navigator (visual grid showing answered/unanswered)
- Rating system (Good, Irrelevant, Wrong Answer, Other Issue)
- Session history and analytics
- Keyboard shortcuts (1-4/A-D for answers, Enter/Backspace for nav)
- Accessibility themes (light, dark, high contrast, dyslexia-friendly)
- Font size and line spacing controls
- LocalStorage persistence (all progress saved automatically)

## Recent Development
- Added 65 ethics questions with detailed rating system
- Added 140 new questions across domains
- Enhanced navigation with question palette
- Improved accessibility overrides

## Quality Standards for Questions
- Clear clinical scenario or theoretical concept
- 4 plausible answer options
- 150-250 word explanation
- Academic citation from credible MFT source
- Study URLs to official resources
- Appropriate difficulty tag
- Relevant clinical tags

## Key Textbooks/Sources
- Bowen (1978) - Family Therapy in Clinical Practice
- Minuchin (1974) - Families and Family Therapy
- Johnson (2004) - Emotionally Focused Couple Therapy
- White & Epston (1990) - Narrative Means to Therapeutic Ends
- AAMFT Code of Ethics
- DSM-5-TR

## Deployment
Push to GitHub → auto-deploys to GitHub Pages in 2-3 minutes

## Working Conventions
- **Branch:** `develop` for active work
- **Commits:** Descriptive messages (e.g., "Add 65 ethics questions and detailed rating system")
- **Testing:** Open index.html locally before pushing

## Potential Future Work
- Additional questions to reach 500+ total
- More vignette-based clinical scenarios
- Spaced repetition study mode
- Question export/import functionality
- Performance analytics by tag/concept
