# System Card Reporting Review

A reusable method, and a first case study, for checking how well an AI system card reports the evidence behind its conclusions.

> **Disclaimer:** This is not a safety assessment. It reviews a document, not a model. It makes no claim about whether any model is safe, and no claim about the intentions of any developer.

---

## What is Here

| Path | Content |
| :--- | :--- |
| `METHOD.md` | Criteria, rating scale, process |
| `criteria.csv` | The 11 reporting criteria plus one judgment criterion |
| `LIMITS.md` | What this work cannot show |
| `cases/gpt-5-6/` | Case study: OpenAI GPT-5.6 System Card (sections 3.1.2, 7.1, 7.2, 7.4) |
| `template/` | Empty CSV sheets to review another card |
| `CHANGELOG.md` | Versions and corrections |

---

## Case Study at a Glance (11 evaluations, 5 claims)

Our first case study evaluates sections of the OpenAI GPT-5.6 System Card (published 9 July 2026). Key findings regarding reporting completeness include:
* **Number of runs stated:** 0 of 11.
* **Sample size fully stated:** 0 of 11 (4 partly; several counts can only be derived from figures).
* **Uncertainty fully reported:** 4 of 10 applicable.
* **Automated grader validated against human labels:** 0 of 8 applicable (1 partly).
* **Decision threshold justified:** 0 of 10 applicable (2 partly).
* **Conclusion follows from the data shown:** Yes: 1 | Partly: 8 | Cannot tell: 2.

**What the card does well:** Counts behind rates are shown in two figures, the lack of multiple-comparison correction is stated openly, and simulation fidelity is measured against a noise funnel. See the full report in `cases/gpt-5-6/` for details, specific pointers, and open questions.

---

## Responsible Communication & Disclosure

As part of standard AI audit and Model Risk Management (MRM) practices, a draft of this review along with formal methodological questions was shared with the OpenAI Security team on **November 6, 2026** (Ticket initiated). 

The repository will be updated to reflect any clarifications, corrections, or feedback provided by the authors. If no response is received within the specified review period, the open questions will remain as part of the public audit record to encourage reproducible reporting standards.

---

## How to Read the Results

* **"Not reported"** means not visible to the reviewer in the public document, not that the work was not done by the developers.
* **Findings** are strictly labeled as either *fact* or *interpretation*. Consequence ratings are indicative, based on a single-reviewer paradigm.
* **Sample sizes** derived from figures are explicitly marked as *'derived'*.
* The analyzed card was accessed on **19 October 2026**; changes made after this date are not reflected.

---

## How to Reuse This Framework

This methodology is designed to be lab-agnostic. To audit a different system card:
1. Copy the blank files from the `template/` directory.
2. Follow the evaluation process outlined in `METHOD.md`.
3. Rate the document against the 11 pre-defined criteria in `criteria.csv`.

---

## Independence

This is an independent, educational work. The author has no financial or personal ties to the developer, did not take part in the design, training, or testing of the system, and is not affiliated with or endorsed by OpenAI. The card's content is paraphrased, not quoted, and referenced strictly by section and figure numbers.

## Corrections

If you are an author of a reviewed document, or you spot a factual error, please open an issue or write to `[your-contact-email]`. Factual corrections will be applied promptly and recorded in `CHANGELOG.md`.

## License

* **Text and Data:** [CC BY 4.0](https://creativecommons.org)
* **Code (if any):** [MIT](https://opensource.org)
