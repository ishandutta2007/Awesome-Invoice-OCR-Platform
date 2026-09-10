# Awesome-Invoice-OCR-Platform

## Top Invoice OCR Platforms Ecosystem
**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on Invoice Data Extraction, Intelligent Document Processing, Field Recognition, Line-Item Parsing & AP Automation*
**Last updated: September 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Invoice OCR** and intelligent document processing. These systems extract structured data (vendor, dates, amounts, line items, tax, etc.) from invoices, receipts, and related financial documents with high accuracy and minimal templates.

**Examples** include Rossum, Nanonets, Veryfi, Klippa, Hypatos, Docsumo, Mindee, ABBYY FlexiCapture / Vantage, Ocrolus, and Base64.ai (the category leaders).

**Open-source emphasis**: Full end-to-end commercial Invoice OCR / IDP platforms are mostly proprietary. Strong open foundations exist in **OCR engines (PaddleOCR, Tesseract, EasyOCR, docTR)** and **document understanding models (LayoutLM family and fine-tunes)**. This section prioritizes these building blocks and community pipelines.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms
- **[Rossum](https://rossum.ai/)**  
  AI-native invoice and document understanding platform with strong extraction accuracy, validation workflows, and AP automation features.

- **[Nanonets](https://nanonets.com/)**  
  No-code / low-code document AI platform popular for custom model training, invoice extraction, and workflow automation.

- **[Veryfi](https://www.veryfi.com/)**  
  Developer-focused OCR and data extraction API specializing in receipts, invoices, and financial documents with mobile SDKs.

- **[Klippa](https://www.klippa.com/)**  
  Document and spend-management platform with high-accuracy invoice and receipt OCR, especially strong in European markets.

- **[Hypatos](https://hypatos.ai/)**  
  AI-powered invoice and document processing platform aimed at enterprise accounts-payable automation.

- **[Docsumo](https://www.docsumo.com/)**  
  Intelligent document processing platform with pre-trained models for invoices and financial documents plus API-first design.

- **[Mindee](https://www.mindee.com/)**  
  Developer-centric document AI API with pre-trained invoice and receipt models and easy integration.

- **[ABBYY FlexiCapture / Vantage](https://www.abbyy.com/)**  
  Enterprise intelligent document processing suite with advanced OCR, classification, and highly customizable extraction (cloud and on-prem options).

- **[Ocrolus](https://www.ocrolus.com/)**  
  Document AI platform focused on financial document analysis, including bank statements and related forms (invoice capabilities vary by offering).

- **[Base64.ai](https://base64.ai/)**  
  Document extraction API supporting invoices and a wide range of structured and semi-structured documents.

## Open-Source GitHub Projects
- **[PaddleOCR](https://github.com/PaddlePaddle/PaddleOCR)**  
  High-performance open-source OCR toolkit (Apache 2.0) with strong layout analysis and table recognition (PP-Structure) — excellent foundation for invoice pipelines.

- **[Tesseract OCR](https://github.com/tesseract-ocr/tesseract)**  
  Classic, widely used open-source OCR engine. Still a reliable building block when combined with modern layout and extraction layers.

- **[EasyOCR](https://github.com/JaidedAI/EasyOCR)**  
  Ready-to-use open-source OCR library supporting 80+ languages with simple Python API.

- **[docTR](https://github.com/mindee/doctr)**  
  Open-source document text recognition library from Mindee, focused on end-to-end OCR for documents.

- **[LayoutLM / LayoutLMv3 and fine-tunes](https://github.com/microsoft/unilm)**  
  Document understanding models that combine text and layout information — frequently fine-tuned for invoice field extraction.

- **[Invoice-specific LayoutLM fine-tuning projects](https://github.com/)**  
  Community repositories that fine-tune LayoutLMv2/v3 on invoice datasets for key-value and line-item extraction.

- **[PaddleOCR + LLM invoice parsers](https://github.com/)**  
  Pipelines that use PaddleOCR for text detection/recognition and an LLM for intelligent field parsing and structuring.

- **[invoice2data and rule-based extractors](https://github.com/)**  
  Older but still useful open tools that combine OCR with template or regex-based field extraction for known invoice formats.

- **[Donut, TrOCR, and other document Transformers](https://github.com/)**  
  Vision-language models adapted for document OCR and information extraction without traditional OCR pipelines.

- **[Label Studio + OCR annotation pipelines](https://github.com/)**  
  Open annotation and training workflows used to create custom invoice extraction datasets.

### Additional Strong Open-Source Options
- Building a pipeline with **PaddleOCR (PP-Structure)** for text + tables, then post-processing with rules or a small LLM.
- Fine-tuning **LayoutLMv3** on your own invoice set for higher field-level accuracy.
- Using **Tesseract or EasyOCR** as a lightweight first stage for clean, high-quality scans.
- Combining open OCR with open validation rules (totals, tax calculations, vendor matching) for human-in-the-loop review.
- Accepting that commercial platforms still lead on out-of-the-box accuracy across thousands of vendor formats, continuous model improvement, and full AP workflow integration.

**Frameworks for building custom systems**: Pre-process images → run open OCR (PaddleOCR / Tesseract) → apply layout-aware models (LayoutLM fine-tunes) or LLM parsing → validate extracted fields → export structured JSON/CSV to ERP or accounting systems. This stack is fully open and controllable. Commercial platforms (Rossum, Nanonets, Veryfi, Mindee, ABBYY, Docsumo, etc.) remain the practical choice when you need high straight-through processing rates, minimal engineering effort, and enterprise support at scale.

## How to Contribute
1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer
- This is a **community-curated** list — not exhaustive and not an endorsement.
- Invoice data is financial and often sensitive. Ensure proper access controls, encryption, retention policies, and compliance with accounting and data-protection regulations. Open-source OCR pipelines require continuous accuracy validation, especially across new vendors and languages. Always keep a human review step for high-value or exception cases. This list is not financial, accounting, or compliance advice.

---
**Made for AP automation teams, fintech engineers, and developers who need reliable invoice data extraction.**
Let's keep document understanding accurate, auditable, and as open as the use case allows.
