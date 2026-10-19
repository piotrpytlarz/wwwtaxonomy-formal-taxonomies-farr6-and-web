---
language:
  - en
  - pl
license: cc-by-4.0
pretty_name: "wwwtaxonomy.com — Formal Combinatorial & Faceted Taxonomies: FARR/6 (57 Hybrid Intersections) & Web Functional Modules Taxonomy v3.0 (26 Archetypes, 88 Boundary Rules)"
description: "Open dataset of two formal classification systems from https://wwwtaxonomy.com: (1) FARR/6, a combinatorial taxonomy of William Farr's 6 classes of violent/unnatural death with all 57 formal hybrid intersections (orders 2 to 6) and 6 analytical axes; and (2) WWW Taxonomy v3.0, a bilingual (EN/PL) faceted taxonomy of web functional modules (4 N/P/O/R gates, 5 families, 26 leaf archetypes, 88 binary boundary rules, and 12 composite test cases)."
size_categories:
  - n<1K
task_categories:
  - text-classification
  - zero-shot-classification
tags:
  - taxonomy
  - classification
  - faceted-classification
  - combinatorics
  - web-architecture
  - nosology
  - william-farr
  - knowledge-organization
---

# wwwtaxonomy.com — Formal Combinatorial & Faceted Taxonomies Dataset (FARR/6 & WWW Taxonomy v3.0)

An open dataset of formal classification models, combinatorial lattices, and binary boundary decision rules from **[wwwtaxonomy.com](https://wwwtaxonomy.com/)**, containing two complete taxonomic systems developed in the project:

1. **FARR/6 — Combinatorial Atlas of Six Violent Deaths (`farr6-combinatorial-hybrids-57.*`):**
   Reconstructs William Farr's historical nosological division of violent deaths (1852/1856: *Battle*, *Homicide*, *Execution*, *Suicide*, *Surgical treatment*, *Accident*) across **6 analytical axes** (*cause vs. social frame*, *actor*, *intent*, *consent*, *institutional mandate*, *unit of analysis*) and exhaustively maps all **$2^6 - 6 - 1 = 57$ non-empty formal hybrid intersections** of orders 2 through 6 ($15$ pairs + $20$ triples + $15$ quadruples + $6$ quintuples + $1$ sextuple), annotated with lexical attestation status (`attested`, `partial`, `atlas`), ontological scope (`single-death`, `causal-chain`, `multi-death-event`, `status-hybrid`), coherence level, and legal/medical/military sources (WHO ICD-10, ICRC, WMA, AMA, CPOST, Polish Supreme Court).
2. **WWW Taxonomy v3.0 — Functional Archetypes of Web Service Modules (`web-functional-archetypes-taxonomy-v3.*` & `web-taxonomy-boundary-rules-88.*`):**
   A bilingual (**English & Polish**) operational taxonomy for classifying web projects by the **functional outcome delivered to the user**, rather than vague industry labels. Uses a strict four-gate priority cascade (**`N` Multi-sided network → `P` Persistent workspace → `O` Operator fulfillment → `R` Session runtime → `Fallback` Publishing & Reference**) partitioning **5 families** and **26 mutually exclusive leaf archetypes**, backed by **88 binary Yes/No boundary rules**, planning facets (`U`, `D`, `T`, modifiers), and **12 composite multi-module test cases**.

- **Live Interactive Atlas & Classifier:** [https://wwwtaxonomy.com/](https://wwwtaxonomy.com/)

---

## Package Contents (`open-data/`)

| File | Records | Description |
| --- | ---: | --- |
| `farr6-combinatorial-hybrids-57.json` / `.csv` | **57 hybrids** (+ 6 base types, 6 axes, 8 boundary scenarios) | Complete combinatorial lattice of orders 2, 3, 4, 5, and 6 over `{battle, homicide, execution, suicide, surgery, accident}` with titles, English/Polish aliases, attestation status, scope, coherence, exemplar scenarios, boundary conditions, and source URLs. |
| `web-functional-archetypes-taxonomy-v3.json` / `.csv` | **36 taxonomy nodes** (incl. **26 leaf archetypes** & **5 families**) | Full bilingual (EN/PL) hierarchy of web functional modules, formal definitions, scope notes, planning facets (`U`, `D`, `T`), and 12 composite test cases. |
| `web-taxonomy-boundary-rules-88.json` / `.csv` | **88 boundary rules** (EN + PL) | Exact binary (`Yes` / `No`) decision questions resolving boundary disputes between adjacent web archetypes and families. |

---

## License & Citation (CC BY 4.0)

This dataset is licensed under **[Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)**.

When referencing or reusing these taxonomies in classification research, ontology engineering, or LLM zero-shot classification benchmarks, please cite:

> **Source:** Piotr Pytlarz, *wwwtaxonomy.com — Formal Combinatorial & Faceted Taxonomies (FARR/6 & WWW Taxonomy v3.0)* ([https://wwwtaxonomy.com](https://wwwtaxonomy.com)), licensed under CC BY 4.0.

```bibtex
@dataset{wwwtaxonomy_formal_taxonomies_2026,
  title        = {wwwtaxonomy.com: Formal Combinatorial and Faceted Taxonomies (FARR/6 and WWW Taxonomy v3.0)},
  author       = {Pytlarz, Piotr},
  year         = {2026},
  version      = {1.0.0},
  publisher    = {wwwtaxonomy.com},
  url          = {https://wwwtaxonomy.com/},
  license      = {CC-BY-4.0}
}
```
