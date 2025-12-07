# Régression logistique (from scratch)

## Description

Ce projet a pour objectif d'implémenter la **régression logistique** depuis les formules mathématiques, sans utiliser de bibliothèques d'implémentation directe, puis de comparer les résultats avec une solution de référence (`scikit-learn`).

Les méthodes implémentées sont :

1. **Descente de gradient** : mise à jour des coefficients β via le gradient de la log-vraisemblance.
2. **Méthode de Newton / IRLS** : mise à jour des coefficients via la Hessienne de la log-vraisemblance.

Le projet permet de visualiser et comparer la convergence des différentes méthodes et la performance sur un dataset réel.

---

## Dataset utilisé

* **Pima Indians Diabetes Database**
* Source : [Kaggle](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)
* Contient des variables biologiques et le label `Outcome` indiquant la présence de diabète.

---

## Contenu du projet

* `Méthode_du_gradient.ipynb` : Notebook implémentant la régression logistique par descente de gradient.
* `Méthode_de_Newton.ipynb` : Notebook implémentant la régression logistique via méthode de Newton / IRLS.
* `requirements.txt` : Dépendances Python nécessaires (`numpy`, `pandas`, `matplotlib`, `scikit-learn`).

---

## Instructions d'utilisation

1. Créer un environnement virtuel Python (optionnel) :

```bash
python -m venv venv
source venv/bin/activate  # mac/linux
venv\Scripts\activate     # windows
```

2. Installer les dépendances :

```bash
pip install -r requirements.txt
```

3. Télécharger le dataset Pima Indians Diabetes et le placer dans le dossier du projet.

4. Lancer les notebooks :

```bash
jupyter notebook Méthode_du_gradient.ipynb
jupyter notebook Méthode_de_Newton.ipynb
```

---

## Résultats attendus

* Comparaison des coefficients β obtenus par les deux méthodes avec `scikit-learn`.
* Convergence rapide de la méthode de Newton (moins d’itérations que la descente de gradient).
* Visualisation des fonctions de perte et évolution des coefficients.

---

## Auteur

Bargouth Eya — Projet réalisé dans le cadre du cours d’optimisation / apprentissage statistique.
