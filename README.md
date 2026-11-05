**Fine-Tuning LLM for Logical Reasoning**

## Project Overview

This project explores fine-tuning a Large Language Model to improve its ability to solve logical reasoning questions using the LogiQA dataset.

The project uses Meta-Llama-3.1-8B-Instruct with LoRA and 4-bit quantization.

## Technologies Used

- Python
- Google Colab
- PyTorch
- Hugging Face Transformers
- Hugging Face PEFT
- BitsAndBytes
- Scikit-learn
- Pandas
- Matplotlib

## Model Configuration

| Parameter | Configuration |
|---|---|
| Base Model | Meta-Llama-3.1-8B-Instruct |
| Fine-tuning | LoRA |
| Quantization | 4-bit NF4 |
| Dataset | LogiQA |
| Training Epochs | 1 |
| Training Steps | 922 |
| Training Loss | 1.9292 |
| Validation Loss | 1.6486 |

## Dataset

| Split | Examples |
|---|---:|
| Training | 7,376 |
| Validation | 651 |
| Testing | 651 |

## Evaluation Results

| Metric | Result |
|---|---:|
| Test Accuracy | 46.08% |
| Macro Precision | 0.46 |
| Macro Recall | 0.46 |
| Macro F1-score | 0.46 |

The evaluation was performed on 651 test examples.

## Repository Structure

- README.md
- LLM_Logical_Reasoning_Fine_Tuning.ipynb
- evaluation_results.csv
- final_evaluation_summary.csv
- project_final_results.csv
- functional_testing_results.csv

## Functional Testing

Three additional logical reasoning examples were tested:
- Human mortality
- Bird characteristics
- Rain and wet ground

All three produced the expected answers in the observed tests.

## Project Limitations

The reported accuracy represents the current evaluation run. Further experiments and comparisons are needed to establish improvements over the original base model.

## Academic Project

SRM Institute of Science and Technology

Department of Computational Intelligence

## License

Add an appropriate license before reuse or redistribution.
"""

readme_path = os.path.join(github_dir, "README.md")

with open(readme_path, "w", encoding="utf-8") as file:
    file.write(readme)

print("Professional README created successfully.")
print(readme_path)
