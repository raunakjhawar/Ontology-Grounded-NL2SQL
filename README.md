# Ontology Grounded NL2SQL

How do we turn a business question into a trustworthy query, rather than merely executable SQL?

This illustrated architecture brief explores how explicit entity mappings, governed measures, grain-aware planning, and independent validation help natural-language-to-SQL systems preserve business intent.

## Start reading

**[Read the illustrated architecture brief](./ontology-nl2sql-architecture-brief.md)**

The post follows a fictional consumer-goods question: **"Which customers missed target, and how much cash is overdue?"** It shows why answering correctly requires resolving customer identities, selecting authoritative facts, and applying consistent reporting cut-offs.

![Overview of disconnected business sources, semantic ambiguities, and the definitions needed to produce a checked answer.](./image-1.png)

## What you will learn

- Define a semantic contract covering identity, physical bindings, relationships, measures, grain, and time.
- Ground a logical plan instead of relying on schema retrieval alone.
- Distinguish context supplied to a model from independently enforced controls.
- Compare semantic placement, query execution, and ownership boundaries across Microsoft Fabric, and NVIDIA Auto-Ontology.
- Validate results against adversarial cases such as join fan-out, duplicate mappings, and future payments.
- Plan production controls for revisions, authorization-aware caching, consistency, query budgets, and observability.
