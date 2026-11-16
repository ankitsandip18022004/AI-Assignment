AI Assignment 2026 - Classical AI Reasoning Agent

OVERVIEW
This project implements an AI reasoning agent that predicts whether a query is supported by a knowledge base. It uses classical reasoning techniques rather than asking a generative AI system to provide the final True/False answer.

SUBMISSION FILES
- reasoning_agent.ipynb : Notebook containing the implementation and evaluation.
- report.pdf             : Short report describing representations, reasoning algorithms, experiments, and example traces.
- submission.csv         : CSV containing prediction IDs and labels.

IMPLEMENTATION
The notebook includes reasoning components for:
- Rule-based inference using forward chaining, backward chaining, and unification.
- First-order logic parsing and logical inference for FOLIO-style examples.
- Counterfactual reasoning for CounterBench-style examples.

HOW TO RUN
1. Open reasoning_agent.ipynb in the notebook environment used for the project (for example, Google Colab).
2. Make sure the public dataset files expected by the notebook are available at the paths configured in the notebook.
3. Run the notebook cells in order.
4. Review the printed evaluation accuracy and inference-time results.
5. Run the submission-generation cell to create submission.csv.

INPUTS AND OUTPUTS
The notebook expects the dataset files and paths specified in its data-loading cells. It generates predictions in submission.csv. The CSV should contain the required identifier and predicted-label columns.


