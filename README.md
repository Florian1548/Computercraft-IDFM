<img src="https://pbs.twimg.com/media/HBdwNTiXQAAjPKH?format=jpg&name=4096x4096"  width="30%" height="15%">
# Programme d’affichage des trains via ComputerCraft

## Avertissement

* N’étant pas développeur Lua, ce programme a été généré par une IA.

>*L’IA est un outil, mais il faut comprendre ce que l’on fait pour savoir quoi lui demander.*

* Le jeton API n’est pas chiffré dans le fichier de configuration : n’importe quel joueur ayant accès à l’ordinateur ComputerCraft peut le lire.

## Description

Ce programme utilise l’API de la [Plateforme Régionale d'Information pour la Mobilité](https://prim.iledefrance-mobilites.fr/fr) (PRIM) d'[Ile De France Mobilité](https://www.iledefrance-mobilites.fr/) (IDFM).  
Après avoir renseigné un code gare, le programme va demander à l’API les 5 premiers départs de cette gare et les afficher dans l’ordre de départ, comme le ferait un véritable écran d’affichage SNCF. L’actualisation des données est réalisée toutes les minutes, la taille de l’écran ComputerCraft multiblocs est détectée et le contenu est automatiquement adapté.

## Installation et utilisation

Créez un compte sur le site de la [PRIM](https://prim.iledefrance-mobilites.fr) et récupérez votre jeton (copiez-le : il ne sera affiché qu’une seule fois).

Après avoir connecté un ou plusieurs écrans au PC ComputerCraft (advanced monitor pour avoir les couleurs), entrez :
```
pastebin get Byas76ec tchoo
```

Le programme va vous poser quelques questions qui seront sauvegardées dans l’ordinateur :
* "Entrez votre jeton API" : copiez-collez-le depuis votre interface PRIM, section ["Mes jetons"](https://prim.iledefrance-mobilites.fr/fr/mes-jetons-authentification).
* "Entrez votre code gare" : saisissez votre code unique de gare via [ce jeu de données](https://prim.iledefrance-mobilites.fr/fr/jeux-de-donnees/emplacement-des-gares-idf-data-generalisee), section "Tableau", recherchez votre gare (filtrez en "Mode" > "Train"), votre code est dans la colonne "id_ref_ZdA" copiez-collez sans espaces.
* "Nombre de trains à afficher" : 5 par défaut.
* "Lancer au démarrage ? y / n " : répondez "y" ou "n".

## Lancer le programme au démarrage

Lorsque vous quitterez votre partie solo ou éteindrez le serveur, tous les ordinateurs ComputerCraft s’éteindront. Vous devrez relancer votre programme en tapant le nom donné après la commande Pastebin (ici, dans l’exemple : "tchoo").
Pour pallier cela, répondez "y" à la question.

Et voilà !
