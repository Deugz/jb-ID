# Smart RX


SmartNev (nouvel procedure pour transferer du SmartRX)

```{note}

Pas besoin de changer les DLL

```

## Spécificités

## Etapes

### Import des données vers le PC

```{warning}

Transferer les données depuis le disque dur vers ordi (C://)

- Checker Cedric doc

```

3 Fichiers

- Client 
- Extraction
    - tmp
- Scan


### Ouvre Dossier Commit 

Dossier Commit 4.8 est une boite a outil qui contient le **logiciel Commit** mais également tout un tas d'outil nécessaire a la réalisation des commits

- On récupère un fichier Dump.sql (Modules/Import/Ressources/NEV/)

On copie et on colle le ficher dans le dossier (Extraction/temp)


#### Lancer Commit

Executer en tant qu'administrateur

- Mise a jour ? Toujours faire une mise a jour quand on commence un nouveau projet


### Créer Nouveau Projet

Ouvre une fenetre pop up

- Import: On selectione le logiciel a parti duquel on ytransfer
    - NEV - SmartRXNEV
    
- Fichier projet: On insere le lien d'arborexscenve vers le dossier qui contient le fichier dump.sql (Extraction/temp), et rentre un nom de fichier (mon choix, exemple testpharmadate) et Enregistrer

.pj4

- OK

```{note}

Est-ce

```

### Options de Reprise

- Cocher deconditionnement des stupéfiants

- OK



### Investigation Base de donnée 

Observation rapide si pas d'erreur

- Praticiens
- Organismes
- Clients
- Produits
- Encours
- Autres donneées
- Programme fidelité
- Conversion


```{note}

Faire capture écran et expliquer les differentes sections


```

### Connexion

Bouton a droite

```{note}

Message erreur, car base pas créé

```

- On ne touche pas le haut de la page (PostgreSQL)

Dans l'onglet DUMP SQL on le met le chemin vers le fichier dump.sql


On clique sur restaurer (*peut etre*)

OK

Message vert qui apparait en dessous de import de donnée (pouce levé emoji)

- Créé un serveur local SQL qui va travailler sur la Base de Donnée


### Reprise de données

Cliuquer sur petite flèche a coté et on clique sur **toute les données**

