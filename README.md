# Ontological Fidelity Scorecard

**7 structural questions every Clinical AI team should answer before deployment.**

[Take the Scorecard](https://1977flow.github.io/odix8-scorecard/) | [Research Corpus](https://1977flow.github.io/odix8-scorecard/research.html)

---

## The Problem

Most clinical AI systems fail not because of bad algorithms, but because they train on structurally distorted data. Billing codes get treated as diagnoses. Administrative categories get mistaken for clinical realities. Workflow artifacts get encoded as medical truth.

These distortions are invisible to standard ML evaluation metrics. A model can achieve excellent accuracy, F1, and AUC scores on benchmarks while systematically learning from data that misrepresents the clinical phenomena it claims to model. The result: systems that perform well in validation but fail on contact with real clinical workflows.

This is not a data quality problem in the conventional sense. It is an ontological problem: the categories your model learns from do not correspond to the clinical realities it needs to represent. We call this **ontological distortion**, and our research has identified seven specific architectural patterns that determine whether a clinical AI system will survive deployment.

## The 7 Design Patterns

The Ontological Fidelity Scorecard evaluates clinical AI systems against seven design patterns derived from peer-reviewed research:

| # | Pattern | Description |
|---|---------|-------------|
| 1 | **Coding-Fidelity Annotation** | Distinguishing billing codes from clinical diagnoses at data ingestion. A patient coded J06.9 for reimbursement may actually present with early pneumonia. |
| 2 | **Signal Preservation** | Preventing rare but critical clinical signals from being drowned by high-volume routine codes in training data. |
| 3 | **Semantic Drift Detection** | Monitoring when terminology meaning shifts due to billing guideline changes, not just statistical distribution shifts. |
| 4 | **Dual Representation** | Maintaining parallel clinical and administrative data layers rather than collapsing them into a single representation. |
| 5 | **Feedback Loop Monitoring** | Tracking the AI influence ratio to prevent reification loops where models reinforce their own distortions. |
| 6 | **Terminology Governance** | Treating vocabulary updates (ICD, SNOMED, LOINC) as schema migrations, not silent changes. |
| 7 | **Regulatory Modularity** | Building pluggable compliance layers (EU AI Act, MDR) rather than hard-coding regulatory logic. |

## Scoring

| Score | Rating | Implication |
|-------|--------|-------------|
| 0-3 | **High Risk** | Structural blind spots likely affecting model validity |
| 4-5 | **Partial Coverage** | Key gaps remain in ontological infrastructure |
| 6-7 | **Ontology-Aware** | Your system addresses structural fidelity |

Most teams score 0-3. This is not a failure of engineering talent. It is a failure to examine the ontological layer beneath the data.

## Research Foundation

This framework is derived from 12 peer-reviewed publications spanning 22 disciplines, including:

- **EMoT: Empirical Model of Thoughtfulness** — [arXiv:2603.24065](https://arxiv.org/abs/2603.24065)
- **Ontological Distortion Series** — 4-paper series (SSRN, arXiv, npj Digital Medicine)
- **Terminology Governance Series** — 4-paper series (IJMI, arXiv, JAMIA)
- **Design Patterns for Ontological Fidelity** — arXiv (in preparation)

Full research corpus: [Research Portfolio](https://1977flow.github.io/odix8-scorecard/research.html)

## How to Use

1. **Take the scorecard** at [1977flow.github.io/odix8-scorecard](https://1977flow.github.io/odix8-scorecard/)
2. Answer all 7 questions honestly
3. Review your score and the corresponding recommendation

**Scored 0-3?** Book a complimentary 30-minute Ontological Fidelity Review: [office@odix8.com](mailto:office@odix8.com)

## About oDIX8

**oDIX8 | Systems for Innovation**

We identify why Clinical AI fails before you deploy it. Our work sits at the intersection of clinical medicine, information systems, and AI governance.

Based in Halle (Germany) and London (UK).

[www.odix8.com](https://www.odix8.com) | [office@odix8.com](mailto:office@odix8.com)

## License

Content: [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/) — Attribution required, non-commercial use.

The Ontological Fidelity framework and design patterns are published research. Citation: Stummer, F. (2026). Ontological Fidelity Scorecard. oDIX8 Systems for Innovation.
