# Quiz Prévention Bruit · Cartonnerie LACAUX Frères

Quiz interactif de prévention du risque bruit en milieu industriel, conçu pour la formation et la sensibilisation des opérateurs de la **Cartonnerie LACAUX Frères**.

Outil pédagogique **PréventIA-LaB** — Laure Bonnefond, IPRP/IST.

🌐 **URL de déploiement** : `https://laurebonnefond.github.io/quiz-bruit-cartonnerie-lacaux/`

---

## 🎯 Objectifs pédagogiques

- Comprendre les paramètres physiques du son (fréquence, intensité)
- Maîtriser les seuils réglementaires (80, 85, 87 dB(A))
- Connaître l'anatomie de l'oreille et le mécanisme de l'audition
- Saisir l'échelle logarithmique des décibels et l'équivalence d'énergie
- Appliquer la règle de port en continu des PICB
- Connaître les niveaux sonores spécifiques aux postes de l'entreprise (atelier palettes, onduleuse, MAP)

---

## 📋 Structure du quiz (12 questions)

| # | Type | Sujet |
|---|------|-------|
| 1 | QCM | Paramètres physiques du son |
| 2 | QCM | Seuil de danger auditif (80 dB(A)) |
| 3 | QCM | Doublement intensité = +3 dB |
| 4 | QCM | Équivalence énergie : 1h@89 dB = 8h@80 dB |
| 5 | Curseur | Niveau sonore en cartonnerie |
| 6 | Glisser-déposer | Anatomie de l'oreille (8 structures) |
| 7 | Glisser-déposer | Échelle des décibels (6 sources) |
| 8 | QCM · LACAUX | Atelier palettes : 89 dB(A) |
| 9 | QCM · LACAUX | Onduleuse, décortiqueur SF1 : 84 dB(A) |
| 10 | QCM · LACAUX | MAP, bobineuse : 89 dB(A) |
| 11 | QCM | Bouchon non porté 10 min = 50 % de protection perdue |
| 12 | Vrai/Faux | Surdité due au bruit professionnel : irréversible |
| 13 | Curseur | Niveau fréquence son  |
---

## 🚀 Déploiement sur GitHub Pages

### 1. Créer le repository

Sur GitHub, créer un nouveau repository **public** nommé :
```
quiz-bruit-cartonnerie-lacaux
```

Description suggérée :
> Quiz interactif de prévention du risque bruit pour la cartonnerie LACAUX Frères. 12 questions (QCM, curseur, glisser-déposer anatomie de l'oreille, échelle des décibels) avec feedback pédagogique INRS et Code du travail. Outil PréventIA-LaB.

### 2. Pousser les fichiers

```bash
git init
git add .
git commit -m "Initial commit - Quiz prévention bruit LACAUX"
git branch -M main
git remote add origin https://github.com/laurebonnefond/quiz-bruit-cartonnerie-lacaux.git
git push -u origin main
```

### 3. Activer GitHub Pages

1. Aller dans **Settings** du repository
2. Section **Pages** (menu de gauche)
3. **Source** : sélectionner `Deploy from a branch`
4. **Branch** : sélectionner `main` et dossier `/ (root)`
5. Cliquer **Save**

Après 1 à 2 minutes, le quiz est accessible à :
```
https://laurebonnefond.github.io/quiz-bruit-cartonnerie-lacaux/
```

---

## 🧪 Test local (avant déploiement)

```bash
cd quiz-bruit-cartonnerie-lacaux
python3 -m http.server 8000
```

Puis ouvrir `http://localhost:8000` dans le navigateur.

---

## 📁 Structure du projet

```
quiz-bruit-cartonnerie-lacaux/
├── index.html              # Quiz complet (HTML + CSS + JS inline)
├── README.md               # Ce fichier
└── assets/
    ├── logo.png            # Logo PréventIA-LaB
    └── ear-anatomy.jpg     # Schéma anatomique de l'oreille
```

---

## 🎨 Personnalisation

Les couleurs de la charte PréventIA-LaB sont définies en variables CSS au début du fichier `index.html`, section `:root` :

```css
--teal: #2A8C8C;       /* couleur principale */
--teal-dark: #1F5F66;  /* version foncée */
--green: #1D9E75;      /* feedback positif */
--red: #E24B4A;        /* feedback négatif */
--orange: #EF9F27;     /* badges LACAUX, étoiles résultat */
--navy: #0E2A38;       /* texte principal */
```

Pour adapter le quiz à une autre entreprise :
1. Remplacer le contenu des questions 8, 9 et 10 (badge "données LACAUX")
2. Adapter la question 5 (curseur) avec le nom de l'entreprise
3. Mettre à jour le titre et footer

---

## 📚 Sources et références

- **INRS ED 6035** · Évaluation et prévention des risques liés au bruit
- **INRS ED 868** · Les protecteurs individuels contre le bruit
- **Code du travail** : articles R.4431-1 à R.4437-4
- **Données entreprise** : mesurages sonométriques LACAUX Frères

---

## 👤 Crédits

**Laure Bonnefond** — Infirmière en santé au travail · IPRP/IST
SPSTI 23/87 — Limoges

Projet développé dans le cadre de **PréventIA-LaB** : plateforme d'outils IA pour la prévention en santé au travail.
🔗 [github.com/laurebonnefond/PreventIA-LaB](https://github.com/laurebonnefond/PreventIA-LaB)

---

## 📄 Licence

Outil pédagogique à usage professionnel. Mention de la source (Laure Bonnefond / PréventIA-LaB) appréciée en cas de réutilisation.
