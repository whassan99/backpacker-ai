# Backpacker AI

A RAG-based travel chatbot built for solo backpackers and budget travelers.

## The Problem

Planning a budget trip is time-consuming and noisy — travel sites are packed with tourist-resort fluff, and the practical details a backpacker actually needs (real hostel costs, which bus to take, visa-on-arrival rules, street food spots) are buried or outdated. Solo travelers need fast, honest, ground-level answers, not sponsored listicles.

## What It Does

The user asks a plain-language question about a destination — things like "How do I get from Bangkok to Chiang Mai on the cheap?", "Do I need a visa for Vietnam as a UK passport holder?", or "What's a realistic daily budget in Lisbon?" — and the system retrieves relevant backpacker-sourced data and returns a concise, no-fluff answer. No hotel recommendations, no tour packages. Just the practical info you need when you're living out of a single bag.

## Setup

1. Install uv if you don't have it yet: https://docs.astral.sh/uv/getting-started/installation/

2. Clone this repository (or download the zip and extract it).

3. Create a `.env` file from the template and add your API key:

       cp .env.example .env

4. Install dependencies:

       uv sync

5. Start Jupyter:

       uv run jupyter notebook

## Notebooks

- `notebooks/01-setup.ipynb` - smoke test that confirms your environment works
- `notebooks/02-rag.ipynb` - a minimal RAG baseline you can adapt to your own data

## Data

Put your project data in the `data/` folder. See `notebooks/02-rag.ipynb` for how to load it.
