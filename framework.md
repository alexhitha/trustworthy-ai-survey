---
title: Framework
nav_order: 2
---

# Conceptual Framework

_How the literature is organized: the major research problems and the families of technical approaches._

## Major research problems

_As framed by Wang et al. (TSE 2026):_

1. **Failure taxonomy:** what kinds of failures do agents have, and how should they be classified?
2. **Failure attribution:** which agent, which step, and what root cause led to a failure?
3. **Benchmarks:** how can attribution methods be evaluated and compared fairly?

## Families of approaches

_Families, central ideas, and reported costs come from Wang et al. (TSE 2026). They will be checked against the original papers as I read them._

| Category | Central idea | Examples | Reported cost |
|---|---|---|---|
| **Pattern analysis** | Find recurring signals across execution traces using statistics | FAMAS, CORRECT, AgentEval | FAMAS uses repeated replay, about 6–8x the tokens of reasoning-based methods |
| **LLM reasoning** | Have an LLM reason over the trace to infer the root cause | Who&When, ECHO, CHIEF, AgentRx | About 2–3x the tokens of single-pass prompting |
| **Model fine-tuning** | Train a specialized model to trace failures | AgenTracer, GraphTracer, Aegis | Lower cost per trace once deployed, but substantial training investment |
| **Dynamic runtime** | Form a hypothesis, then test it with a targeted intervention | DoVer, AgentDebug, TraceElephant | Typically the highest cost per diagnosis; needs access to the running environment |

## How the approaches compare

_My own comparison, in progress. For each approach:_

- _Does it need to know that the run failed?_
- _Does it need to re-run the agent?_
- _Does it need the full trace, or only outputs?_
- _Has it been tested on production agents?_
