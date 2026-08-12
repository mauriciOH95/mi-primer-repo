# Spanish Voice Eval Bench

A practical benchmark for evaluating Spanish text-to-speech systems consistently and turning qualitative listening judgments into structured, repeatable evaluation data.

## V1 scope

This first version focuses only on TTS output. It does **not** evaluate ASR, turn-taking, interruptions, latency, or agent behavior yet.

### Core evaluation dimensions

1. Pronunciation
2. Prosody
3. Rhythm & pace
4. Voice consistency
5. Audio quality
6. Naturalness

### Initial target

- 50 benchmark prompts for calibration
- Expand to 100–150 prompts after the rubric is stable
- Start with Neutral Latin American Spanish
- Compare multiple TTS voices/systems on the same prompts
- Use human labels as the reference set before adding automated evaluators

## Project structure

```text
spanish-voice-eval-bench/
├── README.md
├── data/
│   ├── prompts.csv
│   └── human_labels.csv
├── rubric/
│   ├── evaluation_rubric.md
│   └── failure_taxonomy.md
├── evals/
│   └── README.md
├── audio/
│   └── README.md
└── results/
    └── README.md
```

## Workflow

1. Design benchmark prompts.
2. Generate the same prompts with each TTS system or voice.
3. Evaluate samples using the rubric.
4. Record scores and failure tags.
5. Measure evaluator agreement and refine ambiguous criteria.
6. Compare systems by category and failure type.
7. Later, automate parts of the evaluation and run regression tests.

## Status

**Phase 1 — Benchmark design and human calibration**

The next milestone is to finalize the scoring rubric and create the first 50 benchmark prompts.
