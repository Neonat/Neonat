# PettiChat: evaluating emotion in generated dialogue

**Research internship · Hangzhou, China · October–December 2025**

At [PettiChat](https://pettichat.com/), I worked on dialogue generation and text-emotion evaluation for AI pet characters. The research question was whether a generated reply could express an intended emotion while staying within the character's speaking style.

This work formed part of a collaborative internship research project. My focus was the dialogue and text-evaluation experiments described here.

## The problem

A fluent reply can still miss the intended emotion, break character, or describe an action instead of speaking. Reviewing examples helps, but it becomes difficult to compare experiments when the checks and records change between runs.

The prototype made those checks explicit and kept each response alongside its evaluation.

## Work completed

- **Persona tooling and synthetic dialogue experiments.** Tools combined pet-personality descriptors with prompt templates, alongside experiments that generated dialogue for model adaptation.
- **Emotion-classification experiments.** RoBERTa training and inference notebooks explored classification of pet dialogue into six emotion categories. The work also included a review of textual emotion recognition and emotion recognition in conversation.
- **A generation-and-evaluation prototype.** A Python pipeline generated short character replies, classified their expressed emotion, compared predictions with intended labels, and applied four style checks.
- **Records for review.** CSV logs kept the input, generated reply, intended and predicted emotion, classifier confidence, style result, and evaluation score together.

## How evaluation worked

Style checks covered response length, narration, explicit emotion words, and a language heuristic. Emotion classification was a separate step. A reply could therefore match an emotion label while failing the speaking-style checks.

The evaluation combined those signals into a review record. Its score was an experimental rule, not a validated measure of how a person would interpret the reply.

## Tools and tradeoffs

Python supported the experiments and logging. PyTorch and Hugging Face Transformers provided model training and inference, while scikit-learn metrics and plots supported analysis. CSV made individual cases easy to inspect without a separate application.

Generation and classification were separate stages. This let the prototype inspect a reply with the same evaluation rules and record the cases that needed review.

## Research scope

These were research prototypes. The labels describe generated dialogue, not measurements of a real animal's emotional state. Classifier confidence is not proof of correctness, and automated style checks cannot replace human review.

A mixture-of-experts approach was proposed as a possible research direction. It was separate from the implemented generation and evaluation work.

The implementation, prompts, datasets, and internal results remain private.
