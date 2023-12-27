# Ventes Ordonnances

```{note}

Logiciel téléconsulte: Maya

```

## Procedure

```{note}

Insérer diagramme
- Utiliser les differentes étapes étapes en titres

```

### Code Operateur

Code porteur, si première vente

```{admonition} Info

Si Lecteur de CV bloqué, possibilité de débloquage Configuration/Materiel/Lecteur/F2-Débloquer

```

Difference CPS / CPE

- CPS, Carte professionel de santé (1 par pharmacien)
- CPE, Carte professionel d'Etablissement (commandé pour combler le nombre de poste restant)


```{warning}

On ne peut teletransmettre que a partir d'un poste qui possède une CPS 


```

**Example**:



### Identification patient

::::{grid} 2

:::{grid-item}

#### Avec Carte vitale


Insérez la carte vitale dans le lecteur et appuyez sur <kbd data-key="F8"> </kbd> 

(vous pouvez aussi cliquer sur l'icone en bas de la page a l'aide de votre souris)


:::


:::{grid-item}

#### Sans Carte vitale

Rentrez Manuellement nom du patient

```{note} Astuces

- (*) Pour finir automatiquement le mot ...
- (+) pour ajouter prénom aprés le nom
- etc



```

<h5> <kbd data-key="F7"></kbd>  -  ADRi </h5>

Permet de checker les droits (Attention pas toujours juste)
- Base Amelie



:::

::::

### Identif Prescripteur

#### Importer

Permet de se substituer a la création manuelle

- Multistructure possible

#### Vétérinaires

Pour créer un vétérinaire il faut:
- Cocher l'option médecin vétérinaire
- Rentrer un numéro ordinal (inscrit sur l'ordonnance)

### Date Prescription

#### Renouvellement

### Prise en charge

sections pour tarification specifique (specifique au patient ie difference si sncf, msa etc ...)
- cf liens vers Page Maternité ...

```{note}

Consultation des droits possibles sur ADRI (Aquisition des Droits intégrés)


```

#### Patients

- Patient normal
- Patient ALD (médecin fait demande a l'assurance maladie, valable 5 ans)
- Patient invalide
- AT
- Maternité
- Nourisson
- Pauvre- CSS (Couverture Santé Solidaire)


#### Organisme

- AMO (assurance maladie obligatoire). Différents:
    - CPAM: Caisse Primaire Assurance Maladie (identification 01)
    - MSA: Régime sociale agricole (identification 02)
    - RSI: Régime sociale indépendant (identification 03) a disparu depuis 2020
    - Regime spéciaux (SNCF, RATP, ENIM)
    - Gestion unique (MGEN, MGH ...)


#### Autres

##### Dprev



##### SPExo

### Vente 

VD en meme temps que ordo, meilleur pour les statistiques (panier moyen, frequentation etc ...)

Produit propose generique
- generiques preferentiel etc ....

- SPexo (dossier a part)

```{warning}

PAS DE STOCK NEGATIF DANS LGPI - Dus

- Si erreur possibilité de supprimer le dus directement dans la facturation.
    - Jamais corriger le stock pendant la vente
    
- Possibilité de générer un dues manuellemtn si volonté de conserver du stock (exemple)
    - exemple gardes etc..

```
    
```{note}

Possibilité de faire des commandes specifiques pour guarde


```

F7 recherche DC quand on entre une DCI (ajoute les princeps) - recherche DCI existe pas avec Winpharma


#### Produits

```{note}
Appel produit - Base de donnée pharmacie - si pas présent - BCB - Proposition Importer
```

- Si longue liste: Possibilité de filtrer en appuyant sur F10

##### Medicaments 

- les medicaments qui apparaissent sont ceux avec lequel j'ai déja travaillé (possibilité de filtrer avec * exemple Amo*500)

*profenid fait apparaitre
    - Biprofenid
    - Bi-profenid

- possibilité d'importer depuis la base clade bernard

```{admonition} diffference winfarma

Winfarma travail avec la base de donnée complete

```


#### Génériques

##### Préférentiels

Les Genériques préférentiels sont cochés quand on a le menue déroulant apres selection du princeps

```{note}

Checker les options de configurations (important)

```


### Interactions / Incompatibilités

#### F10

### Serialisation

Au scan du code data matrix 

```{note}

Checker differents types de robots et comment leyur sérialisation est prise en compte

```

### Feuille de Soins Electroniques

#### Tiers Payant

Dispensation du patient de l'avance des frais


#### Hors Tiers Payant

On le fait jamais



### Encaissement


### Validation

- Quantités évite erreurs

- Generiques 
    - MTE marge therapeutique étroite

Possibilité de le faire a la ligne ou a la vente
    
```{admonition} Question
:class: warning

Comment ca se materialise aprés la vente (tracabilité, statistique)

```

- Tiers Payant
- Hors Tiers Payant

Selection puis impression menue

QUAND VALIDATION PROPOSITION DE SCANNER L'ORDONNACE

### Reglement

F8 permet de revenir en arriere si facturation deja selectionné

F10 remise (pourcentage ou montant)


#### CGC compte rond

- passe en perte et profit

Question de tva (a checker ...) 

#### Cheques

- Possibilité de différer

#### Credits

...

```{note}

Beaucoup d'option possible, gros avantage de lgpi


```

Z encaissemnt central (specifique pharmacie rocade ou tarification et encaissemnt sont séparés)


#### Ticket de caisse

Enveloppe permet d'envoyer le ticket par mail 


## Renouvellement


## Ordonnance numérique

Pleine évolution, souhait de l'assurance maladie pour limiter les falsifications:

- Ordonnace numérique -> serveur CPAM + patiente (papier avec un QR code - éléments qui permettent de retrouver l'ordo dans la base de donnée)


```{note}

Pas confondre avec e-ordo. Ordo générés par EHPAD malta que le pharmacien recoit automatiquement via une application LGPI

```

```{admonition} Logiciels Médecin

- Quels logiciels de chez nous permettent de réaliser des ordonnances numériques

```

Présente l'ordo a la pharma, le pharmacien scan le QR code qui va rapatrier l'ordo numérique a la pharma.

Ensuite ?

```{note}

Checker la documentation surmon assistance / confluence (confluence - Formations clients/ Universités 2023 / UV9 / video)

```