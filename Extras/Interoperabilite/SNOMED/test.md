# Test

## Intro


```{note}

Check Chat GPT discussion relative to this topic

```

### Semantic Web

```{note}

Inclure les ressources dans nb-tools et inserer lien vers ce dernier

```

- [Youtube Tutorial](https://www.youtube.com/watch?v=CubeRifQy7I&list=PLea0WJq13cnDDe8V7eVLReIaOnFztOEAq&index=14)
- [Article](https://www.cs.umd.edu/projects/plus/SHOE/pubs/iwann99.pdf)

#### HL7 FHIR

- [Good Doc w/ examples](https://hl7.org/FHIR/allergyintolerance-example.html)

- [ANS Doc sur FHIR](https://industriels.esante.gouv.fr/sites/default/files/media/document/Global_features_FHIR_Server_version_finale_v5.pdf)

- [FHIR](https://fhir-drills.github.io/index.html)



## SNOMED

### Snomed Browser

- [Website](https://browser.ihtsdotools.org/?)
- [Github Repo](https://github.com/IHTSDO/sct-browser-frontend)

### Récupérer SNOMED



- [Technical documentation](https://www.nrces.in/download/files/pdf/doc_TechnicalImplementationGuide_Current-en-US_INT_20150131.pdf)
- [Confluence](https://confluence.ihtsdotools.org/display/DOCANLYT/Data+Analytics+with+SNOMED+CT)



- [**Good Youtube Example**](https://www.youtube.com/watch?v=GZmxDVlHKRc)

```{note}

Bon tuto qui explique comment télécharger l'ontologie tout ca, a checker, au moins pour les premières étapes. Cependant l'auteur ([Youtube Channel link]()) utilise [GO](https://go.dev/doc/articles/wiki/), pour construire son application.

```

Snowmed in 5 minute, github repo avec exemples pour accéder a l'API.

-[Github repo](https://github.com/IHTSDO/SNOMED-in-5-minutes/tree/master)

```{warning}

J'ai télécharger le fichier: Inclure le html sur la page Snowmed. 

```

- [SPHN](https://sphn-semantic-framework.readthedocs.io/en/latest/external_resources/snomed-ct.html)



### Ontology conversion

#### To OWL

- [Youtube tuto](https://www.youtube.com/watch?v=sfFbMMioA_4)




### Browser API

- [Youtube Tutorial](https://www.youtube.com/watch?v=Yl-6DT0VPDU)


#### Other API's

- [Hermes](https://github.com/wardle/hermes)


## Installation

```{code-block} js

    var ontologyFile = 'chemin/vers/votre-ontologie.rdf';

    fetcher.nowOrWhenFetched(ontologyFile, function(success, error) {
        if (!success) {
            console.error('Erreur lors du chargement du fichier RDF :', error);
            return;
        }

        // Supposons que l'ontologie utilise le préfixe "snomed" pour les concepts
        var snomed = $rdf.Namespace('http://snomed.org/ontology#');

        // Recherche de tous les problèmes de santé dans l'ontologie
        var healthIssues = store.each(undefined, snomed('type'), snomed('HealthIssue'));

        // Affichage des informations dans le HTML
        var healthIssueContainer = document.getElementById('health-issue-container');

        healthIssues.forEach(function(issue) {
            var conceptID = store.any(issue, snomed('conceptID'));
            var name = store.any(issue, snomed('name'));
            var description = store.any(issue, snomed('description'));

            var issueDiv = document.createElement('div');
            issueDiv.innerHTML = `<h2>${name.value}</h2><p>Concept ID: ${conceptID.value}</p><p>Description: ${description.value}</p>`;
            healthIssueContainer.appendChild(issueDiv);
        });
    });
});


```