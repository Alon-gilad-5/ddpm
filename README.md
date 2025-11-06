# Homework 2: DDPM

In this section, we will implement DDPM (**Denoising Diffusion Probabilistic Models**) on a simple 1D Mixture of Gaussians Model.  Note that GPUs will not help in any part except the final section with the generation of images (everything else runs in less than a second), so it is recommended to run this part of the homework on a local CPU.

## Repository Contents

- `HW2_318280294.ipynb` — Jupyter notebook with code, analysis, and results.
- `images/` — exported figures from the notebook outputs.

## Setup & Environment

1. Install Python 3.10+ and pip.
2. Create and activate a virtual environment (optional but recommended):

   ```bash
   python -m venv .venv
   source .venv/bin/activate  # Windows: .venv\Scripts\activate
   ```

3. Install dependencies (if you have a `requirements.txt`, place it in the repo root):

   ```bash
   pip install -r requirements.txt
   ```

## How to Run

Open the notebook and run cells top-to-bottom:

```bash
jupyter lab  # or: jupyter notebook
```

## Notebook Outline

* Homework 2: DDPM
  - Section A
* Training
* Sampling
  - Section B
    - Network helpers
    - Position embeddings
    - ResNet block
    - Attention module
    - Group normalization
    - Conditional U-Net
  - Defining the forward diffusion process
    - Forward/ Diffusion process ###
  - Define a PyTorch Dataset + DataLoader
  - Sampling
  - Train the model
* Sampling (inference)
    - Sample at least 64 images for submission.
    - The zip file should follow the format "HW\{\#assignment\}\_\{id\}.\{extension\}" (according to the course syllabus).
    - Images within the zip should be .png or .jpg.

## Results (Figures)

![Figure from cell 1](images/figure_01.png)

![Figure from cell 4](images/figure_02.png)

![Figure from cell 10](images/figure_03.png)

![Figure from cell 10](images/figure_04.png)

![Figure from cell 14](images/figure_05.png)

![Figure from cell 14](images/figure_06.png)

![Figure from cell 16](images/figure_07.png)

![Figure from cell 16](images/figure_08.png)

![Figure from cell 27](images/figure_09.png)

![Figure from cell 27](images/figure_10.jpg)

![Figure from cell 30](images/figure_11.png)

![Figure from cell 30](images/figure_12.png)

![Figure from cell 39](images/figure_13.png)

## Reproducibility Notes

- Record your Python/package versions using `pip freeze > requirements.txt`.
- Set random seeds where applicable.
- Clearly document data sources and preprocessing steps.

## License

This repository is for academic coursework. If you plan to reuse or share parts of this work, ensure compliance with course policy.
