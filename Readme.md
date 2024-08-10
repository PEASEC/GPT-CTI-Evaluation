# Dissertation Script: Testing GPT-3.5 and GPT-4 on Few-Shot CTI Dataset

This repository contains the script used in my dissertation to evaluate the performance of GPT-3.5 and GPT-4 models on the few-shot CTI dataset from the [MSExchange Server CTI Dataset](https://github.com/PEASEC/msexchange-server-cti-dataset). The script is designed to test various configurations and includes parameters for guidelines, few-shot settings, and chain-of-thought (CoT) processing.

## Parameters

The script includes several parameters to customize the testing setup:

- `is_guideline`: Include guidelines in the testing.
  - Default: `True`
- `is_few_shot`: Use the few-shot CTI dataset or the normal CTI dataset.
  - Default: `True`
- `is_chain_of_thought`: Enable zero-shot Chain-of-Thought (CoT) processing.
  - Default: `True`
- `chain_of_thought_v2`: Enable non-zero-shot CoT processing with explanations from `cot_explanations.txt`.
  - Default: `True`

## GPT Models

The script allows changing the GPT model in the request to the OpenAI API. You can test different versions, such as GPT-3.5 and GPT-4, by adjusting the API request configuration.

## Results

The results of the tests are saved in the `Results/` directory. This includes performance metrics and other relevant data generated during the testing process.

## Repository Structure

```
├── cot_explanations.txt     # Explanations for non-zero-shot CoT processing
├── Results/                 # Directory containing the test results
│   ├── result_file1.txt     # Example result file
│   └── ...
├── gpt.py                # Main script for testing GPT models on CTI dataset
└── README.md                # This README file
```

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/PEASEC/GPT-CTI-Evaluation.git
   cd GPT-CTI-Evaluation
   ```

2. Install the required dependencies of the gpt.py file.

3. Get the [MSExchange Server CTI Dataset](https://github.com/PEASEC/msexchange-server-cti-dataset) and store it in data/

4. Configure the parameters in the `gpt.py` file as needed.

5. Run the script:
   ```
   python gpt.py
   ```


## Contributing

If you wish to contribute to this project, please fork the repository and submit a pull request. For any issues or questions, please open an issue on GitHub.

## Author

**Markus Bayer**

For any further information or questions, please contact Markus Bayer.
