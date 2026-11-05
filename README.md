# Getting Started with AI for Spatial Data

A hands-on workshop from the Center for Geographic Analysis, Harvard University. You classify one week of real **NYC 311 service requests** with **Gemma 4** (an open large language model) in Google Colab, evaluate the labels against the official complaint types, and map the results.

[**Workshop website and step-by-step instructions:**] (https://dkakkar.github.io/GenAI-for-Spatial/)

## Contents

| Folder | What's inside |
|---|---|
| `notebook/` | `Spatial_AI_Workshop_Script.ipynb`, the workshop notebook (runs in Google Colab on a free T4 GPU) |
| `slides/` | The presentation (PowerPoint and PDF) |
| `data/` | `nyc311_snapshot.csv`, a backup of the 311 data in case NYC Open Data is unavailable |
| `docs/` | The workshop website (GitHub Pages) |

## What you need

- A Google account (for Colab and Google Drive)
- A Hugging Face account and a Read access token (recommended)
- A laptop with a web browser. Nothing to install.

## Test-run results

Gemma 4 E2B on a Colab T4, 1,000 requests from 1–7 September 2026:

| Method | Accuracy | Cohen's kappa |
|---|---|---|
| P5_retrieval | 97.3% | 0.965 |
| kNN_vote (no LLM) | 95.7% | 0.945 |
| Ensemble | 91.0% | 0.885 |
| Keyword search | 73.7% | 0.660 |

## Data

NYC 311 Service Requests from [NYC Open Data](https://data.cityofnewyork.us/Social-Services/311-Service-Requests-from-2010-to-Present/erm2-nwe9). Street addresses are not included.

## Contact

Devika Jain, Center for Geographic Analysis, Harvard University · kakkar@fas.harvard.edu
