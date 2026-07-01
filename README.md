# HR Operations Interview Playbook

An interactive, self-contained interview-prep tool for **HR Operations** roles, built for MBA candidates at the **University of Utah, David Eccles School of Business**.

It bundles a 48-question bank with layered model answers, the core HR Ops frameworks, a final-round battlecard, common red flags, a readiness self-assessment, a voice practice studio, and an AI-coach prompt generator — all in a single HTML file with no build step, no dependencies, and no backend.

---

## Live links

- **Playbook:** `https://coryjburk.github.io/intv-playbook-hrops_vc/`
- **User manual (styled):** `https://coryjburk.github.io/hr-ops-playbook/manual/`

---

## What's in this repo

| File | What it is |
|------|------------|
| `hr_ops_interview_playbook.html` | The playbook itself. Open it in a browser — everything runs locally. |
| `hr_ops_playbook_user_manual.html` | A styled, end-user manual (for students), matching the playbook's design. Best viewed via GitHub Pages. |
| `README.md` | This file — orientation for anyone landing on the repo. |

---

## Features

- **Question bank** — 48 HR Operations questions across 8 categories (HR Ops & Service Delivery, HRIS & Data, Compliance & Risk, Process Improvement, People Analytics & Metrics, Lifecycle & Experience, Stakeholder & Leadership, Behavioral). Each question has a model answer, a deeper rationale, coaching notes, and red flags. Search, filter by category/difficulty, mark reviewed, and rate your confidence.
- **Models & frameworks** — 8 reference models (Employee Lifecycle, Tiered Service Delivery, SIPOC, DMAIC, RACI, the Ulrich operating model, Moments That Matter, Root Cause Analysis).
- **Battlecard & red flags** — an 8-section quick-reference and 10 common candidate pitfalls.
- **Readiness self-assessment** — a 6-dimension rubric that rolls logged scores into an overall score, a readiness tier, and a trend over time.
- **Voice practice studio** — answer out loud; get word count, duration, speaking pace, and a rough filler tally. (See the transcription note below.)
- **AI coach** — generates a detailed prompt you paste into an AI assistant (e.g., Claude) for a mock interview or critique, then log the rubric scores it returns.

---

## Deploying to GitHub Pages

1. Push these files to the repository.
2. In **Settings → Pages**, set the source to the `main` branch (root).
3. The files serve at `https://coryjburk.github.io/<repo>/<filename>.html`.
4. Optionally rename `hr_ops_interview_playbook.html` to `index.html` so the playbook is the repo's default page.

No build, bundler, or server is required — these are static, standalone HTML files.

---

## Your data & privacy

All progress (reviewed marks, confidence ratings, logged rubric scores) is stored **locally in the user's browser** via `localStorage`. Nothing is uploaded by the playbook. Progress is tied to a specific browser and device; clearing browser data or switching browsers/devices starts fresh.

Storage keys are namespaced under `eccles_hrops_playbook_*` so this playbook's data won't collide with a separately deployed PM playbook on the same Pages domain.

---

## A note on voice transcription

The voice studio transcribes speech using the **browser's built-in speech recognition** (the Web Speech API), not a recording and not custom code. That engine has two known limits:

- It **mangles acronyms and jargon** (e.g., "HRIS," "FLSA"), substituting the nearest everyday words.
- It **drops or rewrites filler words** ("um," "uh"), so the filler count is a floor, not a precise measure.

This is a limitation of the free browser engine, not a defect in the playbook. The studio is best used to assess **pace, structure, and rambling** rather than word-perfect accuracy. A more accurate transcript (with HR-vocabulary recognition and filler detection) would require routing audio to a cloud speech service — a possible future enhancement. The full explanation lives in the user manual's *Voice practice studio* section.

---

## Requirements

- A modern desktop browser. **Chrome (or another Chromium-based browser) is recommended**, especially for the voice studio, where in-browser speech recognition is most reliable.
- Microphone access is required for the voice studio (the browser will prompt on first use).

---

## License / use

Internal teaching tool for the David Eccles School of Business MBA program.
