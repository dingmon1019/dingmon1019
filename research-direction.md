# ICML 2026 Research Prep

ICML 2026 context: July 6-11, 2026 at COEX Convention & Exhibition Center, Seoul, South Korea. I am attending as a backend engineer refining research direction, not as a paper author.

## One-line identity

Turning practical AI engineering experience into testable research questions.

## Research questions

### 1. Medical XAI: explanation faithfulness

- When a heatmap looks plausible to a human, how can we test whether it is faithful to the model's actual decision process?
- In medical imaging, which perturbation, localization, counterfactual, or human-in-the-loop evaluations reveal misleading explanations?
- Can explanation quality be evaluated separately for segmentation, classification, and retrieval-style workflows?

### 2. Uncertainty and calibration for explanations

- Can uncertainty signals help users decide when an explanation should not be trusted?
- How should calibration be reported together with saliency, attribution, or explanation-map outputs?
- Is there a practical way to flag cases where the model is confident but the explanation is unstable, or where the explanation is stable but the prediction is uncertain?

### 3. Agent explainability

- Which parts of an LLM agent trace help a human debug the agent's failure?
- Which trace elements support accountability rather than merely producing a convincing story after the fact?
- Can agent traces be evaluated with task-specific outcomes such as faster debugging, better rejection decisions, or more reliable handoff?

### 4. AI-assisted software engineering evaluation

- How can real engineering tasks become small benchmarks for AI coding agents?
- What should be measured beyond pass/fail: maintainability, testability, regression risk, review burden, and failure analysis?
- Can audit logs, plans, diffs, tests, and review notes become evidence for evaluating an agent's usefulness?

## Papers to read

This is a starter reading queue. Before ICML, refresh the list against the official ICML 2026 program, OpenReview, and workshop pages.

### Explanation faithfulness and saliency evaluation

- Adebayo et al., **Sanity Checks for Saliency Maps**.
- Yeh et al., **On the (In)fidelity and Sensitivity of Explanations**.
- Samek et al., **Evaluating the Visualization of What a Deep Neural Network Has Learned**.
- Hooker et al., **A Benchmark for Interpretability Methods in Deep Neural Networks**.

### Medical XAI and clinical interpretability

- Ghassemi et al., **The false hope of current approaches to explainable artificial intelligence in health care**.
- Tjoa and Guan, **A Survey on Explainable Artificial Intelligence (XAI): Toward Medical XAI**.
- Papers from MICCAI / MIDL / LXAI workshops on explanation faithfulness, segmentation, uncertainty, and radiology workflows.

### Uncertainty and calibration

- Guo et al., **On Calibration of Modern Neural Networks**.
- Gal and Ghahramani, **Dropout as a Bayesian Approximation: Representing Model Uncertainty in Deep Learning**.
- Kendall and Gal, **What Uncertainties Do We Need in Bayesian Deep Learning for Computer Vision?**.
- Ovadia et al., **Can You Trust Your Model's Uncertainty?**

### Agent explainability and AI-assisted software engineering

- Yao et al., **ReAct: Synergizing Reasoning and Acting in Language Models**.
- Papers and benchmarks around SWE-bench, AgentBench, tool-use agents, reasoning traces, and process supervision.
- Work on whether chain-of-thought or trace-style explanations are faithful, useful, or merely persuasive.

## Poster questions

Use these when a poster is close to XAI, uncertainty, agents, or medical imaging:

1. What is the unit of evaluation for the explanation: pixels, concepts, regions, decisions, traces, or user actions?
2. How do you distinguish visually plausible explanations from faithful explanations?
3. Did you test explanation stability under perturbations, distribution shift, or model retraining?
4. Where does uncertainty enter the workflow: prediction confidence, explanation confidence, calibration, or user-facing warnings?
5. What failure case made you distrust the method?
6. If this method were used in a medical imaging workflow, what would be unsafe to infer from the explanation?
7. For agent traces: which trace fields helped humans make better decisions, and which were noise?
8. Do you evaluate trust as user satisfaction, task performance, debugging time, rejection accuracy, or accountability?
9. What minimal benchmark would you recommend for someone entering this research direction from backend engineering?
10. What should I read next if I want to connect this work to practical systems and agent debugging?

## Follow-up message template

Subject: ICML 2026 follow-up on [poster/topic]

Hi [Name],

Thank you for discussing your ICML poster on [topic]. I am a backend engineer transitioning toward XAI and agent explainability research, especially around faithful explanation evaluation, uncertainty, and agent trace usefulness.

One point I found especially useful was [specific detail from the conversation]. It connects to a research question I am trying to sharpen: [one-sentence question].

If you have time, I would appreciate one or two recommended papers or benchmarks for someone approaching this from practical engineering systems rather than a completed research background.

Best,
Hwang Junsu
https://github.com/dingmon1019
