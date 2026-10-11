# AtelierFlow — À mentionner dans le TP / dossier projet et le DP

## Objectif de cette note

Cette note sert à ne pas oublier une fonctionnalité métier importante : la gestion des clients.

Dans AtelierFlow, on ne doit pas seulement créer des commandes. Une commande doit être rattachée à un client. L’application doit donc permettre de créer, consulter et utiliser une fiche client.

---

## 1. Partie TP / dossier projet / présentation

Dans le dossier projet et dans la présentation du titre professionnel, la création des clients doit être présentée comme une vraie fonctionnalité métier.

### Fonctionnalité à mentionner

L’application permet au responsable de l’atelier de créer une fiche client avant de créer une commande.

La fiche client peut contenir :

- nom ;
- prénom ;
- téléphone ;
- email si nécessaire ;
- notes client ;
- historique des commandes.

### Logique métier à expliquer

Le client est au centre du suivi de l’atelier.

Une commande n’existe pas seule : elle est liée à un client. Cela permet de retrouver rapidement qui a passé commande, de suivre les anciennes commandes, de vérifier les paiements et de mieux organiser les échanges avec le client.

Schéma logique à présenter :

```text
Client → Commande → Étapes de fabrication → Paiements → Suivi client
```

### Exemple de phrase pour le dossier projet

> Avant de créer une commande, le responsable de l’atelier peut créer ou sélectionner un client. La commande est ensuite rattachée à cette fiche client. Cela permet de centraliser les informations du client, de suivre ses commandes en cours, son historique et les paiements associés.

### Exemple de phrase pour l’oral

> J’ai ajouté une gestion des clients, car dans un atelier de couture on ne suit pas seulement une commande isolée. On doit aussi savoir qui est le client, quelles commandes il a déjà passées, combien il a payé et où en est sa commande actuelle.

---

## 2. Écrans à prévoir dans Figma

### Écran liste des clients

À prévoir dans la maquette :

- titre : « Clients » ;
- bouton : « Nouveau client » ;
- barre de recherche ;
- liste des clients avec nom, téléphone et nombre de commandes ;
- action : voir la fiche client.

### Écran création client

À prévoir dans la maquette :

- champ nom ;
- champ prénom ;
- champ téléphone ;
- champ email optionnel ;
- champ notes ;
- bouton « Enregistrer le client ».

### Écran fiche client

À prévoir dans la maquette :

- informations du client ;
- commandes en cours ;
- anciennes commandes ;
- paiements liés ;
- bouton « Nouvelle commande pour ce client ».

---

## 3. À intégrer dans le développement AtelierFlow

### Front-end

Prévoir :

- une page ou section « Clients » ;
- un formulaire de création client ;
- une fiche client ;
- un lien entre la fiche client et la création de commande.

### Back-end

Prévoir au minimum :

- une entité ou table `Client` ;
- une relation entre `Client` et `Commande` ;
- une route ou action pour créer un client ;
- une route ou action pour consulter un client ;
- une route ou action pour créer une commande rattachée à un client.

### Base de données

Exemple de relation :

```text
Client 1,n Commande
Commande 1,n Étape
Commande 1,n Paiement
```

---

## 4. Partie DP — dossier professionnel

Attention : si AtelierFlow est utilisé comme projet principal pour le dossier projet / TP, il vaut mieux éviter de réutiliser exactement le même projet comme exemple principal dans le dossier professionnel, sauf validation du formateur.

Par contre, dans le DP, il faut montrer que la compétence est maîtrisée : savoir gérer une entité métier, créer un formulaire, relier des données et exploiter une base de données.

### Formulation possible dans le DP

> J’ai participé à la création d’une fonctionnalité de gestion d’entités métier, avec un formulaire de création, une page de consultation et un rattachement à d’autres données de l’application. Ce type de fonctionnalité permet par exemple de gérer des fiches clients et de les relier à des commandes.

### Compétences que cela peut illustrer

- créer une interface utilisateur ;
- créer un formulaire ;
- valider les données saisies ;
- enregistrer des données en base ;
- relier deux entités métier ;
- afficher des informations liées ;
- sécuriser l’accès aux données.

---

## 5. À ne pas oublier dans le plan de travail

À ajouter dans AtelierFlow :

```text
Créer un client
Consulter la liste des clients
Consulter une fiche client
Créer une commande rattachée à un client
Voir l’historique des commandes d’un client
Voir les paiements liés au client
```

Cette partie doit apparaître dans le TP / dossier projet, dans la présentation orale, et sous forme de compétence dans le DP.