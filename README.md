# A Large-Scale Investigation of Toxicity on GitHub Using Human-in-the-Loop Data Collection

## Overview
This repository contains code, prompts, and output data for the research paper **"A Large-Scale Investigation of Toxicity on GitHub Using Human-in-the-Loop Data Collection."** The study involves toxicity analysis on github issue and pull request discussions.

## Repository Structure
```
- dataset/                # This folder should contain the dataset files 
- output/                 # This folder should contain the generated output files 
- prompts/                # Contains prompts used to generate toxicity scores and explanations
- scripts/                # Contains Jupyter notebooks for model training and hypothesis testing
```

## Dataset and Output
The dataset and output files can be downloaded from the following Google Drive link:

[Download Dataset and Output](https://drive.google.com/file/d/1OS3EzKQfwpWUNK8W18k5ZzMD6AGBnMvT/view?usp=sharing)

After downloading, place the `dataset` and `output` folders in the root directory of this repository.

## Scripts
The `scripts/` directory contains the following Jupyter notebooks:

1. **verifier_model.ipynb** - Used to train the verifier model.
2. **select_incorrect_data.ipynb** - Uses the trained model to verify the large GitHub dataset.
3. **hypothesisTesting.ipynb** - Conducts hypothesis testing based on the verification results.
4. **hypothesisTesting-part2.ipynb** - Continuation of hypothesis testing.

### Adjusting File Paths
In the Jupyter notebooks, users must adjust the input file paths according to the files in the `dataset/` and `output/` folders before running the scripts.

## Usage
1. Download the dataset and output files from the provided link.
2. Place them inside the `dataset/` and `output/` folders.
3. Open the Jupyter notebooks inside the `scripts/` folder and modify the file paths accordingly.
4. Run the notebooks sequentially to train the model, verify data, and test hypotheses.


## License
This project is licensed under MIT license.

