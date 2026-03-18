#Read Me

# Linguatrain Language Packs

This repository contains language packs and localisation files for use with **Linguatrain**.

It is designed to be a clean, structured, and community-friendly way to share and contribute language learning content across multiple languages.

---

## 🔗 Linguatrain

Linguatrain project repository:

https://github.com/wbrisett/linguatrain

---

## ▶️ Getting Started

To use these packs, see the Linguatrain Quick Start guide:

https://github.com/wbrisett/linguatrain

---

## 📦 About These Packs

These starter packs are provided to demonstrate what can be built with Linguatrain and to highlight that it is a **multi-language tool**, not designed for any single language.

Most packs in this repository currently use an English → target language setup. However, Linguatrain is not limited to English. Any language pairing can be used. For example:

- German ↔ Italian
- Spanish ↔ French
- Finnish ↔ Swedish

If the community creates packs for other language pairs, they will work just as well.

---

## ⚠️ Important Note

I am not a native speaker of the sample languages included here. AI tools were used to help generate and refine these packs.

As a result:

- Some phrasing may not reflect natural, everyday usage
- Some teaching patterns may not align perfectly with native instruction methods

These packs are intended as **examples and starting points**, not authoritative sources.

Community contributions, corrections, and improvements are strongly encouraged.

---

## 📁 Repository Structure

```
.
├── localisation/
├── packs/
│   ├── <language>/
│   └── templates/
└── readme.md
```

### localisation/

Contains UI localisation files that control:

- Language pairing (source → target)
- Text-to-speech (TTS) templates
- UI labels and feedback messages

Example:

```
localisation/en-US_fi-FI.yaml
```

---

### packs/

Contains all language learning content.

Each language has its own directory:

```
packs/fi/
packs/de/
packs/es/
packs/fr/
```

Each directory contains multiple pack types:

- `*_basic_phrases.yaml`
- `*_numbers.yaml`
- `*_days_and_months.yaml`
- `*_common_colors.yaml`
- `*_conjugate.yaml`
- `*_transform.yaml`

---

### templates/

Starter templates for building new packs:

- `linguatrain_pack_minimum_template.yaml`
- `linguatrain_pack_complete_template.yaml`
- `linguatrain_pack_conjugate_template.yaml`
- `linguatrain_pack_transform_template.yaml`

Use these as the basis for new contributions.

---

## 🧠 Pack Types

### 1. Standard Packs

Vocabulary and phrase-based learning.

```yaml
prompt: "Hello"
answer:
  - "Hei"
phonetic: "HAY"
```

---

### 2. Conjugate Packs

Verb conjugation drills.

- Defined by `metadata.drill_type: "conjugate"`
- Organized by grammatical person

---

### 3. Transform Packs

Cue-based grammar drills.

- Defined by `metadata.drill_type: "transform"`
- Use prompts + cues + transformation steps

---

## 🧩 Naming Conventions

### Packs

```
<language_code>_<pack_name>.yaml
```

Examples:

- `fi_basic_phrases.yaml`
- `de_conjugate.yaml`
- `es_transform.yaml`

---

### Localisation

```
<source>_<target>.yaml
```

Examples:

- `en-US_fi-FI.yaml`
- `en-US_de-DE.yaml`

---

## ✍️ Contributing

Contributions are welcome.

### Guidelines

- Follow existing structure and naming conventions
- Use templates from `packs/templates/`
- Keep packs **consistent across languages when possible**
- Ensure translations are natural and beginner-friendly
- Validate YAML formatting

---

## 🚀 Design Principles

- **Consistency over complexity**
- **Cross-language alignment**
- **Beginner-friendly content**
- **Separation of content and UI (packs vs localisation)**

---

## 📌 Notes

- `schema_version: 1` should be included in all packs
- Metadata fields should remain minimal and meaningful
- Localisation controls presentation, not content

---

This repository is intended to grow into a shared library of high-quality, structured language learning content for Linguatrain.
