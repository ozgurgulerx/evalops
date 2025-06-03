# EvalOps 🧪📈  
**Continuous & Transparent Evaluation for LLM‑powered Systems**

---
## What is this repo? 🤔

**Your source for the latest in LLM evaluation.**

This repository collects and implements anything novel or new in language model evaluation—covering new research, metrics, frameworks, patterns, and practical code.

- **Continuously updated:** All new capabilities, methods, and benchmarks are regularly added.
- **Research-driven:** Includes the latest research ideas, frameworks, and implementation patterns.
- **Documentation:** Every update and new feature is published under the `docs/` folder.

> If it’s new or impactful in eval, it will be here.

I’m building it **in the open**. Expect rough edges, chatty commit messages, and constant iteration.

---

## Who is it for?
* **LLM builders** that need an easy CI gate before shipping a new model
* **Researchers** who want shareable, reproducible experiment layouts
* **Curious devs** learning best by poking around real code (all notebooks stay in‑repo)

-
---

## Repo Tour 🗺️
| Path | What you’ll find |
|------|------------------|
| `src/evalops/`   | The library – metrics, runners, CLI |
| `pipelines/`     | YAML suites: nightly, regression, smoke |
| `benchmarks/`    | Immutable results (JSON/Parquet) |
| `docs/`          | MkDocs source – guides & API ref |
| `examples/`      | 25‑line, copy‑paste scripts |
| `notebooks/`     | Exploratory scratchpad (ignored by CI) |

<div align="center">
  <img src="docs/images/flow.png" width="600" alt="EvalOps pipeline diagram (model → metrics → snapshot → dashboard)">
</div>

---

## Roadmap 🔭
- [x] Minimal CLI + Hydra config
- [ ] Streamlit diff dashboard
- [ ] Cost & energy metrics
- [ ] Cookiecutter template (`cookiecutter‑evalops`)
- [ ] HuggingFace evaluation hub integration

> ⭐ **Star the repo** to up‑vote any feature – I prioritise based on community noise.

---

## How to contribute 🤝
1. Fork & clone → `poetry install` (or `pip -r requirements.txt`)
2. Run checks: `pytest -q && ruff .`
3. Open a PR with a clear description + screenshot/GIF where useful
4. Join **Discussions** for roadmap votes & help‑wanted tasks

---

## License 📜
MIT – use it, fork it, embed it; just keep the copyright.

---

> Built with ☕ and curiosity by [Ozgur Guler](https://linkedin.com/in/ozguler). Follow along for live build threads and war‑stories.
