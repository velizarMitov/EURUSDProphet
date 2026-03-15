# EURUSDProphet

A Jupyter-based mathematics project for solving and explaining mathematical problems related to EUR/USD forecasting.

## Project Structure

```
JupyterProject1/
├── config/ 
│── config.py             # Configuration file with prompts as Python constants
├── data/                     # Data files and datasets
├── models/                   # Trained models or model definitions
├── notebooks/                # Jupyter notebooks
│   └── main.ipynb           # Main notebook
├── README.md
├── requirements.txt
└── sample.ipynb
```

## Setup

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Open Jupyter notebook:
   ```bash
   jupyter notebook
   ```

## Using the System Prompt

### Option 1: In Python Code
```python
from config.config import MATH_SYSTEM_PROMPT

# Use in your LLM/AI calls
```

### Option 2: In Markdown Cell
Read from `config/system_prompt.md` and include in your prompt context.

