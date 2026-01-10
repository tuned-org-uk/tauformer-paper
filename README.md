# Topological Transformer: A Redesign of the Transformer Architecture

[![DOI](https://img.shields.io/badge/DOI-10.36227%2Ftechrxiv.176800983.30631144%2Fv1-blue)](https://doi.org/10.36227/techrxiv.176800983.30631144/v1)

Starting from prior research on topological spaces for vector search (spectral search with *taumode*), this paper introduces the definition, a concept implementation, and tests for a new class of Transformers focused on improving the attention mechanism.

The **Topological Transformer** (*Tauformer*) preserves the standard attention-based Transformer features (with *nanoGPT* as the baseline) but redesigns attention at its core to:

- Deliver domain-specific context directly within the attention mechanism for more domain-relevant token generation.
- Improve time per token by ~20% and reduce KV-cache memory size by ~50%.
- Provide a pathway to better performance on larger context windows (longer prompts) and high-dimensional embeddings.

These gains are enabled by substituting the standard inner-product attention kernel with *taumode*’s synthetic index–based distance, aiming for meaningful linear improvements in training and generation compared to current GPT-style models.

Paper: https://github.com/tuned-org-uk/tauformer-paper/blob/main/Topological%20Transformer-uploaded%20version.pdf

Code: https://github.com/tuned-org-uk/tauformer

Bench: https://github.com/tuned-org-uk/taugpt-kvcache-bench

Copyright 2025-2026 Lorenzo Moriondo
