# Citation Provenance Bench

> Test whether cited sources actually support answer claims and remain traceable.

**Status:** open project seed · **License:** MIT · **Contributions:** welcome

A reproducible benchmark for claim-to-source support, source identity, and citation stability in retrieval-augmented answers.

## The question

Does each answer claim follow from its cited source, and does the citation still identify the retrieved passage after indexing changes?

## Why build this

This complements your streaming hallucination-sketches work by focusing on evidence provenance and measurable citation failures.

## First milestone

A small public-domain question set; claim/source annotations; baseline lexical and model-assisted metrics reported separately; a simple HTML comparison report.

## A first contribution

**Annotate 25 claim-and-source pairs with supported, partial, unsupported, and wrong-source labels plus a short rationale.**

See [`CONTRIBUTING.md`](CONTRIBUTING.md) for the small, reviewable contribution flow. You can also open an issue with the **good first issue** template, propose a test fixture, review a design choice, improve documentation, or help keep the scope honest. No model API key is needed for the initial milestone.

## Working principles

- Treat model output and retrieved content as untrusted input.
- Prefer deterministic controls, explicit assumptions, and reproducible fixtures.
- Use synthetic or public-domain examples; do not commit credentials, private prompts, personal data, or customer logs.
- Report limits and false positives. A benchmark score or static rule is not a security guarantee.
- Keep security tests inside local fixtures or systems you own and have permission to test.

## Research map

This seed is informed by the [OWASP GenAI Security Project](https://genai.owasp.org/), including its LLM and Agentic Application guidance, and by active open-source work such as [garak](https://github.com/NVIDIA/garak), [promptfoo](https://github.com/promptfoo/promptfoo), [LLM Guard](https://github.com/protectai/llm-guard), and [PyRIT](https://github.com/Azure/PyRIT). Each project aims for a narrow, inspectable contribution rather than a replacement for those broader tools.

[Compare star histories for garak, promptfoo, LLM Guard, and OWASP's LLM Top 10](https://star-history.com/#NVIDIA/garak&promptfoo/promptfoo&protectai/llm-guard&OWASP/www-project-top-10-for-large-language-model-applications). GitHub stars are an attention signal, not evidence of security quality.

## Join in

If this problem interests you, start with the first milestone above. Open an issue to discuss scope before building a large feature, or send a small pull request with a test and a clear explanation. Contributors from security, engineering, research, design, and documentation are all welcome.
