## Quick Overview (In Plain Language)

This project is my **3D data visualization sandbox**.

In simple terms:
- It lets you explore complex data in interactive 3D (rotating, zooming, filtering).
- It uses tools like Plotly, Matplotlib, and Streamlit to turn numbers into visuals.
- It’s designed to eventually show things like AI model behavior and stability over time, not just static charts.

Right now this is an early **prototype**:
- Some examples are simple demos and experiments.
- The goal is to show how I think about visualizing multi-dimensional data (and later, phi-harmonic stability) in a way humans can actually use.
- It pairs with my other repos: evaluation in `junior-apogee-app`, prompts in `ai-prompt-systems-portfolio`, visuals here.


## Quick Start (Local)

```bash
git clone https://github.com/Flickerflash/3d-visualization-hub.git
cd 3d-visualization-hub

python -m venv .venv
# PowerShell:
Set-ExecutionPolicy Bypass -Scope Process -Force
.\.venv\Scripts\Activate.ps1
# or on macOS/Linux:
# source .venv/bin/activate

pip install --upgrade pip
pip install -r requirements.txt

streamlit run app.py


## Example Dataset & Usage

A minimal example dataset and visualization script are included to get you started quickly.

**To run the example:**

```bash
python -m examples.simple_3d_scatter
```

This generates a sample dataset and opens an interactive 3D scatter plot in your browser (via Streamlit). The example demonstrates:
- Data loading and transformation
- Real-time filtering with sliders
- 3D rotation, zoom, and pan controls
- Export to static images

See `examples/` folder for more sample datasets and visualization templates.

---

## Development & CI

This project uses GitHub Actions for continuous integration:
- **Linting**: `pylint` and `black` on Python code
- **Testing**: Unit tests run automatically on every push
- **Docker**: Pre-built Docker image available for cloud deployment

**Running tests locally:**

```bash
pytest tests/ -v
```

**Code style & linting:**

```bash
black .
pylint **/*.py
```

All PRs must pass CI checks before merging.
