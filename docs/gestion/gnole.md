# GNôle (GN Manager)

**GNôle** (nom de projet : `gnmanager`) est une application web libre et centralisée conçue spécifiquement pour simplifier l'organisation et le pilotage logistique des jeux de rôles grandeur nature (GN).

---

## 🔗 Liens Rapides

* 🌐 **Déploiement en ligne (auto-hébergé)** : [https://minimoi.mynetgear.com/gnole](https://minimoi.mynetgear.com/gnole)
* 💬 **Communauté & Support Discord** : [https://discord.gg/EPNhfw7X3z](https://discord.gg/EPNhfw7X3z)
* 💻 **Dépôt GitHub** : [github.com/Pommovore/gnmanager](https://github.com/Pommovore/gnmanager)

---

## 🎯 Présentation du Projet

L'organisation d'un grandeur nature implique traditionnellement de jongler entre de multiples tableurs, formulaires épars, échanges de mails interminables et fiches de personnages distribuées au compte-gouttes.

**GNôle** résout cette fragmentation en fournissant une plateforme unifiée qui rassemble à la fois :
1. **L'espace des participants** : consultation du catalogue des événements, inscription, suivi de validation, paiement et accès sécurisé à leur fiche de rôle.
2. **L'atelier des organisateurs** : outils de casting assisté par algorithme, suivi financier (PAF), génération de trombinoscope prêt à imprimer et communication automatisée.
3. **Le panneau d'administration** : supervision globale, gestion fine des accès et traçabilité des opérations.

---

## ⚙️ Fonctionnalités Principales

### 1. Gestion des Événements & Inscriptions
* **Fiche d'événement complète** : dates, lieux, jauge de participants, description, règles spécifiques et association organisatrice.
* **Formulaires d'inscription intégrés** : choix du type de participation (PJ, PNJ, Organisateur), souhaits de factions/groupes, contraintes et préférences alimentaires.
* **Import Google Forms** : importation directe des réponses CSV avec système d'alias et mapping intelligent des colonnes pour les campagnes d'inscriptions externes.
* **Suivi de la PAF (Participation Aux Frais)** : suivi en temps réel des encaissements, méthodes de paiement et soldes dus par participant.

### 2. Module de Casting Intelligent
* **Matrice Rôles / Participants** : interface visuelle croisant l'ensemble des inscrits et des rôles à pourvoir.
* **Scoring d'adéquation (0 à 10)** : notation personnalisée de la compatibilité entre un joueur et un personnage selon ses souhaits et affinités de jeu.
* **Algorithme d'attribution automatique ("Casting pondéré")** : calcul et proposition d'une répartition optimale équilibrée minimisant les frustrations.
* **Scénarios de casting alternatifs** : colonnes de simulation pour tester et comparer différentes options avant validation finale.

### 3. Fiches de Personnages & Trombinoscope
* **Distribution des rôles & documents** : rattachement de documents de jeu (PDF, Google Docs) consultables directement depuis l'espace personnel du joueur une fois le casting publié.
* **Trombinoscope dynamique** :
    * Visualisation claire avec cadre coloré selon la disponibilité de la photo (photo personnalisée validée, avatar de profil, photo manquante, rôle non attribué).
    * Dispositions modulables (1, 2 ou 4 portraits par ligne).
    * Export **ODT** prêt à l'impression pour le livret orga.
    * Export **ZIP** de l'ensemble des photos avec convention de nommage standardisée.

### 4. Communication & Intégrations
* **Webhooks Discord** : notifications automatisées des nouvelles inscriptions, des changements d'état et des annonces directement dans les salons de votre serveur associatif.
* **Export emails formaté** : extraction en un clic de la liste des adresses emails des participants filtrés au format standard (`Nom <email@domaine.com>`).
* **Exports tabulaires CSV/Excel** : export des listes d'inscrits, régimes, fiches et statuts pour un usage hors-ligne.

### 5. Ergonomie & Données Personnelles
* **Interface moderne & réactive** : réalisée avec Bootstrap 5, compatible mobile, avec alternance dynamique thème clair / thème sombre.
* **Respect de la vie privée (RGPD)** : modale de gestion de profil complète avec procédure de désinscription autonome et option de purge définitive des données personnelles.

---

## 💻 Architecture Technique

Le projet repose sur des standards modernes, légers et pérennes :

* **Backend** : Python (FastAPI / Flask) avec ORM SQLAlchemy.
* **Base de données** : SQLite (idéal pour l'auto-hébergement, la sauvegarde instantanée et la simplicité de maintenance).
* **Frontend** : HTML5, Vanilla JavaScript moderne (ES6+), Bootstrap 5.3 et Bootstrap Icons.
* **Gestionnaire de dépendances** : `uv` pour des installations ultra-rapides et des environnements reproductibles.

---

## 🚀 Accéder et Découvrir GNôle

Pour tester l'application ou suivre le développement :

* Visitez l'instance de démonstration auto-hébergée sur [https://minimoi.mynetgear.com/gnole](https://minimoi.mynetgear.com/gnole).
* Rejoignez le serveur Discord d'entraide et d'échange [https://discord.gg/EPNhfw7X3z](https://discord.gg/EPNhfw7X3z) pour poser vos questions, échanger des retours ou contribuer à l'évolution de la plateforme.
