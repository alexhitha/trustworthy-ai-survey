---
title: Research Papers
nav_order: 3
---

# Research Papers

_Papers are grouped by the categories in the [Framework](framework.html). Each entry lists title, authors, venue and year, a link, and a short summary of its main contributions._

## Surveys

### A Survey for LLM Agent Trajectory Analysis: From Failure Attribution to Enhancement
- **Authors:** Junjie Wang, Yawen Wang, Mengzhuo Chen, Xiaofei Xie, Chunyang Chen, Fangwen Mu, Zhe Liu, Qing Wang
- **Venue / Year:** IEEE Transactions on Software Engineering, 2026
- **Link:** [DOI](https://doi.org/10.1109/TSE.2026.3717765)

This survey reviews 55 papers, published between early 2025 and April 2026, on analyzing the execution trajectories of LLM agents. It organizes them along five dimensions: failure taxonomy, failure attribution, system enhancement and optimization, monitoring and analysis tools, and datasets and benchmarks. It groups failure attribution methods into four families: pattern analysis, LLM reasoning, model fine-tuning, and dynamic runtime methods. It reports that step-level attribution accuracy remains limited (about 25% to 52% on the Who&When benchmark), and that enhancement techniques rarely consume attribution outputs. It also maps these topics to classic software engineering techniques and calls for evaluation on real-world deployments.

## Agents in production

### Measuring Agents in Production
- **Authors:** Melissa Z. Pan, Negar Arabzadeh, et al. (UC Berkeley, Intesa Sanpaolo, UIUC, Stanford University, IBM Research)
- **Venue / Year:** ICML 2026
- **Link:** [arXiv 2512.04123](https://arxiv.org/abs/2512.04123)

This paper is the first large study of how LLM agents are built and run in production, based on 20 in-depth interviews with deployment teams and a survey covering 86 deployed systems across 26 domains. A general pattern emerges: teams deliberately choose simplicity and control over capability, because control makes agents more reliable. Most prompt off-the-shelf models with no post-training (70%), use predefined structured workflows rather than fully autonomous planning (80% of case studies), and keep agents to at most 10 steps before a human steps in (68%), which also keeps cost and model-migration effort low. Evaluation relies mostly on people (74%), and reliability, meaning consistent correct behavior over time, remains the top deployment challenge. Relevance to this survey: reliability is the main bottleneck for agents, just as it is for general software systems, so finding and fixing agent failures is an engineering problem, not only a model problem.

## Pattern analysis

_..._

## LLM reasoning

_..._

## Model fine-tuning

_..._

## Dynamic runtime

_..._
