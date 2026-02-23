# 🌐 3D Visualization Hub

**Interactive 3D data visualizations powered by Google Cloud. Features Plotly, Matplotlib, and Streamlit for stunning multidimensional data exploration with phi-harmonic modal analysis and real-time cloud streaming.**

## Features

✨ **Interactive 3D Visualizations**
- Plotly-powered rotating, zoomable 3D scatter plots
- Surface meshes for mathematical and statistical data
- Real-time data streaming from Google Cloud sources
- Color-mapped multidimensional analysis

🎵 **Phi-Harmonic Analysis**
- Golden ratio-based frequency visualization
- Modal analysis for orchestration systems
- Recursive system topology mapping
- Constraint-based governance framework visualization

☁️ **Google Cloud Integration**
- Cloud Run serverless deployment
- BigQuery data source integration
- Cloud Datastore real-time metrics
- Cloud Build CI/CD pipeline ready

🚀 **Web Interface**
- Streamlit-based dashboard
- REST API endpoints
- WebSocket real-time connections
- Mobile-responsive design

## Quick Start

### Prerequisites

- Python 3.9+
- Google Cloud Account with active project
- Git

### Installation

```bash
git clone https://github.com/Flickerflash/3d-visualization-hub.git
cd 3d-visualization-hub
pip install -r requirements.txt
```

### Running Locally

```bash
streamlit run app.py
```

The app will open at `http://localhost:8501`

## Project Structure

```
3d-visualization-hub/
├── app.py                    # Streamlit main application
├── requirements.txt          # Python dependencies
├── Dockerfile                # Container configuration
├── cloud_run_deploy.sh      # Cloud Run deployment script
├── src/
│   ├── visualizations.py    # 3D visualization components
│   ├── data_handlers.py     # BigQuery & Cloud Datastore integrations
│   └── phi_harmonics.py     # Phi-harmonic analysis algorithms
└── README.md
```

## Deployment to Cloud Run

```bash
# Set your Google Cloud project
export PROJECT_ID="your-project-id"

# Build and push container
docker build -t gcr.io/$PROJECT_ID/3d-viz .
docker push gcr.io/$PROJECT_ID/3d-viz

# Deploy to Cloud Run
gcloud run deploy 3d-viz --image gcr.io/$PROJECT_ID/3d-viz \
  --platform managed \
  --region us-central1 \
  --allow-unauthenticated
```

## Visualization Examples

### 1. Phi-Harmonic Wave Surface

Visualize harmonic frequencies based on the golden ratio and modal analysis principles.

### 2. Modal Frequency Orchestration

Explore how different AI agents operate across modal frequency spaces in your orchestration system.

### 3. Recursive System Topology

Visualize constraint-based governance frameworks as 3D network diagrams.

## Architecture

**Frontend:** Streamlit + Plotly  
**Backend:** Python 3.9+  
**Cloud:** Google Cloud Run, BigQuery, Cloud Datastore  
**CI/CD:** Cloud Build  
**Version Control:** GitHub

## Configuration

Set environment variables for Google Cloud integration:

```bash
export GOOGLE_CLOUD_PROJECT="your-project-id"
export BIGQUERY_DATASET="visualization_data"
export DATASTORE_NAMESPACE="prod"
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

MIT License - see LICENSE file for details

## Roadmap

- [ ] VR/AR viewing capabilities
- [ ] Advanced frequency analysis filters
- [ ] Custom color scheme builder
- [ ] Real-time collaborative visualization
- [ ] Machine learning model integration
- [ ] Performance optimization for large datasets

## Support & Documentation

For detailed documentation, see the [Google Drive documentation](https://drive.google.com/drive/folders/YOUR_FOLDER_ID) or visit the [wiki](./wiki).

---

**Built with ❤️ for data visualization enthusiasts and AI systems architects**
