# VillageManager

**Application de gestion pour les comités de village et les associations locales**

VillageManager est une application de bureau conçue pour faciliter la gestion quotidienne d’un village ou d’une association : adhérents, cotisations, dons, amendes, activités, dépenses, statistiques et sauvegardes. L’application fonctionne localement avec une base de données SQLite, pour une utilisation sans connexion Internet après installation et configuration.

> **Distribution commerciale — Windows 10/11**
>
> VillageManager est un logiciel propriétaire. Ce dépôt public présente le produit et ses fonctionnalités ; il n’autorise pas la copie, la modification, la redistribution ou la commercialisation du logiciel.

## Sommaire

- [Fonctionnalités](#fonctionnalités)
- [Technologies](#technologies)
- [Compatibilité et fonctionnement](#compatibilité-et-fonctionnement)
- [Installation](#installation)
- [Données et confidentialité](#données-et-confidentialité)
- [Sécurité et sauvegardes](#sécurité-et-sauvegardes)
- [Captures d’écran](#captures-décran)
- [Licence et distribution](#licence-et-distribution)
- [Assistance](#assistance)

## Fonctionnalités

### Tableau de bord
- Vue d’ensemble de la situation financière.
- Indicateurs des cotisations, dons, amendes et activités.
- Suivi des recettes, dépenses et du solde.
- Liste des cotisations impayées, avec recherche et export PDF.
- Notifications utiles à la gestion courante.

### Gestion des citoyens et adhérents
- Gestion d’un grand nombre de fiches, avec prise en charge de plus de 10 000 adhérents selon les performances du poste.
- Recherche rapide par nom, prénom ou famille.
- Détection des doublons et mise en forme automatique des noms.
- Suivi du statut : actif, décédé ou parti.
- Gestion des exonérations de cotisation.

### Cotisations annuelles
- Définition du montant par année.
- Suivi des paiements pour chaque adhérent.
- Recherche interactive d’un adhérent.
- Gestion des paiements excédentaires, pouvant être comptabilisés comme dons selon les règles de l’application.
- Historique par année.

### Dons
- Enregistrement des dons en argent ou en nature.
- Valeur estimée pour les dons matériels.
- Suivi par année et attribution aux familles concernées.

### Amendes
- Enregistrement des amendes et des paiements.
- Suivi des amendes payées et impayées.
- Recherche par nom et enregistrement de la date de paiement.

### Activités et cotisations exceptionnelles
- Création d’activités ou d’appels à contribution avec nom, montant et description.
- Affectation à tous les adhérents ou à une sélection manuelle.
- Suivi des participants et des paiements.
- Consultation des détails, listes et statistiques.
- Modification des activités et export PDF détaillé.

### Dépenses
- Enregistrement et suivi des dépenses par année.
- Consultation de l’historique et export PDF.

### Statistiques et rapports financiers
- Génération d’un rapport financier PDF détaillé de plusieurs pages.
- Graphiques de répartition des recettes.
- Classement des dix familles les plus contributrices.
- Statistiques sur les amendes et les activités.
- Comparaison entre les montants attendus et collectés.
- Évolution mensuelle des recettes.
- Analyse par nom de famille et synthèse financière.

### Gestion sur plusieurs années
- Consultation des données par année.
- Historique pluriannuel selon les années présentes dans la base de données.
- Navigation entre les années disponibles.

### Interface utilisateur
- Thème clair et thème sombre.
- Mode plein écran pour les présentations.
- Raccourcis clavier pour accéder rapidement aux principales pages et actions.
- Interface de bureau moderne avec animations.

### Sauvegardes et restauration
- Sauvegardes automatiques avec conservation d’un nombre limité de copies.
- Vérification de l’intégrité de la base de données.
- Restauration à partir d’une sauvegarde.

## Technologies

Les technologies utilisées comprennent notamment :

- **Python** — langage principal.
- **PySide6 / Qt** — interface graphique.
- **SQLite** — base de données locale.
- **ReportLab** — génération de rapports PDF.
- **Matplotlib** — graphiques et visualisations statistiques.
- **NumPy** — calculs et traitement de données.
- **Pillow** — traitement d’images.
- **cryptography** — fonctions cryptographiques.
- **argon2-cffi** — hachage des mots de passe.
- **PyInstaller** — génération de l’application exécutable.
- **GitHub Actions** — automatisation de la compilation Windows.

Les versions exactes des dépendances sont définies par les fichiers de configuration du projet et peuvent évoluer.

## Compatibilité et fonctionnement

- **Système cible :** Windows 10 et Windows 11.
- **Type :** application de bureau.
- **Stockage :** base de données SQLite locale.
- **Connexion Internet :** non nécessaire pour l’utilisation courante après installation et configuration.
- **Utilisation :** conçue pour un comité de village ou une association locale.

Les performances dépendent notamment de l’ordinateur, de la taille de la base de données et de son état.

## Installation

VillageManager est distribué sous forme d’application compilée aux utilisateurs autorisés.

1. Obtenez le paquet auprès du distributeur autorisé.
2. Extrayez les fichiers dans un dossier local si la distribution est fournie sous forme d’archive.
3. Suivez les instructions de configuration remises avec votre version.
4. Conservez les fichiers de licence et les informations de compte dans un emplacement sûr.
5. Effectuez régulièrement une sauvegarde de la base de données.

**Remarque :** ce dépôt de présentation ne fournit pas nécessairement le programme exécutable ni les fichiers requis pour l’activation. Ne téléchargez pas de fichiers de licence depuis une source non fiable.

## Données et confidentialité

VillageManager utilise une base de données locale pour les données de gestion. Comme l’application peut contenir des informations personnelles et financières sur les adhérents, l’organisme utilisateur doit :

- limiter l’accès à l’ordinateur et au compte utilisateur ;
- utiliser des mots de passe robustes ;
- protéger les sauvegardes ;
- ne pas partager les bases de données contenant des informations réelles ;
- respecter les règles applicables en matière de protection des données personnelles.

Avant de publier des captures d’écran ou des exemples, vérifiez qu’ils ne contiennent aucun nom, numéro de téléphone, montant confidentiel ou autre donnée réelle identifiable.

## Sécurité et sauvegardes

L’application comprend des mécanismes de sauvegarde et de vérification de l’intégrité de la base de données. La sécurité globale dépend également de la protection de l’ordinateur, des comptes utilisateurs et des fichiers exportés.

Bonnes pratiques :
- réaliser des sauvegardes sur un support séparé et sécurisé ;
- tester périodiquement la restauration d’une sauvegarde ;
- ne jamais publier de clé privée, mot de passe, base de données client ou fichier d’activation ;
- ne pas envoyer de données personnelles par un canal non sécurisé.

## Captures d’écran

Des captures d’écran pourront être ajoutées après anonymisation des données.

Structure suggérée :

```text
docs/
└── screenshots/
    ├── dashboard.png
    ├── citizens.png
    ├── contributions.png
    └── statistics.png
```

Pour afficher une capture après l’avoir ajoutée :

```markdown
![Tableau de bord](docs/screenshots/dashboard.png)
```

## Licence et distribution

VillageManager est un logiciel propriétaire distribué commercialement. Sauf autorisation écrite du titulaire des droits, aucune disposition de ce dépôt ne donne le droit de :

- copier ou redistribuer le logiciel ;
- modifier ou décompiler le programme ;
- vendre, louer ou sous-licencier le logiciel ;
- réutiliser ses éléments propriétaires dans un autre produit.

Les conditions applicables sont celles du contrat ou de la licence remis avec la version distribuée. Les droits impératifs prévus par la loi restent applicables.

## Assistance

Pour toute question sur l’utilisation, la distribution ou une demande de démonstration, contactez le responsable du projet :

- **Contact :** jubatensaout23@gmail.com
- **Projet :** VillageManager

Avant de rendre ce dépôt public, remplacez le contact provisoire et vérifiez qu’aucune donnée confidentielle, clé privée, base de données réelle ou fichier de licence n’est inclus.
