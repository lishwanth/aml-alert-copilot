# agents/

LangGraph multi-agent investigation pipeline.

Planned:
- `graph.py` — LangGraph graph definition wiring the agents together
- `transaction_analyst.py` — queries the DuckDB feature store, explains risk signals
- `compliance_research.py` — RAG over the regulatory corpus for matching typologies
- `report_writer.py` — drafts the citation-backed investigation memo ("draft for analyst review")
