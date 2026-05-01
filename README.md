# ⚡ News-to-Insight: AI Cognitive Pipeline

**News-to-Insight** is an automated intelligence pipeline that transforms global news into high-impact Instagram content.

Unlike simple news scrapers, this system filters, interprets, and transcreates news through a multi-stage AI architecture using LLMs and diffusion models.

---

## 🧠 Problem: Signal vs. Noise

Most news automation tools simply collect and summarize articles, often creating more noise than insight.

This project is designed to mimic the workflow of a **Senior News Editor**:

1. **Smart Sourcing**  
   Monitors Google News across Korean and U.S. sources to detect macroeconomic, political, and social shifts.

2. **Cognitive Curation**  
   Uses Gemini 2.5 Flash Lite to prioritize stories based on market impact, relevance, and narrative value — not just recency.

3. **Editorial Synthesis**  
   Converts complex information into concise, human-centered copy optimized for Korean Instagram audiences.

4. **Visual Metaphor Generation**  
   Creates symbolic visuals with SDXL to support copyright-safe, brand-consistent storytelling.

---

## 🛠️ Technical Architecture

| Component | Technology | Role |
| :--- | :--- | :--- |
| **Orchestrator** | Python 3.10+ | Manages pipeline logic and system operations |
| **Reasoning Engine** | Gemini 2.5 Flash Lite | Curates news and generates editorial copy |
| **Vision Engine** | SDXL 1.0 (Hugging Face) | Generates contextual visual metaphors |
| **Content Extractor** | Trafilatura / gnewsdecoder | Extracts clean article text and normalizes URLs |
| **Imaging Unit** | Pillow (PIL) | Applies typography, gradients, and editorial layouts |

---

## 🚦 Project Status: MVP

Current MVP features include:

- [x] **Deduplication**  
  Prevents repeated content using a JSONL-based history blacklist.

- [x] **Redundancy**  
  Uses primary and backup article logic to improve pipeline reliability.

- [x] **Visual Branding**  
  Automatically generates editorial-style layouts with bottom-weighted gradient overlays.

- [ ] **Instagram Auto-Publishing**  
  Currently in development. Final assets are stored in `/outputs` for manual quality control before publishing.

---

## 🚀 Quick Start

### 1. Prepare the Environment

Create a `.env` file in the project root and add your API credentials:

```env
GEMINI_API_KEY=your_google_api_key
HF_TOKEN=your_huggingface_token
