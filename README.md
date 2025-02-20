# Guide des Commandes Linux

## 1. Commandes de Base

### Affichage d'informations sur l'utilisateur et le système
- `whoami` : Affiche le nom de l'utilisateur actuel.
- `hostname` : Affiche le nom de la machine.
- `pwd` : Affiche le répertoire de travail actuel.
- `ls` : Liste les fichiers et dossiers du répertoire actuel.
- `cd [répertoire]` : Change de répertoire.
- `cd ..` : Remonte d'un niveau dans l'arborescence.

### Manuel et Aide
- `man [commande]` : Affiche la documentation d'une commande.
- `info [commande]` : Affiche les informations détaillées.
- `[commande] --help` : Affiche une aide rapide sur une commande.

## 2. Manipulation des fichiers et répertoires

### Lecture de fichiers
- `cat [fichier]` : Affiche le contenu d'un fichier.
- `more [fichier]` : Affiche le fichier page par page.
- `less [fichier]` : Similaire à `more` avec la possibilité de revenir en arrière.
- `head [fichier]` : Affiche les premières lignes du fichier.
- `tail [fichier]` : Affiche les dernières lignes du fichier.

### Création et modification de fichiers
- `touch [fichier]` : Crée un fichier vide.
- `mkdir [répertoire]` : Crée un répertoire.
- `cp [source] [destination]` : Copie un fichier ou un dossier.
- `mv [source] [destination]` : Déplace ou renomme un fichier/dossier.
- `rm [fichier]` : Supprime un fichier.
- `rm -r [répertoire]` : Supprime un répertoire et son contenu.

## 3. Gestion du système de fichiers

### Chemins et navigation
- `.` : Répertoire courant.
- `..` : Répertoire parent.
- `/` : Répertoire racine.
- `~` : Répertoire personnel de l'utilisateur.
- `ls -l` : Affiche la liste détaillée des fichiers.
- `ls -a` : Affiche tous les fichiers, y compris les fichiers cachés.

### Rechercher des fichiers
- `find [chemin] -name "nom_du_fichier"` : Recherche un fichier par nom.
- `locate [nom_du_fichier]` : Trouve un fichier à l'aide d'une base de données mise à jour.
- `which [commande]` : Affiche le chemin d'exécution d'une commande.
- `whereis [commande]` : Affiche les emplacements possibles d'une commande.

## 4. Gestion des utilisateurs et permissions

### Informations sur les utilisateurs
- `who` : Liste des utilisateurs connectés.
- `w` : Affiche des détails sur les utilisateurs connectés.
- `users` : Affiche les utilisateurs connectés en une ligne.
- `id` : Affiche l'UID et GID de l'utilisateur actuel.

### Gestion des permissions
- `ls -l` : Affiche les permissions des fichiers et dossiers.
- `chmod [mode] [fichier]` : Change les permissions d'un fichier.
  - Ex : `chmod 755 script.sh` (lecture, écriture, exécution pour l'utilisateur ; lecture, exécution pour les autres).
- `chown [utilisateur]:[groupe] [fichier]` : Change le propriétaire d'un fichier.
- `chgrp [groupe] [fichier]` : Change le groupe propriétaire d'un fichier.

## 5. Compression et archivage

- `zip [archive.zip] [fichier]` : Compresse un fichier en ZIP.
- `unzip [archive.zip]` : Décompresse un fichier ZIP.
- `tar -cvf [archive.tar] [fichier/dossier]` : Crée une archive TAR.
- `tar -xvf [archive.tar]` : Extrait une archive TAR.
- `tar -czvf [archive.tar.gz] [fichier/dossier]` : Crée une archive compressée en Gzip.
- `tar -xzvf [archive.tar.gz]` : Extrait une archive Gzip.

## 6. Gestion des processus

- `ps` : Affiche les processus en cours.
- `ps aux` : Liste tous les processus en cours d'exécution.
- `top` : Affiche les processus en temps réel.
- `kill [PID]` : Tue un processus par son PID.
- `killall [nom_du_processus]` : Tue tous les processus portant ce nom.
- `jobs` : Liste les processus en arrière-plan.
- `bg [numéro]` : Remet un processus en arrière-plan.
- `fg [numéro]` : Remet un processus en avant-plan.

## 7. Gestion du réseau

- `ping [adresse]` : Vérifie la connectivité réseau.
- `ifconfig` ou `ip address` : Affiche les informations des interfaces réseau.
- `netstat -lt` : Affiche les ports ouverts.
- `nslookup [nom_de_domaine]` : Résout un nom de domaine.
- `dig [nom_de_domaine]` : Résout un nom de domaine avec plus de détails.
- `scp [fichier] utilisateur@ip:/chemin` : Copie un fichier à distance.
- `ssh utilisateur@ip` : Se connecte à une machine distante.

## 8. Redirection et pipes

- `>` : Redirige la sortie vers un fichier (écrase le fichier existant).
- `>>` : Redirige la sortie vers un fichier (ajoute à la fin).
- `<` : Prend l'entrée depuis un fichier.
- `|` : Enchaîne les commandes.
- `ls | grep "mot"` : Filtre les résultats avec `grep`.

## 9. Automatisation et scripts

### Création de scripts Bash
Un script Bash commence par :
```bash
#!/bin/bash
```

Exemple :
```bash
#!/bin/bash
echo "Bonjour, $USER !"
pwd
ls -l
```
Pour rendre un script exécutable :
```bash
chmod +x script.sh
./script.sh
```

## 10. Autres commandes utiles

- `history` : Affiche l'historique des commandes.
- `alias ll='ls -l'` : Crée un alias pour une commande.
- `unalias ll` : Supprime un alias.
- `clear` : Nettoie l'écran du terminal.
- `exit` : Ferme le terminal.

---
**📌 Astuce** : Pour approfondir ces commandes, utilise `man` ou `--help` après chaque commande !

