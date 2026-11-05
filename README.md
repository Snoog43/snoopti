# Snoopti

Optimiseur Windows pour le jeu : réglages Windows, services, réseau, NVIDIA, applis, jeux, latence.

## Installer

Ouvrir PowerShell (clic droit sur Démarrer, « Terminal » ou « Windows PowerShell »), coller puis Entrée :

```powershell
irm https://raw.githubusercontent.com/Snoog43/snoopti/main/install.ps1 | iex
```

La commande télécharge le dernier `Snoopti-Setup.exe` (onglet Releases), vérifie son empreinte SHA256 et l'ouvre. Accepter la demande administrateur, puis « Installer ». Relancer la même commande plus tard met Snoopti à jour.

Sans PowerShell : télécharger `Snoopti-Setup.exe` dans [Releases](https://github.com/Snoog43/snoopti/releases/latest). Exe non signé : Windows affiche SmartScreen, cliquer « Informations complémentaires » puis « Exécuter quand même ».

## Ce qu'il installe

- Snoopti dans `C:\Program Files\Snoopti`, raccourcis menu Démarrer et bureau, désinstallation depuis Paramètres > Applications.
- Seulement ce qui manque : Visual C++, DirectX, et avec une carte NVIDIA son panneau de configuration et Profile Inspector.
- Rien ne se lance au démarrage de Windows, rien ne tourne en fond.

## À savoir

- Avant tout : bouton « Opti tout en un » du tableau de bord, ou page par page. Un point de restauration est créé, et « État d'origine » (page Windows) remet tout comme avant.
- Pages BIOS et Overclock : cartes mères MSI seulement, avec SCEWIN (non fourni). Ne pas s'en servir sur une autre carte.
