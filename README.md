# Agent-as-a-Judge: Multi-Agent Pipeline for RAG Evaluation

[![Paper](https://img.shields.io/badge/Paper-PDF-red.svg)](./Agent_Judgement_Paper.pdf) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This repository contains the official code and data for the paper: **"Can a Multi-Agent Pipeline Effectively Simulate Human Reasoning in RAG Evaluation?"**

The project introduces a multi-agent framework designed to automate the evaluation of Retrieval-Augmented Generation (RAG) systems. We compare two distinct LLM-based evaluation paradigms:
1. **Pointwise Grading System:** Maps qualitative errors to strict numerical penalties.
2. **Pairwise Comparison System:** Evaluates two responses head-to-head based on a qualitative weight-of-evidence analysis.

Our findings demonstrate that LLMs struggle with absolute numerical grading but show significant improvements when utilizing structured, language-based pairwise comparisons.

## Repository Structure

This project is divided into two main submodules to separate the evaluation logic from the user interface:

- 🧠 **[Backend Repository](https://github.com/CuzImAram/aaaj-backend)**: Contains the `n8n` workflow files, Python evaluation scripts and the generated outputs.
- 🖥️ **[Frontend Repository](https://github.com/CuzImAram/aaaj-frontend)**: A web-based application to manually test, visualize, and interact with the Pairwise Comparison System.