# Prompting Well: Communicating Clearly with AI — Skill Lab

An interactive, self-contained HTML activity for the **Module 1 skill lab** of a faculty development series on AI literacy. Faculty build prompts, compare weak and strong versions, steer the results, and test their work in Claude across models and effort levels.

This repo contains a single file, `prompting-skill-lab.html`, with no external dependencies — safe to host on GitHub Pages and embed in Canvas via iframe.

---

## Instructor facilitation note

### At a glance

| | |
|---|---|
| **Audience** | Faculty across disciplines; no prior AI experience assumed |
| **Setting** | Module 1 skill lab; works in a live session or fully asynchronous |
| **Time** | 45–60 min facilitated, or ~30 min self-paced |
| **What faculty need** | This page open, plus a [claude.ai](https://claude.ai) account open in a second tab, in a **private / incognito window** |
| **Outcome** | Faculty can brief Claude using Task / Context / Constraints / Output, steer a response toward what they need, choose a model and effort level to match the task, and leave with a personal verification checklist |

### What faculty should have open

Two tabs, side by side: this activity, and Claude. Before starting, point out the **model selector** and the **extended thinking (effort)** toggle in Claude's message box — the whole lab hinges on faculty finding and using those two controls.

> **Run Claude in a private / incognito window.** Have the cohort do the entire lab incognito so no saved memory or earlier chat influences a reply. This keeps everyone's A/B comparisons clean and comparable. Memory is introduced as its own concept — a variable the user controls — in the companion **Claude Onboarding** skills lab, which is the prerequisite to this one. Here, "switch to incognito" is all faculty need to do.

> **Note on model names.** The page references Sonnet 5 and Opus 4.8 as examples. Account tiers and model names change over time; tell faculty to use whichever current models and effort settings they have. The transferable skill is the *comparison*, not the label.

### Suggested run of show (≈50 min)

1. **Frame it (5 min).** The one idea: you don't need a secret formula, you need to communicate the work clearly — the same skill you use briefing a colleague or a research assistant. Confirm everyone is in an incognito window.
2. **Principles 1–4, Task/Context/Constraints/Output (20 min).** Walk the before/after cards. For each, have faculty copy *both* prompts into Claude, read the two replies, **then send the "Then steer it" follow-up** so they practice shaping the result, not just one-shotting it. The point lands fastest when they see how much improvement came from *defining the work* and *directing the output*, not from clever wording.
3. **Prompt builder (10 min).** Faculty build one prompt for something they actually need this term, then run the **four-way experiment**: Sonnet 5 and Opus 4.8, each with extended thinking off and on.
4. **Steer + thinking partner (10 min, Principles 5–6).** Faculty run the steering sequence (steer / direct / reshape — note this is the portable move that carries to agentic tools), then try one "critique, don't rewrite" prompt against their own material.
5. **Debrief (5 min, Principle 7).** Faculty judgment moves upstream: define the problem, supply context, evaluate the output. Land the **verification-decay** message below — this is the beat not to cut.

For a shorter session, assign the builder and the four-way experiment as pre-work and use class time for the debrief — but keep the Principle 7 verification-decay beat in the live portion; it's the part that most needs a human to land it.

### What to listen for in the four-model comparison

This is the part faculty find most revealing, and the discussion is richer if you steer it away from "which is best":

- **For simple, well-specified tasks, differences are often small.** Name this explicitly — it's the correct finding, not a failure. It tells faculty *not* to reach for the heaviest model by reflex.
- **Extended thinking earns its keep on ambiguity.** Tasks with real tension (the *Frankenstein* "end in disagreement" prompt, or any "challenge my assumptions" critique) are where the deeper model plus thinking tends to show its value.
- **Effort is a cost/benefit choice, not a quality dial.** Prompt faculty to ask: was the extra wait worth it *for this task*? Matching model and effort to the job is the skill.
- **Watch for plausible-but-wrong.** As responses get more polished, errors get harder to spot. Use the comparison to surface where two runs disagree on a fact — a natural cue to verify.

### The verification-decay message (Principle 7) — don't cut this beat

Principle 7 is not a checklist exercise; it's a warning about a predictable failure of habit, and it's the highest-leverage thing in the lab. Make these points explicit:

- **The checklist is correct but will decay in practice.** Once responses keep passing, people stop running the checks — precisely *because* the model looks reliable. Name this out loud so faculty expect it.
- **The cost is miscalibrated epistemics, and it compounds later.** A verification habit that lapses here carries into agentic tools, where output arrives faster than anyone can read it and there's functionally no time to check everything. Unchecked errors compound downstream. This is why it can't be deferred to a later module — deferring it shaves rungs off the ladder to agentic work.
- **What to have faculty actually do:** keep a short personal checklist of what matters most in their field (for most, avoiding hallucinated facts and citations comes first); run it *by hand every time*, even when sure; expect it to stop feeling necessary, and treat noticing that slip as the skill itself; then send the checks as prompts into a *fresh, adversarial* chat — always before anything reaches students. The closing reflection has each faculty member write their own checklist; make sure they leave with it.

### Good debrief questions

- Which single change to your prompt made the biggest difference in the reply?
- Where did more context matter more than a better model?
- When would you *not* bother with extended thinking?
- Where in the response did your disciplinary expertise catch something Claude got wrong or flattened?

### Common snags

- **Faculty can't find the effort toggle.** It moves around across interface versions; have them look near the model selector or the send button, and reassure them the exercise still works with just the model comparison.
- **"It saved my reflections and I lost them."** It doesn't — nothing is stored. Tell faculty upfront to keep their own notes; the copy buttons are the only thing that leaves the page.
- **File upload questions.** Principle 2 encourages attaching a rubric or objective. Faculty should use only anonymized or non-sensitive materials and follow your institution's data-handling policy.

### Accessibility & privacy

The activity uses semantic headings, keyboard-focusable controls, and high-contrast text. It sets nothing to a server and stores nothing locally — reflection boxes clear on reload by design.

---

## Embedding in Canvas

1. Commit `prompting-skill-lab.html` to this repo and enable **GitHub Pages** (Settings → Pages).
2. In a Canvas page's HTML editor, add an iframe pointing to the Pages URL:

   ```html
   <iframe src="https://YOUR-USERNAME.github.io/YOUR-REPO/prompting-skill-lab.html"
           width="100%" height="2400" style="border:0;"
           title="Prompting Skill Lab"></iframe>
   ```

3. The page scrolls internally, so set a generous fixed `height` (the value above is a safe starting point) or use an auto-resize script if your Canvas theme permits it.

## Attribution

Content adapted for use with Claude from a faculty-development presentation on prompting. Guidance reflects Anthropic's recommendations for working with Claude — including steering responses and treating first drafts as starting points rather than finished products.
