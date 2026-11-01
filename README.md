# Аннотации по теме "Прослеживаемость решений агентов и анализ зависимостей"
## Структура проекта: 
```text
project/
├── main_files/
│   ├── 1-first_article.tex
│   ├── 2-second_article.tex
│   ├──...
├── images/
│   ├── beautiful.png
│   ├── img2.png
├── tables/
│   ├── tables.tex
├── README.md
├── literature.bib
└── annotations.tex
```

## Структура аннотаций 

Аннотация для каждой статьи должна следовать следующей структуре:
1. Название оригинальной статьи
2. Ключевые идеи, математическое описание метода
3. Алгоритм
4. Наборы данных
5. Метрики
6. Модели

## Стилистика оформления формул, текста в Tex 
- Длинное тире (например, в определениях) `~--`
- Все формулы (кроме математических символов, используемых единично в тексте; они должны быть заключены в $$) должны быть заключены в окружение `equation`
- При переносе формулы на следующую строку (или несколько следующих строк) использовать окружение `aligned`
- Стараться придерживаться единой системы обозначений. К примеру, если в основной статье, где дается первое определение методу/формуле вводится терминология и используются "канонические" обозначения, привести обозначения из последующих статей к этой же системе
- Если нужно что-то выделить, то использовать `\emph`

## Добавление аннотаций в репозиторий 
- Клонировать репозиторий
- Создать отдельную ветку, вести работу в ней
- Выставлять PR при добавлении аннотаций и вести работу в этой ветке, где будут оставляться комментарии и ревью
- При получении аппрува смерджить ветку в master

## Базовая литература 
- Агенты
  - для общего понимания и быстрого погружения в тематику https://github.com/pridees/agentic-design-patterns-book-rus
  - https://github.com/WooooDyy/LLM-Agent-Paper-List?tab=readme-ov-file#1-the-birth-of-an-agent-construction-of-llm-based-agents  
- Часть по прослеживаемости и безопасности
  - Обзор https://arxiv.org/abs/2606.04990
  - ProvenanceGuard https://arxiv.org/abs/2607.01236
  - CaMeL https://arxiv.org/abs/2503.18813

## Статьи для аннотирования
| № | Название | Год | Ссылка на источник | Ссылка на реализацию (github репо или другое) | Проаннотирована (✔) |
|---:| :--- | ---: | :--- | :--- | :---: |
| 1 | Safeguarding LLM Agents from Misalignment through Provenance Analysis | 2026 | [arxiv 2607.01236](https://arxiv.org/abs/2607.01236) | [Код](https://github.com/cmu-soda/ProvenanceGuard), [данные и пакет](https://doi.org/10.5281/zenodo.19342590) |  |
| 2 | The Granularity Mismatch in Agent Security: Argument-Level Provenance Solves Enforcement and Isolates the LLM Reasoning Bottleneck | 2026 | [arxiv 2605.11039](https://arxiv.org/abs/2605.11039) |  |  |
| 3 | TraceCompiler: Skill-Guided Mining and Compilation of LLM Agent Traces into Mostly Deterministic Workflows | 2026 | [arxiv 2608.02680](https://arxiv.org/abs/2608.02680) | [AppWorld](https://github.com/StonyBrookNLP/appworld) |  |
| 4 | When Tool Outputs Become Commands: Separating Action Induction from Runtime Authorization in Tool-Augmented LLM Agents | 2026 | [arxiv 2608.27146](https://arxiv.org/abs/2608.27146) |  |  |
| 5 | Localizing Emergent Failures in Agentic AI: Recovering Minimal Repair Families via Counterfactual Replay | 2026 | [arxiv 2608.29228](https://arxiv.org/abs/2608.29228) |  |  |
| 6 | From Agent Traces to Trust: A Survey of Evidence Tracing and Execution Provenance in LLM Agents | 2026 | [arxiv 2606.04990](https://arxiv.org/abs/2606.04990) | [Каталог литературы](https://github.com/xiaoqi-7/Agent-Tracing-Survey) |  |
| 7 | PROV-AGENT: Unified Provenance for Tracking AI Agent Interactions in Agentic Workflows | 2025 | [arxiv 2508.02866](https://arxiv.org/abs/2508.02866) | [Flowcept](https://github.com/ORNL/flowcept) |  |
| 8 | LLM Agents for Interactive Workflow Provenance: Reference Architecture and Evaluation Methodology | 2025 | [Источник](https://doi.org/10.1145/3731599.3767582) | [Код и материалы оценки](https://github.com/flowcept/FlowceptAgent-WORKS25) |  |
| 9 | AgentTrails: Towards Trust and Reuse for Agentic Tasks | 2026 | [arxiv 2607.18816](https://arxiv.org/abs/2607.18816) |  |  |
| 10 | LEDGER: Claim-to-Evidence Trace Graphs for Auditing LLM Agents | 2026 | [arxiv 2608.18398](https://arxiv.org/abs/2608.18398) |  |  |
| 11 | ExecWeave: Cross-Layer Execution Provenance for Observable Agentic Software | 2026 | [arxiv 2610.21146](https://arxiv.org/abs/2610.21146) | [Код](https://github.com/Irish-kw/ExecWeave) |  |
| 12 | AgentTriage: Replayable Security Diagnosis Across Heterogeneous Agent Runtimes | 2026 | [arxiv 2610.30738](https://arxiv.org/abs/2610.30738) | [Код и отдельные материалы](https://github.com/AsnGs/agenttriage-open-source) |  |
| 13 | Correct Answers, Unsupported Findings: Evidence Binding in Forensic Reconstruction of LLM Agent Logs | 2026 | [arxiv 2610.09581](https://arxiv.org/abs/2610.09581) | [Артефакт авторов](https://anonymous.4open.science/r/2027_DFRWS_EU-624C) |  |
| 14 | BLADE: Auditing Information Use for Failure Attribution in LLM Multi-Agent Systems | 2026 | [arxiv 2610.18780](https://arxiv.org/abs/2610.18780) | [Код](https://github.com/GXG-CS/BLADE) |  |
| 15 | Defeating Prompt Injections by Design | 2025 | [arxiv 2503.18813](https://arxiv.org/abs/2503.18813) | [CaMeL](https://github.com/google-research/camel-prompt-injection) |  |
| 16 | Securing AI Agents with Information-Flow Control | 2025 | [arxiv 2505.23643](https://arxiv.org/abs/2505.23643) | [FIDES](https://github.com/microsoft/fides) |  |
| 17 | IPIGuard: A Novel Tool Dependency Graph-Based Defense Against Indirect Prompt Injection in LLM Agents | 2025 | [Источник](https://aclanthology.org/2025.emnlp-main.53/) | [Код](https://github.com/Greysahy/ipiguard) |  |
| 18 | Can CaMeLs Talk? Securing Multi-Agent Systems Against Indirect Prompt Injection Attacks | 2026 | [arxiv 2610.05640](https://arxiv.org/abs/2610.05640) |  |  |
| 19 | SafeAgent: A Runtime Protection Architecture for Agentic Systems | 2026 | [arxiv 2604.17562](https://arxiv.org/abs/2604.17562) | [SafeAgent Core](https://github.com/SafeAgent-Development/safeagent_core) |  |
| 20 | Judges Follow the Reference: The Derivation Gap in Verifying Tool-Call Arguments | 2026 | [arxiv 2610.18497](https://arxiv.org/abs/2610.18497) | [Код](https://github.com/SarielMa/DeRef_release), [данные](https://huggingface.co/datasets/lm2445/DeRef) |  |
| 21 | AgentDojo: A Dynamic Environment to Evaluate Prompt Injection Attacks and Defenses for LLM Agents | 2024 | [arxiv 2406.13352](https://arxiv.org/abs/2406.13352) | [Код, среда и задачи](https://github.com/ethz-spylab/agentdojo) |  |
| 22 | Why and Where: A Characterization of Data Provenance | 2001 | [Источник](https://doi.org/10.1007/3-540-44503-X_20) |  |  |
| 23 | Provenance as Dependency Analysis | 2007 | [Источник](https://doi.org/10.1007/978-3-540-75987-4_10) |  |  |
| 24 | Language-Based Information-Flow Security | 2003 | [Источник](https://doi.org/10.1109/JSAC.2002.806121) |  |  |
| 25 | The Complexity of Causality and Responsibility for Query Answers and non-Answers | 2010 | [Источник](https://www.vldb.org/pvldb/vol4/p34-meliou.pdf) |  |  |
