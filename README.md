# 3D Visualization Hub
![Status](https://img.shields.io/badge/Status-Active-brightgreen)
![Language](https://img.shields.io/badge/Language-Python-blue)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

> **Governance:** DGAF / Agent Amethyst — Yes. This visualization hub is part of the ndrorchestration DGAF ecosystem. See [DGAF-Framework](https://github.com/ndrorchestration/DGAF-Framework) for spine documentation.

Interactive 3D data visualization platform powered by Google Cloud. Features Plotly, Matplotlib, and Streamlit for multidimensional data exploration — with **phi-harmonic modal analysis**, governance score plotting, drift trajectory visualization, and real-time agent chain rendering.

Part of the [Phi-Harmonic Pentagon ecosystem](https://github.com/ndrorchestration/DGAF-Framework).

## What This Visualizes

- **Governance scores** — audit trail plots from `junior-apogee-app` and DGAF eval runs
- **Drift trajectories** — harmonic state monitoring surfaces from `Driftwatch`
- **Agent chain viz** — multi-agent synthesis flow graphs
- **Phi-harmonic modal analysis** — frequency decomposition in 3D manifold space
- **General multidimensional data** — rotating, zooming, filtering on any dataset

## Quick Start (Local)

```bash
git clone https://github.com/ndrorchestration/3d-visualization-hub.git
cd 3d-visualization-hub

python -m venv .venv
# PowerShell:
Set-ExecutionPolicy Bypass -Scope Process -Force
.\.venv\Scripts\Activate.ps1
# macOS/Linux:
# source .venv/bin/activate

pip install --upgrade pip
pip install -r requirements.txt

streamlit run app.py
```

## Example Dataset & Usage

A minimal example dataset and visualization script are included.

```bash
python -m examples.simple_3d_scatter
```

This generates a sample dataset and opens an interactive 3D scatter plot in your browser. The example demonstrates:
- Data loading and transformation
- Real-time filtering with sliders
- 3D rotation, zoom, and pan controls
- Export to static images

See `examples/` for more sample datasets and visualization templates.

## Development & CI

This project uses GitHub Actions for continuous integration:
- **Linting**: `pylint` and `black` on Python code
- **Testing**: Unit tests run automatically on every push
- **Docker**: Pre-built Docker image available for cloud deployment

```bash
# Run tests
pytest tests/ -v

# Code style
black .
pylint **/*.py
```

All PRs must pass CI checks before merging.

## Related Ecosystem

- [Driftwatch](https://github.com/ndrorchestration/Driftwatch) — phi-driven drift detection and harmonic state monitoring
- [junior-apogee-app](https://github.com/ndrorchestration/junior-apogee-app) — AI evaluation platform (source of governance score data)
- [DGAF-Framework](https://github.com/ndrorchestration/DGAF-Framework) — governance spine for the full ecosystem
- [Acoustic-mesh](https://github.com/ndrorchestration/Acoustic-mesh) — WebRTC acoustic mesh with phi-harmonic sensor analysis

## Provenance

Developed by [Ndr "Ender" Hensel](https://github.com/ndrorchestration) — AI Orchestration Engineer & Systems Architect, Columbus OH.  
[LinkedIn](https://www.linkedin.com/in/andrewhensel) · [GitHub](https://github.com/ndrorchestration)
