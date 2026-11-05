# System card reporting review

A reusable method, and a first case study, for checking **how well an AI system card reports the evidence behind its conclusions**.

> **This is not a safety assessment.** It reviews a document, not a model. It makes no claim about whether any model is safe, and no claim about the intentions of any developer.

## What is here

| Path | Content |
|---|---|
| `METHOD.md` | Criteria, rating scale, process |
| `criteria.csv` | The 11 reporting criteria plus one judgment criterion |
| `LIMITS.md` | What this work cannot show |
| `cases/gpt-5-6/` | Case study: OpenAI GPT-5.6 System Card (sections 3.1.2, 7.1, 7.2, 7.4) |
| `template/` | Empty CSV sheets to review another card |
| `CHANGELOG.md` | Versions and corrections |

## Case study at a glance (11 evaluations, 5 claims)

- Number of runs stated: 0 of 11.
- Sample size fully stated: 0 of 11 (4 partly; several counts can only be derived from figures).
- Uncertainty fully reported: 4 of 10 applicable.
- Automated grader validated against human labels: 0 of 8 applicable (1 partly).
- Decision threshold justified: 0 of 10 applicable (2 partly).
- Conclusion follows from the data shown: yes 1, partly 8, cannot tell 2.

The card also does several things well: counts behind rates are shown in two figures, the lack of multiple-comparison correction is stated openly, and simulation fidelity is measured against a noise funnel. See the report for details and for each finding's wording, pointer and open question.

## How to read the results

- "Not reported" means *not visible to the reviewer in the public document*, not *not done*.
- Findings are labelled fact or interpretation. Consequence ratings are indicative, from one reviewer.
- Some sample sizes were derived from figures and are marked "derived".
- The card was accessed on 19 October 2026; later changes are not reflected.

## Independence

Independent, educational work. The author has no financial or personal ties to the developer, did not take part in the design, training or testing of the system, and is not affiliated with or endorsed by OpenAI. The card is paraphrased, not quoted, and referenced by section and figure.

## Corrections

If you are an author of a reviewed document, or you spot a factual error, please open an issue or write to [contact]. Factual corrections are applied promptly and recorded in `CHANGELOG.md`.

## License

Text and data: CC BY 4.0. Code, if any: MIT.
