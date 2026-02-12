# 🦊 Heures Sup' Ultimate

Système complet de suivi des heures supplémentaires avec RPG, gamification et 600 scénarios juridiques.

---

## 📁 Structure du dépôt

```
heures-sup-ultimate/
│
├── index.html                   ← Page principale (copier-coller ici)
│
├── css/
│   └── style.css                ← Tous les styles
│
├── js/
│   ├── modes.js                 ← Sélecteur Démo / Production / Dev
│   ├── safety.js                ← Sécurités anti-bug
│   ├── config.js                ← Configuration + globalData
│   ├── storage.js               ← Sauvegarde localStorage
│   ├── assets-config.js         ← 🎨 Configuration des images
│   ├── data-bridge.js           ← Lecture seule Modules 1 & 2
│   ├── module-loader.js         ← Chargement modules
│   ├── scenarios-fox-data.js    ← 600 scénarios (données brutes)
│   ├── scenarios-fox.js         ← Moteur scénarios FOX
│   ├── rpg-system.js            ← 50 badges + 10 ligues + XP
│   ├── module1.js               ← Module 1 (annuel)
│   ├── module2.js               ← Module 2 (mensuel)
│   ├── module3.js               ← Module 3 RPG (badges + ligues)
│   └── main.js                  ← Point d'entrée principal
│
├── assets/                      ← 🎨 VOS IMAGES ICI
│   ├── badges/                  ← Images des 50 badges
│   ├── leagues/                 ← Images des 10 ligues
│   ├── characters/              ← Renard 4 saisons
│   └── backgrounds/             ← Décors 4 saisons
│
└── modules/
    ├── module1-annuel.html      ← Module 1 (fichier séparé)
    └── module2-mensuel.html     ← Module 2 (fichier séparé)
```

---

## 🎨 Ajouter vos images

### ⚠️ IMPORTANT : Si une image est absente → emoji automatique, pas de bug !

---

### 🦊 Renard saisonnier (4 fichiers)

Dossier : `assets/characters/`

| Fichier            | Saison          | Mois     |
|--------------------|-----------------|----------|
| `fox_spring.png`   | 🌸 Printemps    | Mars–Mai |
| `fox_summer.png`   | ☀️ Été          | Juin–Août|
| `fox_autumn.png`   | 🍂 Automne      | Sep–Nov  |
| `fox_winter.png`   | ❄️ Hiver        | Déc–Fév  |

**Taille recommandée** : 200×200 px (ou plus, PNG avec fond transparent)

---

### 🌿 Décors saisonniers (4 fichiers)

Dossier : `assets/backgrounds/`

| Fichier            | Saison       |
|--------------------|--------------|
| `bg_spring.jpg`    | 🌸 Printemps |
| `bg_summer.jpg`    | ☀️ Été       |
| `bg_autumn.jpg`    | 🍂 Automne   |
| `bg_winter.jpg`    | ❄️ Hiver     |

**Taille recommandée** : 1920×1080 px minimum (paysage)  
**Format** : JPG ou PNG  
Si absent → gradient CSS automatique

---

### ⚔️ Ligues (10 fichiers)

Dossier : `assets/leagues/`

| Fichier                  | Ligue        | XP requis  |
|--------------------------|--------------|------------|
| `league_bronze3.png`     | 🥉 Bronze III| 0          |
| `league_bronze2.png`     | 🥉 Bronze II | 500        |
| `league_bronze1.png`     | 🥉 Bronze I  | 1 000      |
| `league_silver3.png`     | 🥈 Silver III| 2 000      |
| `league_silver2.png`     | 🥈 Silver II | 3 500      |
| `league_silver1.png`     | 🥈 Silver I  | 5 500      |
| `league_gold3.png`       | 🥇 Gold III  | 8 000      |
| `league_gold2.png`       | 🥇 Gold II   | 12 000     |
| `league_gold1.png`       | 🥇 Gold I    | 18 000     |
| `league_legend.png`      | 👑 Legend    | 30 000     |

**Taille recommandée** : 128×128 px, PNG transparent

---

### 🏆 Badges (50 fichiers)

Dossier : `assets/badges/`

**Format du nom** : `badge_[ID].png`

#### Communs (20 badges)
| Fichier                            | Badge             |
|------------------------------------|-------------------|
| `badge_first_scenario.png`         | Premier Pas       |
| `badge_scenarios_10.png`           | Curieux           |
| `badge_scenarios_25.png`           | Étudiant          |
| `badge_scenarios_50.png`           | Appliqué          |
| `badge_scenarios_100.png`          | Assidu            |
| `badge_level_5.png`                | Niveau 5          |
| `badge_level_10.png`               | Niveau 10         |
| `badge_wisdom_100.png`             | Sage débutant     |
| `badge_standard_master.png`        | Classique         |
| `badge_intense_reader.png`         | Résistant         |
| `badge_night_worker.png`           | Noctambule        |
| `badge_weekend_warrior.png`        | Weekendeur        |
| `badge_wellbeing_fan.png`          | Zen               |
| `badge_module1_user.png`           | Annuel            |
| `badge_module2_user.png`           | Mensuel           |
| `badge_first_week.png`             | Première Semaine  |
| `badge_hours_100.png`              | Centenaire        |
| `badge_consistent.png`             | Régulier          |
| `badge_explorer.png`               | Explorateur       |
| `badge_quick_learner.png`          | Rapide            |

#### Rares (15 badges)
| Fichier                            | Badge             |
|------------------------------------|-------------------|
| `badge_scenarios_150.png`          | Studieux          |
| `badge_scenarios_200.png`          | Érudit            |
| `badge_level_15.png`               | Niveau 15         |
| `badge_level_20.png`               | Niveau 20         |
| `badge_wisdom_250.png`             | Sage averti       |
| `badge_wisdom_500.png`             | Grand Sage        |
| `badge_category_master.png`        | Polyvalent        |
| `badge_hours_500.png`              | Travailleur       |
| `badge_overtime_tracker.png`       | Vigilant          |
| `badge_night_expert.png`           | Expert Nuit       |
| `badge_prevention_master.png`      | Préventeur        |
| `badge_both_modules.png`           | Double Suivi      |
| `badge_perfect_week.png`           | Semaine Parfaite  |
| `badge_marathon.png`               | Marathon          |
| `badge_league_silver.png`          | Argent Atteint    |

#### Épiques (10 badges)
| Fichier                            | Badge             |
|------------------------------------|-------------------|
| `badge_scenarios_300.png`          | Expert            |
| `badge_scenarios_400.png`          | Maître            |
| `badge_level_30.png`               | Niveau 30         |
| `badge_level_40.png`               | Niveau 40         |
| `badge_wisdom_1000.png`            | Sage Suprême      |
| `badge_all_categories.png`         | Omniscient        |
| `badge_hours_1000.png`             | Millénaire        |
| `badge_legal_expert.png`           | Juriste du Travail|
| `badge_league_gold.png`            | Or Atteint        |
| `badge_wellbeing_champion.png`     | Champion Bien-être|

#### Légendaires (5 badges)
| Fichier                            | Badge             |
|------------------------------------|-------------------|
| `badge_scenarios_500.png`          | Légende           |
| `badge_completionist.png`          | Complétionniste   |
| `badge_level_50.png`               | Niveau Maximum    |
| `badge_wisdom_2000.png`            | Oracle            |
| `badge_league_legend.png`          | Légende Ultime    |

**Taille recommandée** : 128×128 px, PNG transparent

---

## 🚀 Utilisation

### Ouvrir localement
```
Ouvrir index.html dans votre navigateur
```

### Via GitHub Pages
```
Settings → Pages → Source: main branch
→ Accessible sur https://[vous].github.io/[repo]/
```

### Premier lancement
```
→ Choisir un mode (Démo, Production, Dev)
→ Le choix est mémorisé pour les prochaines fois
→ Bouton "Changer mode" dans le Dashboard
```

---

## 🎮 Modes

| Mode | Utilisation | Données |
|------|-------------|---------|
| 🎮 Démo | Découvrir | Pré-remplies (niveau 12) |
| 💼 Production | Utilisation réelle | Vos données |
| 🛠️ Dev | Développement | Panneau debug |

---

## 📖 Scénarios

600 scénarios juridiques couvrant :
- Semaines standard et intenses
- Travail de nuit et astreintes
- Weekends et jours fériés
- Limites légales et violations
- Bien-être et prévention burn-out
- Et ~15 autres catégories

---

## 🏆 Système RPG

- **50 badges** : Commun / Rare / Épique / Légendaire
- **10 ligues** : Bronze III → Legend
- **XP** : Gagné en lisant scénarios et débloquant badges
- **Sagesse** : Accumulée à chaque scénario lu
- **Level up** automatique

---

## 🛡️ Sécurités

- Erreurs interceptées (pas de crash)
- Validation des données au chargement
- Réparation automatique si données corrompues
- Fallback emoji si image absente
- `healthCheck()` disponible en console (mode Dev)

---

## 📦 Version

**v3.0.0-ULTIMATE-SECURE**  
Tous les fichiers sont indépendants — pas de dépendance externe, pas d'installation requise.
