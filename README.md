# SlydeForge — Téléchargements / Downloads

[🇫🇷 Français](#-français) · [🇬🇧 English](#-english)

---

## 🇫🇷 Français

**SlydeForge** est un logiciel de création de présentations assisté par l'IA : vous décrivez votre sujet, SlydeForge construit la présentation (plan, textes, mises en page, graphiques, images) dans le respect de votre charte graphique. Vous retouchez ensuite chaque slide, vous l'animez, puis vous l'imprimez ou l'exportez en PowerPoint, PDF ou vidéo.

👉 Site officiel, version Windows, guides et tarifs : **<https://slydeforge.com/>**

Ce dépôt ne contient **pas de code** : il héberge uniquement les fichiers à télécharger de l'**édition Docker** de SlydeForge.

### Qu'est-ce que l'édition Docker ?

SlydeForge, dans votre navigateur, sur un serveur qui vous appartient :

- 🌐 **Rien à installer sur les postes** : on ouvre une adresse et on retrouve SlydeForge complet.
- 💻 **Windows, Mac, Linux et autres** : toute personne avec un navigateur récent peut travailler.
- 👥 **Comptes et équipes** : invitations par lien, ou connexion avec l'annuaire de l'entreprise (Active Directory / LDAP, Microsoft Entra, Google, Keycloak…).
- 🔒 **Vos données chez vous** : présentations, comptes et réglages restent sur votre machine ou votre réseau ; chaque personne travaille dans une session séparée.
- 🔄 **Mises à jour en un clic** depuis la console d'administration, avec sauvegarde avant et retour automatique à l'ancienne version en cas de problème.
- 🧑 **Seul ou en équipe** : sur un poste seul, aucun compte n'est nécessaire.

### Installer (Windows)

1. Téléchargez **`SlydeForge-Docker-Setup.exe`** dans la section *Releases* (colonne de droite).
2. Double-cliquez et suivez les étapes. L'installateur propose d'installer **Docker Desktop** s'il est absent ; au premier démarrage de Docker Desktop, cliquez sur **« Skip »** à l'écran « Welcome to Docker » : aucun compte n'est nécessaire.
3. L'installateur télécharge l'image de SlydeForge (environ 800 Mo), démarre le serveur, puis **ouvre une page web** pour terminer la configuration (seul ou en équipe, compte administrateur).

Pour redémarrer ou rouvrir SlydeForge plus tard : menu Démarrer › **SlydeForge Docker**.

### Installer à la main (Linux, macOS, serveur)

SlydeForge fonctionne partout où Docker fonctionne. Avec l'archive `SlydeForge-x.y.z-docker.tar.gz` de la release :

```bash
# 1. Vérifier l'empreinte (comparez avec celle indiquée dans la release)
sha256sum SlydeForge-1.6.0-docker.tar.gz

# 2. Charger l'image
gunzip -c SlydeForge-1.6.0-docker.tar.gz | docker load
```

Les lanceurs Linux et macOS (avec console d'administration web) sont en préparation.

### Vérifier le téléchargement

L'empreinte **SHA-256** de chaque archive est publiée avec sa release. Le lanceur Windows la vérifie automatiquement avant d'installer.

| Version | SHA-256 de `SlydeForge-1.6.0-docker.tar.gz` |
|---|---|
| 1.6.0 | `8a1c65bf30ec890305c33c50acbf79377b69ca08cd71db54c6b5d17a5f160a7e` |

### Configuration requise

- Docker Desktop (Windows, macOS) ou Docker Engine (Linux).
- Environ 3 Go d'espace disque pour l'image, 4 Go de mémoire vive conseillés.
- Un navigateur récent pour les utilisateurs.

Docker Desktop est gratuit pour un usage personnel, l'enseignement et les petites entreprises ; certaines organisations doivent souscrire un abonnement (voir <https://www.docker.com/pricing/>).

### Aide

- Documentation et guides : <https://slydeforge.com/>
- Une question, un problème : <https://slydeforge.com/fr/contact.php>

© SlydeForge — Emilien MOREL. Tous droits réservés.

---

## 🇬🇧 English

**SlydeForge** is an AI-assisted presentation maker: you describe your topic, SlydeForge builds the presentation (outline, text, layouts, charts, images) in line with your brand guidelines. You then fine-tune each slide, animate it, then print it or export it to PowerPoint, PDF or video.

👉 Official website, Windows version, guides and pricing: **<https://slydeforge.com/>**

This repository contains **no code**: it only hosts the downloads of the SlydeForge **Docker edition**.

### What is the Docker edition?

SlydeForge in your browser, on a server that belongs to you:

- 🌐 **Nothing to install on people's computers**: open an address and the full SlydeForge is there.
- 💻 **Windows, Mac, Linux and more**: anyone with a recent browser can work.
- 👥 **Accounts and teams**: invitation links, or sign-in with the company directory (Active Directory / LDAP, Microsoft Entra, Google, Keycloak…).
- 🔒 **Your data stays with you**: presentations, accounts and settings stay on your machine or your network; each person works in a separate session.
- 🔄 **One-click updates** from the administration console, with a backup first and an automatic return to the previous version if anything goes wrong.
- 🧑 **Alone or as a team**: on a single computer, no account is needed.

### Install (Windows)

1. Download **`SlydeForge-Docker-Setup.exe`** from the *Releases* section (right column).
2. Double-click it and follow the steps. The installer offers to install **Docker Desktop** if it is missing; on Docker Desktop's first start, click **"Skip"** on the "Welcome to Docker" screen: no account is needed.
3. The installer downloads the SlydeForge image (about 800 MB), starts the server, then **opens a web page** to finish the setup (solo or team, administrator account).

To restart or reopen SlydeForge later: Start menu › **SlydeForge Docker**.

### Manual install (Linux, macOS, server)

SlydeForge runs wherever Docker runs. With the release's `SlydeForge-x.y.z-docker.tar.gz` archive:

```bash
# 1. Check the checksum (compare with the one given in the release)
sha256sum SlydeForge-1.6.0-docker.tar.gz

# 2. Load the image
gunzip -c SlydeForge-1.6.0-docker.tar.gz | docker load
```

Linux and macOS launchers (with the web administration console) are in preparation.

### Verify your download

The **SHA-256** checksum of each archive is published with its release. The Windows launcher checks it automatically before installing.

| Version | SHA-256 of `SlydeForge-1.6.0-docker.tar.gz` |
|---|---|
| 1.6.0 | `8a1c65bf30ec890305c33c50acbf79377b69ca08cd71db54c6b5d17a5f160a7e` |

### Requirements

- Docker Desktop (Windows, macOS) or Docker Engine (Linux).
- About 3 GB of disk space for the image, 4 GB of RAM recommended.
- A recent browser for the users.

Docker Desktop is free for personal use, education and small businesses; some organizations need a subscription (see <https://www.docker.com/pricing/>).

### Help

- Documentation and guides: <https://slydeforge.com/>
- A question or a problem: <https://slydeforge.com/en/contact.php>

© SlydeForge — Emilien MOREL. All rights reserved.
