# Création Praticien / Annuaire RPPS

:::::{div} full-width

::::{grid} 2

:::{grid-item}
:columns: 9

> Dans le cadre de la **Cerification des LAD** (Logiciels d'Aide a la Dispensation) il est prévu que pour chaque praticien on doit mémoriser une fiche dans la *BDD ID*. On doit pouvoir consulter les numéros RPPS, rechercher un praticien par lieu d'exercice ...


:::

:::{grid-item}
:columns: 3

<div id="colour">

<br>
    
**ID version**: 2.20.3.1 <br>
**Page modifié le**: 18/12/2023


</div>

:::

::::

:::::

<br>

## L'annuaire RPPS

:::::{div} full-width

<p class="emphase2">Le Répertoire Partagé des Professionnels intervenant dans le système de santé (RPPS) </p>

::::{grid} 2

:::{grid-item}
:columns: 4

>Le RPPS intègre les données d'identification de l'ensemble des professionnels de santé, fournis et certifiées par les ordres professionnels et par le service de santé des armées. L'intégration est progressive, en fonction des possibilités des autorités d'enregistrement (ordre professionnel, agence régionale de santé, service de santé des armées). (cf Information sur le [site internet de l'ANS](https://esante.gouv.fr/produits-services/repertoire-rpps?position&keys=rpps&pageNumber=1)). L'annuaire des PS est mis à disposition par l'ANS (Agence du Numérique en Santé), il est intégré au LGO et accessible a tout moment.

:::

:::{grid-item}
:columns: 8

<iframe src="../../../_static/PDF/ans_tableau-des-populations-rpps.pdf" width="100%" height="400px"> </iframe>

:::

::::

:::::


:::::{div} full-width

::::{grid} 2

:::{grid-item}
:columns: 4

**Navigation**:

Fiche Praticien: <kbd data-key="F8"></kbd> 

Facturation: <kbd data-key="F7"></kbd> 

:::

:::{grid-item}
:columns: 8


```{note}

Pour les praticiens conventionnés, le numéro d'A.M est communiqué par la caisse de rattachement du PS, en principe mentionné sur les prescriptions. Il est nécessaire pour la facturation des TP ou HTP, il n'est pas disponible à partir de l'annuaire RPPS.

```

:::

::::

:::::

### Recherche

```{figure} Docs/Creation-prat-1.png
---
width: 100%
name: Creation-prat-1
---

```


### Selection

```{figure} Docs/Creation-prat-2.png
---
width: 100%
name: Creation-prat-2
---

```

Appuie sur Fin

### Création 

Le professionel de santé sur lequel on est positionné n'a pas été trouvé dans la BDD ID, la liste des correspondances est donc vierge.


### Mise a jour


## La fiche Praticien

Pour facturer en TP ou HTP, a ce jour il est obligatoire de renseigner le **numéro d'AM du prescriptuer**. Pour les praticiens rattachés à un établissement, c'est le **numéro FINESS de la structure** qui doit être renseigné. (cf creation de structure(link))

Pour un vétérinaire, vous cochez la case (+ rentrer le numéro ordinal), cette information est vérifiée lorsque vous facturez des produits vétérinaires soumis a prescription.


## Structure

### Creation

#### Médecin Hospitalier

Il faut créer sa fiche comme vu précedemment, puis on l'intègre à la liste des praticiens hospitaliers depuis la fiche de l'établissement.

#### Un établissement de santé


Pour créer l'hopital saisissez son nom ou son numéro pour lancer la recherche, choisissez l'option F3-Créer, puis prenez l'option structure. Ensuite complétez le nom, le FINESS et l'adresse de l'établissement.


### Multistructure

:::::{div} full-width

::::{grid} 2

:::{grid-item}
:columns: 7

<br>

<div id="speech-bubble">
    
J'ai un hopital proche de ma pharmacie dont chaque service possède son propre numéro FINESS ... Comment puis-je dissocier les médecins du service en question ...    
    
</div>

:::

:::{grid-item}
:columns: 5

```{note}

Un Praticien peut exercer au sein de plusieurs structures, pour saisir une structure de rattachement supplémentaire, cliquez sur INSER puis sélectionnez le type de structure (hopital ou cabinet), et renseignez l'adresse ..., si besoin, ajouter le numéro d'A.M de cette nouvelle structure de rattachement.


```

:::

::::


<br>
<br>


```{figure} Docs/Crea-prat-3.png
---
width: 100%
name: Creation-prat-2
---

```

:::::



