# Evidence notes

## RAGAS: V1 vs V2

In the current `data/ragas_report.json` run, V2 has slightly higher faithfulness (0.9617 vs 0.9543), while V1 has higher answer relevancy (0.9194 vs 0.8956) and context precision (0.9450 vs 0.9417). Context recall is 1.0000 for both. Both versions exceed the faithfulness target of 0.8. A plausible explanation is that V2's explicit fact-selection and no-speculation instructions improve grounding, while V1's shorter response style stays closer to the question; this is an interpretation of these scores, not a causal result.

## Evidence files

- `01_langsmith_traces.png` — LangSmith traces for the RAG pipeline.
- `02_prompt_hub.png` — the two versioned prompts in Prompt Hub.
- `02_ab_routing_log.txt` — A/B routing labels for the 50 questions.
- `03_ragas_scores.png` — terminal score comparison screenshot.
- `03_ragas_report.json` — copy of `data/ragas_report.json`.
- `04_pii_demo_log.txt` — PII redaction examples.
- `04_json_demo_log.txt` — JSON repair and fallback examples.
