# Assignment 1

Personal Git repository for **Assignment 1**: learning Bash, Python, and R workflows with conda, JupyterLab, and version control.

## Description

This project practices:

- Writing and running simple **Hello, World!** programs in Bash, Python, and R
- Creating and activating a conda environment
- Launching JupyterLab with language-specific kernels
- Organizing and pushing project files to GitHub

The repo has two complementary areas:

| Folder | Purpose |
|--------|---------|
| `manual/` | Original Hello, World! scripts and notebooks |
| `ai/` | AI-assisted workspace with the same exercises as scripts and Jupyter notebooks |

## Project structure

```
bash_env_assignment/
├── README.md
├── environment.yml      # Conda environment definition
├── requirements.txt     # Optional pip packages
├── setup_env.sh         # Environment setup (HPC / cluster)
├── manual/              # Manual Hello, World! exercises
│   ├── hello.sh
│   ├── hello.py
│   ├── hello.R
│   ├── hello_bash.ipynb
│   ├── hello_python.ipynb
│   └── hello_r.ipynb
└── ai/                  # AI-assisted workspace
    ├── hello.sh
    ├── hello.py
    ├── hello.R
    ├── hello_bash.ipynb
    ├── hello_python.ipynb
    └── hello_r.ipynb
```

## Requirements

- Miniconda or Anaconda
- Python 3.10
- JupyterLab and Python kernel (`jupyterlab`, `ipykernel`)
- R and R kernel (`r-base`, `r-irkernel`)
- Bash kernel (for `ai/hello_bash.ipynb` and `manual/hello_bash.ipynb`)

## Set up

1. Clone the repository:

```bash
git clone https://github.com/nguyen3693/bash_env_assignment.git
cd bash_env_assignment
```

2. Create the conda environment:

```bash
conda env create -f environment.yml
```

3. Activate the environment:

```bash
conda activate 7030_class_1
```

On the cluster, you can also run:

```bash
./setup_env.sh
```

## Usage

### Run scripts from `manual/`

```bash
cd manual
./hello.sh
./hello.py
./hello.R
```

### Run scripts from `ai/`

```bash
cd ai
./hello.sh
./hello.py
./hello.R
```

### Open notebooks in JupyterLab

From the repo root:

```bash
jupyter lab
```

Then open notebooks in either folder:

- `manual/hello_bash.ipynb`, `manual/hello_python.ipynb`, `manual/hello_r.ipynb`
- `ai/hello_bash.ipynb`, `ai/hello_python.ipynb`, `ai/hello_r.ipynb`

The `ai/` folder is an **AI-assisted workspace** for interactive, cell-by-cell exploration—the same Hello, World! examples, organized for notebook-based workflow with AI tooling support.

## Conclusion

Yippie! :^)
