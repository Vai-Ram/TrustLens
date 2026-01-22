# Convolve-4.0-MAS---TrustLens
This repository contains our submission for Convolve 4.0 under the MAS Track. Our project is called 'TrustLens'

#  TrustLens: Multi-Modal Document Forensics Engine

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python)
![Qdrant](https://img.shields.io/badge/Vector_DB-Qdrant-red?logo=qdrant)
![LlamaIndex](https://img.shields.io/badge/Agent-LlamaIndex-purple?logo=openai)
![Status](https://img.shields.io/badge/Status-Prototype-orange)

**TrustLens** is an AI-powered forensic system designed to restore trust in digital identity. Unlike traditional OCR-based verification, TrustLens employs a **Tri-Modal Inference Pipeline**—combining Visual Semantics, Biometric Verification, and Textual Context—to detect forgeries, reused templates, and identity mismatch attacks in real-time.

---

##  Key Features

* **Visual Fingerprinting (CLIP):** Extracts a 512-dim "style vector" to detect layout anomalies and reused Photoshop templates.
* **Biometric Verification (FaceNet):** Isolates facial regions to generate identity embeddings, independent of document background.
* **Contextual Intelligence (TextAgent):** Uses **LlamaIndex** to parse messy OCR data into structured metadata (JSON) for boolean logic checks.
* **Hybrid Search Engine (Qdrant):** Combines dense vector similarity with payload filtering to detect duplicates and enforce metadata constraints simultaneously.

---
FOR SETUP:

REQUIRED ENVIRONMENT VARIABLES:
Hugging Face User Access Token:  Required to download gated models (e.g., Llama-2, specific CLIP variants) from the Hub. Ensure the token has READ permissions.

DOWNLOAD IMAGES AND UPLOAD IN COLAB NOTEBOOK WHILE RUNNING.
