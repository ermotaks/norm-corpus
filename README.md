# norm-corpus
Normative sentences corpus for Norm sentence decomposition (Täks XML/CSV model)

Stanza vs spaCy Norm-Analysis

This project supports the article "From Norm Fragments to Semantic Units", which aims to structure legal provisions into semantic units and compare different NLP tools for norm-sentence decomposition.

1. Project Objective

The goal of Article 1: "From Norm Fragments to Semantic Units" is to formalize a repeatable method for breaking down legal norms into atomic semantic units (subject–predicate–object–condition). The ultimate aim is to reduce ambiguity in legal texts and enable machine reasoning on processed norm data.

The main objectives are:

Decompose norm sentences into an XML/CSV model.

Compare NLP tools (spaCy vs. Stanza) in tokenization, POS tagging, and dependency parsing.

Cross-validate results with manually annotated data.

2. Project Type and Use Cases

This project falls under the legal NLP domain, focusing on extracting semantic units from legal norms. The primary use cases include:

Structuring Legal Norms: Break down complex normative sentences into manageable semantic units (S–P–O–C) suitable for logic frameworks or rule-based systems.

Tool Comparison: Evaluate parsing accuracy, speed, and memory usage of spaCy versus Stanza for norm-sentence processing.

Automated Rule-Based Post-Processing: Provide core code to transform legal texts into machine-readable form and support automated inference.

Academic Research and Prototyping: Use the methodology for both writing the article and building practical prototypes in legal technology.

3. Quick Start

Follow these steps to set up the environment and run an example comparison:

Clone the repository:

git clone https://github.com/YourUsername/stanza-vs-spacy-norm-analysis.git
cd stanza-vs-spacy-norm-analysis

Create and activate a Conda environment (or use a Python virtual environment):

conda env create -f environment.yml
conda activate normnlp
# Alternatively, using pip:
# pip install -r requirements.txt

Run an example comparison using the Stanza model:

python -m src.evaluate --model stanza

To compare with spaCy, simply replace --model stanza with:

python -m src.evaluate --model spacy

Results will be saved in the results/comparisons/ directory as CSV files. Visualizations can be found in the Jupyter notebooks under the notebooks/ directory.

4. License and Author Information

License: MIT License © 2025 Ermo Täks

See the full license in the LICENSE file.

Author:

Name: Ermo Täks

Affiliation: IS Group, Tallinn University of Technology, Akadeemia tee 15A, 12169 Tallinn Estonia

Email: ermo.taks@taltech.ee

GitHub: https://github.com/ermotaks

References

Article: "From Norm Fragments to Semantic Units" (full text under composition).
