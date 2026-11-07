# Calculus II Interactive Jupyter Companion

Eight interactive lessons designed to accompany the **condensed, five-volume typeset Calculus II lecture notes** derived from the uploaded handwritten and typed MATH 2300 notes. This project is a teaching supplement, **not a line-by-line transcription** of the source scans. Where the original source had obscured passages, the notebooks do not claim to reconstruct them.

## Notebook index

| Notebook | Main topics | Companion volume |
|---|---|---|
| 01 | Integration techniques; integration by parts | 1 |
| 02 | Trigonometric substitution; partial fractions | 1 |
| 03 | Volumes and work | 2 |
| 04 | Parametric curves and polar coordinates | 3 |
| 05 | Sequences and infinite series | 4 |
| 06 | Convergence tests | 4 |
| 07 | Power series | 5 |
| 08 | Taylor and Maclaurin series | 5 |

## Run in GitHub Codespaces (beginner-friendly)

1. Create a new GitHub repository (for example `calc2-interactive-notebooks`).
2. Upload **the contents** of this folder, including the hidden `.devcontainer` folder. You can use GitHub's **Add file → Upload files** interface; hidden directories can be easier to preserve by uploading with Git locally.
3. Choose **Code → Codespaces → Create codespace on main**.
4. Wait for `postCreateCommand` to install Python dependencies.
5. Open `notebooks/01_integration_techniques.ipynb`, select the **Python (Calc II)** kernel, and run cells from top to bottom.
6. Use sliders/dropdowns in the **Interactive experiment** section. If controls do not render, ensure the notebook is trusted and the Jupyter extension is active.

## Run locally in VS Code

```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
python -m pip install -r requirements.txt
```

Open the project folder in VS Code; install the Python and Jupyter extensions, open a notebook, and choose the `.venv` Python kernel.

## Teaching design

Each notebook contains a conceptual introduction, mathematical formula, static plot, interactive experiment, student exercises, and instructor notes. `numpy`, `scipy`, `matplotlib`, `sympy`, and `ipywidgets` provide the calculations and controls. Numerical experiments supplement rather than replace proofs. **New numerical examples are labeled as teaching supplements**; the topics and progression follow the condensed lecture-note volumes.

## Known limitations

- Widget output requires a live Jupyter frontend; the controls are not rendered in GitHub's static notebook preview.
- The notebooks have been checked for notebook validity and Python syntax; live widget interaction should be checked in Codespaces.
- Several mathematical examples are intentionally simpler than the handwritten worked examples to make sliders useful.
- Graphs are generated at runtime; no external datasets, API keys, or network calls are required after installation.

## Suggested workflow

Begin with 01 and 02 alongside Volume 1; complete exercises before proceeding. Encourage students to explain observed behavior and then justify it mathematically.
