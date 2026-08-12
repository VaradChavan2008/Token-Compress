# 🧠 Token-Diet: Dynamic Context Compressor

![Status](https://img.shields.io/badge/Status-Prototype_Active-brightgreen)
![Hackathon](https://img.shields.io/badge/Hackathon-VCET_Arcade-blue)
![Team](https://img.shields.io/badge/Team-CodeBlooded-red)
![UI](https://img.shields.io/badge/UI-Liquid_Glassmorphism-purple)

**A post-retrieval optimization pipeline inserted between the vector database and the LLM to drastically reduce API costs and TTFT latency.**

---

## 🚨 The Problem
Traditional Retrieval-Augmented Generation (RAG) engines blindly pass massive, unfiltered paragraphs into LLM context windows. This bloated context balloons the Time-To-First-Token (TTFT) latency and drives AI API costs through the roof, especially at enterprise scale.

## 💡 Our Solution
**Token-Diet** intelligently compresses retrieved context *before* it ever reaches the model, without altering the underlying data architecture. Inspired by models like Microsoft's LLMLingua, this prototype demonstrates how a local NLP filtering layer can aggressively strip conversational filler, pronouns, and non-essential tokens while preserving the core semantic meaning.

### ✨ Key Prototype Features
* **Zero-Setup Execution:** Runs entirely in the browser using React (via CDN) and vanilla JavaScript. No backend server required.
* **Lexical NLP Filter:** Utilizes a custom, highly optimized $O(1)$ Stop-Word Dictionary mapping to strip bloat while intelligently preserving punctuation boundaries.
* **Live Telemetry Dashboard:** Calculates and displays real-time metrics, including Original vs. Compressed Token counts, actual Compression Ratios, TTFT Latency Drops (ms), and projected GPT-4 API cost savings.
* **Liquid Glassmorphism UI:** A luxury-grade, dual-theme (Dark/Light) interface utilizing a custom Alabaster, Racing Red, and Black Cherry color palette.

---

## 🚀 How to Run the Demo

Because this prototype is designed for instant accessibility, there are no heavy dependencies or package installations required.

1. Clone this repository to your local machine:
   ```bash
   git clone [https://github.com/yourusername/Token-Diet-Compressor.git](https://github.com/yourusername/Token-Diet-Compressor.git)
