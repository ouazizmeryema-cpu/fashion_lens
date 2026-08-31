# 👗 FashionLens

Assistant de style par IA  envoie une photo d'une pièce de ta garde-robe, reçois des suggestions de pièces complémentaires pour compléter ta tenue. Computer vision, transfer learning, API FastAPI + interface React.

> **Statut : 🚧 Démarrage**  Setup du projet en cours, modélisation à venir.

## 🎯 Objectif

Construire un assistant de style capable de recommander comment compléter une tenue à partir d'une simple photo :
- **Entrée** : une photo d'une pièce de vêtement (un pull, un pantalon...)
- **Traitement** : analyse visuelle de la pièce et comparaison avec une base de vraies tenues complètes
- **Sortie** : suggestions de pièces complémentaires (type de bas/haut, chaussures, style général) pour compléter le look

Architecture backend/frontend séparée :
- **Backend** : API d'analyse et de recommandation visuelle (Python, FastAPI, TensorFlow)
- **Frontend** : interface d'upload de photo et d'affichage des suggestions (React)

## 📊 Dataset

[Shop The Look Dataset](https://www.kaggle.com/datasets/pypiahmad/shop-the-look-dataset) — paires scène complète / produit issues de tenues réelles, permettant d'apprendre quelles pièces sont typiquement associées ensemble *(en cours de validation)*.

## ✅ Avancement

- [x] Setup projet (structure, venv, environnement)
- [x] Cadrage du concept (recommandation de style plutôt que simple classification)
- [ ] Sélection et validation du dataset
- [ ] Exploration des données (structure des paires scène/produit)
- [ ] Preprocessing des images (redimensionnement, normalisation, augmentation de données)
- [ ] Extraction de caractéristiques visuelles par transfer learning (ResNet / MobileNet)
- [ ] Moteur de similarité/recommandation entre pièces
- [ ] Évaluation qualitative des recommandations
- [ ] API de recommandation (FastAPI, upload d'image)
- [ ] Interface frontend (React)
- [ ] Dockerisation

## 🛠️ Stack technique

**Backend**
- Python, TensorFlow/Keras (transfer learning, extraction de caractéristiques visuelles)
- FastAPI + python-multipart (upload d'images)
- Pillow, NumPy (traitement d'image)
- Scikit-learn (similarité, métriques d'évaluation)

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
│   ├── features/          # extraction de caractéristiques visuelles
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

## Auteur 
Meryem  OUAZIZ Etudiante en Bachelor developpement IA EPSI 
