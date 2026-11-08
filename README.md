<div align="center">

# 🧬 Hydroxyurea Synthesis Console

**Simulateur expert · Synthèse de l'hydroxyurée (CH₄N₂O₂) · API pharmacopée**

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/fr/docs/Web/HTML)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/fr/docs/Web/JavaScript)
[![License: MIT](https://img.shields.io/badge/License-MIT-1B7F4B?style=for-the-badge)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-1.0.0-0055A4?style=for-the-badge)](https://github.com/gunout/Hydroxyuree-Synthesis-Console/releases)

[![CH₄N₂O₂](https://img.shields.io/badge/CH₄N₂O₂-76.05_g/mol-6B4FBB?style=flat-square)](#)
[![Yield](https://img.shields.io/badge/Yield-88%25-1B7F4B?style=flat-square)](#)
[![Purity](https://img.shields.io/badge/Purity-99.5%25-1B7F4B?style=flat-square)](#)
[![pKa](https://img.shields.io/badge/pKa-10.5-B8860B?style=flat-square)](#)
[![GMP](https://img.shields.io/badge/GMP-Ready-6B4FBB?style=flat-square)](#)
[![USP](https://img.shields.io/badge/USP-42-0055A4?style=flat-square)](#)
[![Ph.Eur.](https://img.shields.io/badge/Ph.Eur.-9-0055A4?style=flat-square)](#)

</div>

---

## 🎯 Description

Simulateur mono-fichier HTML/CSS/JS dédié à la synthèse industrielle de l'**hydroxyurée** (principe actif **HYDROCURE®** / **Hydrea®**). Couvre l'intégralité du procédé : stœchiométrie, thermodynamique, cinétique, économie et contrôle qualité pharmacopée (USP 42 / Ph. Eur. 9).

> ⚡ **Ouvrez `index.html` → ça fonctionne.** 0 dépendance, 0 build, offline-first.

---

## ✨ Fonctionnalités

| Section | Description |
|---------|-------------|
| 📊 Vue d'ensemble | KPIs, bilan matière, PFD, applications |
| ⚛️ Constructeur | Réaction 1:1 interactive (NH₂OH·HCl + NaOCN) |
| 🔥 Réacteur | Cuve batch 200 L · T/pH/conversion animés |
| 🌡️ Thermodynamique | ΔG°(T), K_eq, spéciation pH (pKa 10,5) |
| ⏱️ Cinétique | Ordre 2, Arrhenius (Ea = 58 kJ/mol), t½ |
| 💰 Économie | OPEX, CAPEX, décomposition des coûts |
| ⚠️ Sécurité | HAZOP 6 nœuds + simulateur emballement |
| 📋 Pharmacopée | USP 42 / Ph. Eur. 9 + propriétés |
| 📚 Documentation | Formules, hypothèses, références |

**Extras** : export JSON (`Ctrl+E`), impression (`Ctrl+P`), palette tricolore, responsive, WCAG AA.

---

## 🔬 Données scientifiques

**Réaction** : `NH₂OH·HCl + NaOCN → CH₄N₂O₂ + NaCl` (ratio 1:1)

| Propriété | Valeur |
|-----------|--------|
| Formule brute | CH₄N₂O₂ |
| Masse molaire | 76,05 g/mol |
| Point de fusion | 145–147 °C (déc.) |
| Solubilité (eau 25 °C) | ~180 g/L |
| pKa | 10,5 |
| logP | −1,80 |
| Densité (20 °C) | 1,83 g/cm³ |
| Biodisponibilité orale | ~80 % |
| Demi-vie plasmatique | 3–4 h |

**Équations**

- Thermodynamique : `ΔG°(T) = ΔH° − T·ΔS°` avec `ΔH° = −248 kJ/mol` · `ΔS° = −92 J/mol·K`
- Constante d'équilibre : `K_eq = exp(−ΔG°/RT)`
- Loi de vitesse : `r = k(T)·[NH₂OH]·[OCN⁻]` (ordre 2 global)
- Arrhenius : `k(T) = A·exp(−Ea/RT)` avec `Ea = 58 kJ/mol` · `A = 2,1×10⁸`
- Demi-vie : `t½ = 1/(k·C₀)`
- Henderson-Hasselbalch : `pH = pKa + log([A⁻]/[HA])`

**Rendements** : massique 56,5 % · molaire ≤ 100 % · industriel 88 % · pureté 99,5 %

---

## 🩸 Applications thérapeutiques

| Indication | Mécanisme | Dose |
|------------|-----------|------|
| 🩸 Drépanocytose | Induction HbF | 15–35 mg/kg/j |
| 🎗️ Leucémie myéloïde | Inhibiteur RRM2 | 20–30 mg/kg/j |
| 🔬 Tumeurs solides | Radiosensibilisation | 1–2 g/m² |
| 🧬 VIH (investig.) | Potentialisation ddI | Essais |

**Pharmacophore** : `–NH-OH` · inhibition RRM2 → blocage synthèse ADN phase S.

---

## 🚀 Installation

```bash
git clone https://github.com/gunout/Hydroxyuree-Synthesis-Console.git
cd Hydroxyuree-Synthesis-Console

# Ouvrir
open index.html      # macOS
start index.html    # Windows
xdg-open index.html # Linux
```

Ou serveur local : `python -m http.server 8000` → http://localhost:8000

---

## 📋 Pharmacopée (USP 42 / Ph. Eur. 9)

| Paramètre | Cible |
|-----------|-------|
| Apparence | Poudre blanche |
| Identification | IR, HPLC |
| Pureté (HPLC-UV 214 nm) | 99,0–101,0 % |
| Impuretés totales | ≤ 1,0 % |
| Perte dessiccation (105 °C/4 h) | ≤ 1,0 % |
| Résidus ignition (600 °C) | ≤ 0,1 % |
| Métaux lourds (ICP-MS) | ≤ 20 ppm |
| Urée | ≤ 0,5 % |
| Solvants (ICH Q3C cl. 2) | GC-HS |
| Endotoxines (LAL) | ≤ 0,5 UI/mg |

---

## ⚠️ Sécurité HAZOP

| Substance | Danger | Niveau |
|-----------|--------|--------|
| NH₂OH·HCl | Explosif > 130 °C · CMR | 🔴 Critique |
| NaOCN | Toxique (libère HCN) | 🟠 Élevé |
| Hydroxyurée | Cytotoxique · tératogène | 🔴 Critique |
| Produit sec | Poussière explosive | 🟡 Modéré |

**6 nœuds HAZOP** : stockage NH₂OH · dosage NaOCN · pH bas (HCN) · agitation HS · filtration (poudre) · séchage (dégradation)

**Simulateur emballement** : 60 °C nominal → 80 °C alerte → 100 °C alarme → **> 130 °C explosion**

---

## 🛠️ Stack technique

- **HTML5** · **CSS3** (variables CSS) · **JavaScript** ES2020+ · **Canvas API**
- ✅ 0 npm · 0 build · 0 CDN · 0 framework · offline-first
- Palette tricolore `#0055A4` / `#FFFFFF` / `#EF4135` · Responsive · WCAG AA

---

## 📁 Structure

```
Hydroxyuree-Synthesis-Console/
├── index.html          # Application mono-fichier (~50 KB)
├── README.md           # Ce fichier
├── LICENSE             # MIT
└── docs/
    └── FORMULAS.md
```

---

## 🤝 Contribuer

```bash
git checkout -b feature/ma-fonctionnalite
git commit -m "feat: ajout fonctionnalité X"
git push origin feature/ma-fonctionnalite
```

Conventions : [Conventional Commits](https://www.conventionalcommits.org/) · 2 espaces · camelCase.

[![Open Issue](https://img.shields.io/badge/Open_Issue-EF4135?style=for-the-badge&logo=github&logoColor=white)](https://github.com/gunout/Hydroxyuree-Synthesis-Console/issues/new)

---

## ⚠️ Avertissement

> **Simulateur pédagogique.** Modèles cinétiques et thermodynamiques simplifiés.  
> Usage réglementaire : valider via **DSC**, **ARC**, **HPLC-UV**, **ICP-MS**, **LAL** et dossier **DMF** conforme **ICH Q7**.

---

## 📄 Licence MIT

Copyright (c) 2024 Hydroxyurea Synthesis Console

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.

---

<div align="center">

[![Star](https://img.shields.io/badge/⭐_Star_this_repo-yellow?style=for-the-badge&logo=github)](https://github.com/gunout/Hydroxyuree-Synthesis-Console)

[⬆ Retour en haut](#-hydroxyurea-synthesis-console)

</div>
