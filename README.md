# ocl-scispacy-match
Matching algorithm using the scispacy language models.

Please use file - scispacy_loinc_mapping_algorithm.ipynb for using the matchng algorithm

# 🧪 LOINC Mapping Pipeline

This project implements a robust pipeline to map **lab terms** (e.g., _"MCH"_, _"heart rate"_) to their most appropriate **LOINC codes**, using a combination of:

- ✅ **Axis-based matching** (`COMPONENT`, `PROPERTY`, `SYSTEM`, `METHOD`)
- 📊 **LOINC's official `COMMON_TEST_RANK`**
- 🧮 **Custom composite scoring**
- ⚙️ **Batch-based processing** for large-scale performance
- 🛠️ **Hardcoded fallbacks** for known ambiguous terms

The algorithm returns the **best match candidates** for each input term.

---

## 📦 Required Files

Make sure the following files are present in the run environment:

- `loinc.csv`
- `LoincPartLink_Primary.csv`

> These files are available for download from [https://loinc.org/downloads/loinc/](https://loinc.org/downloads/loinc/).

## UMLS Access key required
For testing purposes UMLS personal key was used for API. We need an account with production level access and use that key in the first step- labelled "# UMLS API Key — Replace this at runtime - PROVIDE THE API KEY" in scispacy_loinc_mapping_algorithm.ipynb

## The OCL Digital Public Good

This repository is not part of the [OCL Digital Public Good](https://github.com/OpenConceptLab/.github/blob/main/DIGITAL-PUBLIC-GOOD.md). That page lists the repositories that are.
