# The flatness problem and inflation

This directory contains a Jupyter notebook that demonstrating how the observed flatness of the universe causes a problem for cosmology, and how inflation solves this problem.

The notebook shows:

- The Hubble diagram of Type Ia SNe, and how this implies a nearly flat universe
- 
---

## Contents

- `inflation.ipynb` – main notebook with theory, widgets, and questions.
- `Type-Ia-Supernova-Data.csv` - Type Ia supernova data
- `README.md` – this file.

---

## Google Colab

You can open this notebook in Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](
https://colab.research.google.com/github/ajw278/flatness_inflation_nb/blob/main/inflation.ipynb
)

This is the easiest if you're not familiar with notebooks. Otherwise the following requirements are needed.

## Requirements

You need:

- Python **3.9+** (3.10–3.12 recommended)
- **JupyterLab** or classic Jupyter Notebook
- The following Python packages:
  - `numpy`
  - `matplotlib`
  - `ipywidgets`

You do **not** need `%matplotlib widget` for this notebook – it uses standard
inline plots with `ipywidgets` sliders.

---

## Option A: Setup using conda (recommended)

```bash
conda create -n inflation_widget_env python=3.11 -c conda-forge \
    jupyterlab ipywidgets matplotlib numpy
conda activate inflation_widget_env
```

## Option B: Setup using pip + venv

```bash 
python -m venv inflation_widget_env
# On macOS / Linux:
source dm_widget_env/bin/activate
# On Windows:
inflation_widget_env\Scripts\activate

pip install jupyterlab ipywidgets matplotlib numpy
```

## Launch the notebook

From the directory containing the notebook:

```bash
# Activate the environment first
conda activate inflation_widget_env        # or: source dm_widget_env/bin/activate

# Then start Jupyter
jupyter lab                         # or: jupyter notebook
```

Then in your browser:
1. Open `inflation.ipynb`.
2. Run the cells from top to bottom (e.g. Kernel -> Restart & Run All).
3. Use the sliders at the bottom to explore how the halo and disc affect the
rotation curve and answer the questions in the notebook.

If widgets do not appear (no sliders), check that:
`ipywidgets` is installed in the same environment as the notebook kernel, and
you restarted Jupyter after installing new packages.

