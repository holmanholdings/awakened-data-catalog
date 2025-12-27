# 🏦 Awakened Data Catalog

**Version:** v1.1.0  
**Last Updated:** December 27, 2025  
**Source:** Iron Bank v1.1.0

---

## What This Is

The official catalog of all public **Awakened Data Standard (ADS)** packs. This repo contains metadata and statistics for our wisdom node collections—the training data equivalent of a library catalog.

## 📊 Iron Bank v1.1.0 Statistics

| Metric | Value |
|--------|-------|
| **Total Validated Nodes** | 255,597 |
| **Public Packs** | 8 |
| **Last Updated** | 2025-12-27 |

### Available Packs

| Pack | Nodes | Avg Posterior | Description |
|------|-------|---------------|-------------|
| `huggingface_edu` | 94,497 | 0.950 | Educational content from HuggingFace |
| `classics_lit` | 59,661 | 0.831 | Literary wisdom from classic texts |
| `arxiv_science` | 44,443 | 0.845 | Core science papers from ArXiv |
| `arxiv_physics` | 26,224 | 0.759 | Physics papers from ArXiv (WO-PHYS-03) |
| `github_code` | 13,671 | 0.892 | Code wisdom from GitHub repos |
| `neurips_2024` | 9,938 | 0.783 | ML blueprints via Two-Pass Tri-Optic extraction |
| `ethics_gutenberg` | 5,276 | 0.923 | Classical philosophy from Gutenberg |
| `youtube_wisdom` | 1,887 | 0.841 | Wisdom extracted from YouTube transcripts |

## 📁 File Structure

```
catalog.json           # Root catalog with all pack metadata
packs/
  arxiv_physics_v1.1.0.json
  arxiv_science_v1.1.0.json
  classics_lit_v1.1.0.json
  ethics_gutenberg_v1.1.0.json
  github_code_v1.1.0.json
  huggingface_edu_v1.1.0.json
  neurips_2024_v1.1.0.json
  youtube_wisdom_v1.1.0.json
```

## 🧬 What is the Awakened Data Standard (ADS)?

The Awakened Data Standard is a 12-field schema designed for:

### Provenance
Every node tracks its source, extraction method, and lineage. You know exactly where each insight came from.

### Quality Scoring
**Posterior scores** (0.0-1.0) measure extraction confidence. Higher = more reliable.

### Human Relevance
**Warmth** indicators (high/medium/low) flag content with ethical, emotional, or human-centered significance.

### Deduplication
**Event fingerprints** (SHA-256) ensure each insight appears only once, even across multiple source documents.

### Tiering
- **Universal:** Verified, shareable, Olympus-grade
- **Sacred:** Internal family use only (not in this catalog)

## 🏗️ Iron Bank Architecture

The Iron Bank is our versioned, auditable data library:

1. **GENESIS:** Immutable snapshot of the source corpus
2. **Packs:** Domain-specific shards (physics, ethics, ML, etc.)
3. **Validation:** Pack-specific quality floors
4. **Releases:** Semantic versioning (v1.0.0, v1.1.0, etc.)
5. **FAISS Indices:** Per-pack + omnibus for instant search

## 🔬 Extraction Methods

| Method | Packs | Description |
|--------|-------|-------------|
| **Two-Pass Tri-Optic** | `neurips_2024` | Section chunking → LLM K/V extraction → 3 specialized lenses |
| **Ethics Lens** | `ethics_gutenberg` | Philosophy-focused extraction with warmth requirements |
| **Science Pipeline** | `arxiv_*` | Evidence-chain extraction from academic papers |
| **Standard ADS** | All others | Core 12-field extraction with quality validation |

## 📈 Version History

| Version | Date | Changes |
|---------|------|---------|
| v1.1.0 | 2025-12-27 | +34,583 nodes: recovered physics, merged NeurIPS Tri-Optic, integrated USB batches |
| v1.0.0 | 2025-12-26 | Initial Iron Bank release |

## 🎯 Get the Data

Want access to the full dataset? These samples and catalogs demonstrate our quality. Contact us for:

- Full pack exports (.jsonl)
- FAISS indices for instant search
- Custom extraction pipelines
- Enterprise licensing

---

*Built with cathedral-grade precision.*

**The Awakened Financial Council 💛🦁**

