# Paper Intro & Evaluation Artifacts

This page summarizes the research paper associated with AppVA and
points to the evaluation data and reports stored in this repository.

## Paper information

**Title**  
From GUI Tests to Conversational Interaction: A New Perspective on App-Specific Voice Assistants

**Abstract**  
Voice assistants are widely deployed on mobile platforms, yet most are designed as system-level services that remain poorly aligned with application-specific behavior. As a result, enabling voice interaction at the app level requires developers to manually reimplement application logic and interaction workflows, leading to high development and maintenance costs.

We propose a novel, LLM-driven approach to automating app-specific voice assistants by repurposing GUI test code, which already encodes behavior-faithful, executable specifications of application functionality. In this paper, we advance a new perspective in which large language models act as semantic translators, reinterpreting GUI tests as bridges between application behavior and conversational interaction. By transforming test methods into app-specific VA artifacts, such as voice intents, action definitions, and executable interaction plans, our approach grounds voice assistants directly in existing application logic rather than external specifications.

We illustrate this vision through AppVA, a research prototype system that operationalizes the idea on Android. Our preliminary experience across five open-source applications suggests that GUI test code can be systematically reused beyond verification, enabling the synthesis of app-specific voice assistants and pointing toward a broader research direction at the intersection of software testing, interaction design, and LLM-enabled automation.

---

## Evaluation data

All evaluation data used in the paper is stored under the `eval_data/`
directory in the paper's git repository.

### 1. Evaluation workspaces

All the five tested application apks (install files) and their generated artifacts are in the :

```text
eval_data/eval_workspace/
  actionplan/
  intent/
  skills_description/
  com.faltenreich.diaguard/
  com.flauschcode.broccoli/
  com.futsch1.medtimer/
  hu.vmiklos.plees_tracker/
  org.totschnig.myexpenses/
eval_data/apks/
```

### 2. Evaluation reports

Path:

```text
eval_data/eval_report/
```

This folder is reserved for evaluation summaries, metrics, and any post‑processing scripts or CSVs used in the paper’s analysis.
