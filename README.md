# 🏦 Awakened Data Catalog

**The official inventory of Iron Bank v1.1.0** — our versioned corpus of curated wisdom nodes.

---

## What This Is

This catalog is generated directly from **Iron Bank v1.1.0**, our versioned, auditable data library. It provides metadata and statistics for all public packs — the training data equivalent of a library catalog.

**Total Public Nodes:** 255,597 (matches `catalog.json`)  
**Public Packs:** 8  
**Last Updated:** 2025-12-27

---

## 📦 Available Packs

| Pack ID | Display Name | Nodes | Avg Posterior | Description |
|---------|--------------|-------|---------------|-------------|
| `huggingface_edu` | Awakened Educational | 94,497 | 0.950 | Educational content from HuggingFace |
| `classics_lit` | Awakened Classics | 59,661 | 0.831 | Literary wisdom from classic texts |
| `arxiv_science` | Awakened Science | 44,443 | 0.845 | Core science papers from ArXiv |
| `arxiv_physics` | Awakened Physics | 26,224 | 0.759 | Physics papers from ArXiv |
| `github_code` | Awakened Code | 13,671 | 0.892 | Code wisdom from GitHub repos |
| `neurips_2024` | Awakened ML — NeurIPS 2024 | 9,938 | 0.783 | ML blueprints via Two-Pass Tri-Optic |
| `ethics_gutenberg` | Awakened Ethics | 5,276 | 0.923 | Classical philosophy from Gutenberg |
| `youtube_wisdom` | Awakened Media | 1,887 | 0.841 | Wisdom from YouTube transcripts |

**Note:** Pack IDs (e.g., `neurips_2024`) match the filenames in `packs/*.json` and the keys in `catalog.json`.

---

## 📁 File Structure

```
catalog.json              # Root catalog with all pack metadata
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

Each `packs/<pack_id>_v1.1.0.json` contains:
- Pack ID and version
- Node count
- Average posterior
- Source type distribution

---

## 🧬 Awakened Data Standard (ADS)

Every node in Iron Bank follows the 12-field ADS schema:

### Provenance
Every node tracks its source, extraction method, and lineage. You know exactly where each insight came from.

### Quality Scoring
**Posterior scores** (0.0-1.0) measure extraction confidence. Higher = more reliable.

### Human Relevance
**Warmth** indicators (high/medium/low) flag content with ethical, emotional, or human-centered significance.

### Deduplication
**Event fingerprints** (SHA-256) ensure each insight appears only once, even across multiple source documents.

### Tiering
- **Universal:** Verified, shareable, Olympus-grade (what you see here)
- **Sacred:** Internal family use only (not in this catalog)

---

## 🏗️ Iron Bank Architecture

The Iron Bank is our versioned, auditable data library:

1. **GENESIS:** Immutable snapshot of the source corpus
2. **Packs:** Domain-specific shards (physics, ethics, ML, etc.)
3. **Validation:** Pack-specific quality floors
4. **Releases:** Semantic versioning (v1.0.0 → v1.1.0)
5. **FAISS Indices:** Per-pack + omnibus for instant search

---

## 🔬 Extraction Methods

| Method | Packs | Description |
|--------|-------|-------------|
| **Two-Pass Tri-Optic** | `neurips_2024` | Section chunking → LLM K/V extraction → 3 specialized lenses |
| **Ethics Lens** | `ethics_gutenberg` | Philosophy-focused extraction with warmth requirements |
| **Science Pipeline** | `arxiv_*` | Evidence-chain extraction from academic papers |
| **Standard ADS** | All others | Core 12-field extraction with quality validation |

---

## 📈 Version History

| Version | Date | Changes |
|---------|------|---------|
| v1.1.0 | 2025-12-27 | +34,583 nodes: recovered physics, merged NeurIPS Tri-Optic, integrated USB batches |
| v1.0.0 | 2025-12-26 | Initial Iron Bank release |

---

## 🎯 Get the Data

Want access to the full dataset?

- **Samples:** See [awakened-wisdom-samples](https://github.com/holmanholdings/awakened-wisdom-samples) for taste-test files
- **Hugging Face:** [AwakenedIntelligence](https://huggingface.co/AwakenedIntelligence)
- **Enterprise:** Contact us for full pack exports, FAISS indices, and custom pipelines

---

*Built with cathedral-grade precision from Iron Bank v1.1.0.*

**The Awakened Intelligence Family 🦁**
