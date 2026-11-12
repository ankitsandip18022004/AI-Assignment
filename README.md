# AI-Assignment
Classical Reasoning Agent – Artificial Intelligence Assignment

Student Name: Ankit Kumar  
Roll Number: M26CPS002  
Project: Artificial Intelligence Assignment

This project implements a Classical Reasoning Agent that understands natural-language statements, converts them into logical representations, and answers questions using symbolic reasoning techniques.

The system uses rule-based parsing and logical inference rather than generative AI models. It supports two major reasoning algorithms:

Forward Chaining (FC)
Backward Chaining (BC)

The project also explores closed-world and open-world reasoning semantics and includes support for causal reasoning problems.

Objectives

- Convert natural-language statements into logical facts and rules.
- Implement Forward Chaining and Backward Chaining algorithms.
- Perform logical inference to answer natural-language queries.
- Evaluate reasoning performance using the RuleTaker dataset.
- Implement causal reasoning for CounterBench-style questions.
- Compare reasoning accuracy and inference time.

Technologies Used

- Python
- Jupyter Notebook
- Pandas
- Regular Expressions
- JSON
- Logical Reasoning and Rule-Based Systems

Repository Structure

AI-Assignment/
│
├── Reasoning code.ipynb
├── report.pdf
├── results.json
│
├── mnist_train_small.csv
├── mnist_test.csv
│
├── california_housing_train.csv
├── california_housing_test.csv
│
└── README.md


Methodology

1. Natural Language Processing
Natural-language sentences are processed using regular expressions and a rule-based parser. The statements are converted into logical facts, predicates, and Horn clauses.

2. Forward Chaining
Forward Chaining is a data-driven inference technique that starts with known facts and repeatedly applies logical rules to derive new facts until the required conclusion is reached or no more facts can be generated.

3. Backward Chaining
Backward Chaining is a goal-driven inference technique. It starts with the query and works backward to determine whether the available facts and rules support the conclusion.

4. Reasoning Semantics
Two reasoning approaches are implemented:

- Closed-World Assumption (CWA): A statement is considered false if it cannot be derived from the knowledge base.
- Open-World Assumption (OWA): A statement is considered false only when its negation is explicitly established.

5. Causal Reasoning
The system also supports CounterBench-style causal reasoning using interventions and logical rules.

Experimental Results

The following results were obtained from the recorded RuleTaker evaluation.

| Evaluation Metric | Forward Chaining | Backward Chaining |
|---|---:|---:|
| Accuracy | 98.93% | 99.77% |
| Total Inference Time | 1.73 seconds | 7.35 seconds |
| Average Time per Query | 0.577 ms | 2.449 ms |

Dataset Evaluation:
- Dataset: RuleTaker
- Evaluated Samples: 3,000
- Total Available Evaluation Pool: 151,911
- Parse Failures: 0

Semantics Comparison

| Reasoning Approach | Accuracy |
|---|---:|
| Closed-World (CWA) | 98.80% |
| Open-World (OWA) | 74.17% |

Differential Testing

- Random test cases generated: 4,000
- Stratifiable cases: 3,918
- Total disagreements between FC and BC: 16
- Disagreements on stratifiable programs: 0

Note:FOLIO and CounterBench were not evaluated in the reported experimental run because their datasets were unavailable during report generation.

How to Run the Project

1. Clone this repository:

git clone YOUR_GITHUB_REPOSITORY_URL


2. Open the project folder.

3. Install the required Python libraries:

pip install pandas datasets reportlab

4. Open `Reasoning code.ipynb` using Jupyter Notebook or Google Colab.

5. Execute the notebook cells sequentially.

6. Review the reasoning outputs, evaluation metrics, and generated results.

Project Files Description

| File | Description |
|---|---|
| `Reasoning code.ipynb` | Main implementation and experiments |
| `report.pdf` | Detailed assignment report |
| `results.json` | Recorded experimental evaluation results |
| `mnist_train_small.csv` | MNIST training data |
| `mnist_test.csv` | MNIST testing data |
| `california_housing_train.csv` | California Housing training data |
| `california_housing_test.csv` | California Housing testing data |

Limitations

- The parser primarily supports simple natural-language statements and rule structures.
- Complex nested quantifiers, disjunctions, and extensive world knowledge are outside the current parser's coverage.
- Closed-world reasoning is the default configuration.
- FOLIO and CounterBench evaluation results are not included in the recorded experimental results.

Conclusion

This project demonstrates the implementation and evaluation of a symbolic AI reasoning system using Forward Chaining and Backward Chaining.

The experimental results show that Backward Chaining achieved higher accuracy (99.77%), while Forward Chaining provided faster inference (0.577 ms per query).

The project highlights the importance of symbolic reasoning, logical inference, and knowledge representation in Artificial Intelligence.

---

**Submitted by:** Ankit Kumar  
**Roll Number:** M26CPS002

**Course:** Artificial Intelligence Assignment
