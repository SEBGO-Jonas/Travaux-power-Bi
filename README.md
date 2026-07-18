# 📊 Dashboard Power BI — Suivi des commandes clients/produits

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi&logoColor=black)
![Status](https://img.shields.io/badge/Statut-Terminé-brightgreen)

Tableau de bord **Power BI** interactif permettant de suivre l'activité commerciale à partir des commandes clients : chiffres clés, répartition géographique, ventes par catégorie et évolution mensuelle.

## 📁 Contenu du dépôt

| Fichier | Description |
|---|---|
| [`DASHBORD SJP.pbix`](./DASHBORD%20SJP.pbix) | Fichier Power BI Desktop contenant le modèle de données, les mesures et les 4 pages du rapport. |
| `README.md` | Ce fichier. |

> 💡 GitHub ne propose pas d'aperçu visuel des fichiers `.pbix` (fichier binaire) : seul un lien de téléchargement s'affichera. Pensez à ajouter une **capture d'écran** du dashboard dans le README (ex : `docs/apercu.png`) pour illustrer le rendu directement sur la page du dépôt.

## 🗂️ Modèle de données

Le rapport s'appuie sur une table unique : **`commande client produit`**, contenant :

| Colonne | Description |
|---|---|
| `IDcommande` | Identifiant de la commande |
| `IDClient` | Identifiant du client |
| `IDProduit` | Identifiant du produit |
| `Nom catégorie` | Catégorie du produit |
| `Pays` | Pays du client |
| `Quantité` | Quantité commandée |
| `Prix unitaire` | Prix unitaire du produit |
| `Montant` | Montant total de la commande |
| `Date livraison` | Date de livraison |
| `Année Mois` | Période (agrégation mensuelle) |

## 🖥️ Pages du rapport

Le dashboard est structuré en **4 pages** avec un menu de navigation personnalisé (boutons *Accueil*, *Tableau*, *Détails*) :

1. **Accueil** — vue d'ensemble avec cartes KPI (indicateurs clés) et texte de synthèse « Notre activité d'un coup d'œil ».
2. **Carte & répartition** — carte géographique (`map`) des ventes par pays, diagramme circulaire (`pieChart`) par catégorie de produit et graphique combiné courbe/colonnes empilées (`lineStackedColumnComboChart`) pour la tendance mensuelle.
3. **Tableau** — table détaillée (`tableEx`) des commandes avec graphiques en colonnes groupées et en courbe.
4. **Détails** — vue détaillée complémentaire des données.

## 📈 Visuels utilisés

- Cartes KPI (`card`)
- Carte géographique (`map`)
- Diagramme circulaire (`pieChart`)
- Graphique combiné courbe/colonnes (`lineStackedColumnComboChart`)
- Graphique en colonnes groupées (`clusteredColumnChart`) et en courbe (`lineChart`)
- Table détaillée (`tableEx`)
- Navigation personnalisée par boutons/icônes (formes et images)

## 🛠️ Utilisation

1. Installer [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (gratuit, Windows).
2. Ouvrir le fichier [`DASHBORD SJP.pbix`](./DASHBORD%20SJP.pbix).
3. Naviguer entre les pages via le menu personnalisé (Accueil / Tableau / Détails) ou les onglets de pages.
4. Actualiser les données via **Accueil > Actualiser** si une nouvelle source est connectée.

## 🧰 Technologies

- **Power BI Desktop**
- Modélisation de données (table unique orientée commandes)
- DAX (mesures et agrégations)
- Visuels natifs Power BI (carte, KPI, courbes, colonnes, secteurs, table)

## 📄 Licence

Projet personnel réalisé à des fins d'apprentissage (Data Analyst).
