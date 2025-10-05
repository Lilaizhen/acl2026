# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with research paper LaTeX files in this repository, incorporating best practices from successful ML research papers.

## Project Overview

This repository contains the complete LaTeX source for a research paper to be submitted to ACL (Association for Computational Linguistics). The writing follows established guidelines for impactful computational linguistics research papers, using the official ACL style files and formatting requirements.

## Document Structure

### Main Paper
`paper.tex` - Main LaTeX document that compiles the entire paper, including all sections and components.

### Paper Components
- `abstract.tex` - Research summary and key contributions
- `intro.tex` - Introduction, motivation, and research questions
- `related.tex` - Related work
- `method.tex` - Methodology and algorithmic approach
- `results.tex` - Experimental evaluation and results
- `conclusion.tex` - Conclusions and future work
- `appendix.tex` - Supplementary material and proofs

### Supporting Files
- `common.tex` - Shared LaTeX commands and packages
- `math_commands.tex` - Mathematical notation and definitions
- `reference.bib` - Main bibliography in BibTeX format
- `custom.bib` - Custom bibliography entries
- `anthology.bib` - ACL Anthology bibliography database
- `acl.sty` - ACL conference style package
- `acl_natbib.bst` - ACL bibliography style file

### Algorithms (`algorithms/`)
- `overview.tex` - High-level algorithm overview

### Figures (`figures/`)
- `overview.pdf` - System architecture diagram

### Tables (`tables/`)
- `compare.tex` - Main Comparisons
- `ablation.tex` - Ablation study results

## Research Paper Structure

### Key Sections Overview

**Abstract** (`abstract.tex`):
- ...

**Introduction** (`intro.tex`):
- ...

**Methodology** (`method.tex`):
- ...

**Experiments** (`results.tex`):
- ...

**Conclusion** (`conclusion.tex`):
- ...

**Appendices** (`appendix.tex`):
- ...

## Research Paper Writing Guidelines

Based on established best practices for successful ML research papers:

### Core Writing Principles
- **Audience**: Write for researchers in closely related fields who don't know your specific topic
- **Insights over novelty**: Focus on novel understanding rather than just technical innovations
- **Self-contained**: Make the paper fully understandable without requiring knowledge of previous work
- **Scientific method**: Follow Observation → Hypothesis → Test → Analysis structure
- **Critical analysis**: Identify limitations and potential weaknesses before reviewers do
- **Appropriate complexity**: Use math/formulas only when they aid understanding, not to appear sophisticated

### Writing Process
- **Concept before writing**: Have final results and complete analysis before writing (except introduction)
- **Abstract last**: Write the abstract after completing the entire paper to properly summarize key insights
- **Introduction early**: Start writing the introduction to clarify research questions and identify related work

### Content Quality Principles
- Clear motivation explaining why research matters
- Novel insights supported by thorough analysis
- Self-contained presentation without external dependencies
- Scientific method structure with formal hypothesis testing
- Identified and discussed limitations
- Appropriate use of mathematical notation
- Complete results and analysis before writing begins

## Editing Guidelines

### LaTeX Conventions
- Use semantic line breaks for git-based collaboration convention and avoid long lines of source text
- Use definitions in `common.tex` for shared commands and packages
- General mathematical notation defined in `math_commands.tex`
- Algorithmic descriptions in `algorithms/` directory

### Figure Management
- Source files in `figures/` with `.tex` for TikZ diagrams
- Generated plots have corresponding `.py` scripts
- Use `\includegraphics` with appropriate scaling for PDF figures
- Maintain consistent styling across all visualizations

### Citation Style
- BibTeX entries in `reference.bib`, `custom.bib`, and `anthology.bib`
- Use `\cite{}` for inline citations
- ACL supports natbib citation commands: `\citep{}`, `\citet{}`, `\citealp{}`, `\citeyearpar{}`, `\citeposs{}`

### Reproducibility Standards
- All hyperparameters listed with ranges explored
- Source code and computing infrastructure specified
- Evaluation metrics formally defined
- Algorithms used for each result clearly stated
- Experimental analysis goes beyond single metrics
