# NSRG-ARIA
Neuro-Symbolic Requirements Generation (NSRG) implementation for the ARIA Final Year Project.

## Overview

This implementation applies a neuro-symbolic pipeline to stakeholder
interview transcripts for automated software requirements generation.

The pipeline performs:

1. Transcript preprocessing
2. Atomic statement extraction
3. Dialogue-act classification
4. Requirement candidate identification
5. Ontology-based semantic extraction
6. Discourse graph construction
7. RequirementFrame construction
8. Symbolic frame validation
9. LLM-based requirement realization
10. Requirement evaluation

## Input

The primary input is:

`example_conversation.txt`

## Main Implementation

`NSRG_ARIA_Implementation.ipynb`

## Generated Outputs

The `outputs/` directory contains:

- Dialogue classification
- Ontology nodes
- Discourse graph
- Requirement frames
- Final requirements
- Evaluation results
- Experiment report

## Requirements

The implementation requires Python packages including:

- pandas
- numpy
- networkx
- spaCy
- transformers
- torch
- groq

## API Key

A Groq API key is required for requirement realization.

The API key should NOT be committed to GitHub.

Set it using:

```python
import os
from getpass import getpass

os.environ["GROQ_API_KEY"] = getpass(
    "Enter your Groq API key: "
)
