# health-llm-eval-examples
Notes and examples on failure modes in health &amp; symptom triage LLMs
# Health LLM Symptom Triage — Evaluation Notes

This repository documents common failure modes observed in
health chatbots and symptom triage systems, particularly
around anxiety-driven physical symptoms.

The goal is to clarify where LLMs struggle and what kinds
of data or evaluation help reduce risk.

## Core problem

Users experiencing anxiety or panic often report physical
sensations (e.g. chest tightness, palpitations, breathlessness)
that resemble cardiac or medical emergencies.

LLMs frequently:
- escalate anxiety by implying imminent danger
- over-triage benign anxiety responses
- under-triage due to dismissive reassurance
- confuse subjective fear with objective risk

## Why this matters

In health-facing systems, these failures can:
- increase panic
- reduce trust
- cause inappropriate escalation
- create safety and liability concerns

## Common failure patterns

1. **Language ambiguity**
   - “pressure”, “tightness”, “flutter”, “can’t breathe”
2. **Context collapse**
   - ignoring stressors, timing, or emotional state
3. **Binary reasoning**
   - anxiety *or* heart issue, with no overlap handling
4. **Tone mismatch**
   - overly clinical or overly reassuring responses

## Where ACOS-H fits

ACOS-H (Anxiety–Cardiac Overlap Set – Human) is designed to
support training and evaluation around these edge cases by
providing natural, first-person narratives with structured context.

This repository does not include dataset files.
Previews are shared privately to ensure responsible use.

## Intended audience

- Health chatbot builders
- Symptom triage engineers
- Applied NLP practitioners in healthcare
- LLM safety and eval teams
