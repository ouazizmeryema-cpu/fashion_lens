# 👗 FashionLens

Reconnaissance automatique de vêtements par IA — computer vision, transfer learning, API FastAPI + interface React.

> **Statut : 🚧 Démarrage** — Setup du projet en cours, modélisation à venir.

## 🎯 Objectif

Construire un système capable d'identifier automatiquement la catégorie d'un vêtement (t-shirt, robe, pantalon, chaussures...) à partir d'une simple photo, avec une architecture backend/frontend séparée :
- **Backend** : API de classification d'image (Python, FastAPI, TensorFlow)
- **Frontend** : interface d'upload et d'affichage des résultats (React)

## 📊 Dataset

Dataset de vêtements avec catégories labellisées *(à confirmer — dataset Kaggle en cours de sélection)*.

## ✅ Avancement

- [x] Setup projet (structure, venv, environnement)
- [ ] Sélection et exploration du dataset
- [ ] Preprocessing des images (redimensionnement, normalisation, augmentation de données)
- [ ] Modélisation par transfer learning (ResNet / MobileNet)
- [ ] Évaluation du modèle (accuracy, matrice de confusion)
- [ ] API de classification (FastAPI, upload d'image)
- [ ] Interface frontend (React)
- [ ] Dockerisation

## 🛠️ Stack technique

**Backend**
- Python, TensorFlow/Keras (transfer learning)
- FastAPI + python-multipart (upload d'images)
- Pillow, NumPy (traitement d'image)
- Scikit-learn (métriques d'évaluation)

**Frontend**
- React (Vite)
- Tailwind CSS

**Infra**
- Docker *(à venir)*

## 📁 Structure du projet

\`\`\`
fashionLens/
├── data/                  # raw/processed (non versionné)
├── notebooks/             # exploration et prototypage
├── models/                # modèles entraînés (non versionné)
├── src/
│   ├── features/          # preprocessing des images
│   ├── models/             # entraînement, transfer learning
│   └── api/                # API FastAPI
├── tests/
└── requirements.txt
\`\`\`

## 🚀 Installation

\`\`\`bash
git clone https://github.com/ouazizmeryema-cpu/fashionLens.git
cd fashionLens
python -m venv venv
source venv/Scripts/activate  # Windows (Git Bash)
pip install -r requirements.txt
\`\`\`

## 📝 Licence

MIT
