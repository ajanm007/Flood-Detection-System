 Flood Detection System 

This project uses SAR, RGB, and Multi-Spectral satellite data to detect urban flooding in real-time.  
Built with deep learning models, trained and validated with high recall to prioritize sensitivity in flood-prone zones.

Model Performance Summary

| Model         | Accuracy | F1 Score | Recall | Precision |
|---------------|----------|----------|--------|-----------|
| SAR           | 82.31%   | 0.4850   | 1.0000 | 0.3261    |
| RGB           | 72.77%   | 0.4272   | 1.0000 | 0.2765    |
| Multi-Spectral| 66.67%   | 0.4285   | 1.0000 | 0.2818    |

Features

- Real-time flood detection using satellite imagery.
- High recall deep learning models.
- Modular design for model comparison.
- Ready for Docker deployment.

Folder Structure
├── assets/ # Visuals and reference images
├── models/ # Trained model weights (if not too big)
├── notebooks/ # Jupyter notebooks for training and evaluation
├── src/ # Python scripts for preprocessing and inference
├── app/ # Flask or FastAPI app (for deployment)
├── Dockerfile # For containerized deployment
├── requirements.txt # Dependencies
└── README.md # You're looking at it


---

Features

- Real-time flood detection using satellite data  
- Modular design: compare SAR vs RGB vs Multi-spectral  
- Easy to plug-in your own models  
- Built for deployment — Flask + Docker ready

---

Docker Deployment (Coming Soon)

```bash
docker build -t flood-detector .
docker run -p 5000:5000 flood-detector

