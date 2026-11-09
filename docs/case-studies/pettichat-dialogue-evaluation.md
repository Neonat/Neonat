# PettiChat research — persona dialogue and emotion evaluation

An experience case study of **Nathaniel Sim's Research Intern (Affective
Computing)** role at **PettiChat**, October–December 2025 in Hangzhou, China.
This account is based on the role description in his
[public LinkedIn experience](https://www.linkedin.com/in/nathaniel-sim/details/experience/).

## Research focus

The work explored how configurable pet personas could generate dialogue and how
the resulting responses could be evaluated for emotion and style. The broader
research context was human–pet communication.

## Contributions and outputs

| Area | Work described in the public experience record |
|---|---|
| Persona-based generation | Built a modular dialogue-generation and emotion-evaluation pipeline; synthesised additional dialogue from configurable pet personas. |
| Evaluation coverage | Assessed responses against **six emotion categories** and automated emotional-alignment checks plus **four dialogue-style constraints**. |
| Analysis records | Logged predictions, confidence and scores to CSV for inspecting model behaviour. |
| Model adaptation | Fine-tuned **RoBERTa** models on cat and dog dialogue datasets. |
| Research comparison | Evaluated textual emotion recognition (TER) and emotion recognition in conversation (ERC) approaches. |
| Proposed direction | Proposed a **mixture-of-experts (MoE)** approach for pet dialogue as a research direction. |

## Workflow described

```text
Configurable pet persona
        ↓
Generated dialogue
        ↓
Emotion evaluation + dialogue-style checks
        ↓
CSV predictions, confidence and scores
        ↓
Analysis of model behaviour
```

The six emotion categories and four style constraints describe evaluation
coverage. The public role summary provides no accuracy, latency, dataset-size or
comparative benchmark measurements to report here. The MoE item records a
proposal; the delivered work described above centres on generation, evaluation,
model adaptation and analysis tooling.

## Generative AI engineering themes

- **Generation and evaluation together:** pair persona-conditioned output with
  explicit checks for the behaviour the application needs.
- **Inspectable model behaviour:** retain predictions, confidence and scores in
  an analysis-friendly format.
- **Task-specific adaptation:** combine model fine-tuning and synthetic dialogue
  generation with a defined research question.

## Related public work

- [Sprout Web](https://github.com/Neonat/sprout-web) — multimodal plant-to-creature
  generation, operator tooling and testing in a collaborative project.
- [Mira](https://github.com/Neonat/mira) — evidence-linked LLM research and human
  review for an SMU YTP-AIF project responding to a DBS Internal Audit brief.

These projects illustrate related engineering interests across separate work
contexts. PettiChat's company information is available at
[pettichat.com](https://pettichat.com/).
