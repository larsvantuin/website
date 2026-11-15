# Website Lars van Tuin

Deze site draait op GitHub Pages met Jekyll. Na elke wijziging bouwt GitHub de site binnen 1 à 2 minuten opnieuw.

## Iets toevoegen (zonder te programmeren)

Alle inhoud staat in de map `_data`. Open op github.com het bestand, klik op het potloodje (Edit), pas het aan en klik op **Commit changes**.

| Wat | Bestand |
|---|---|
| Wetenschappelijke publicatie | `_data/wetenschappelijk.yml` |
| Column, blog, whitepaper | `_data/publieksstukken.yml` |
| Interview, podcast, video, persbericht | `_data/media.yml` |
| Lezingonderwerpen | `_data/lezingen.yml` |
| Onderzoekslijnen | `_data/onderzoek.yml` |
| Links, e-mailadres, foto's | `_data/profiel.yml` |

Een nieuwe publicatie toevoegen: kopieer een bestaand blok, zet het **bovenaan** de lijst en pas het aan:

```yaml
- jaar: 2027
  titel: "Titel van het artikel"
  bron: "Journal of Occupational Health Psychology"
  met: "Medeauteur A, Medeauteur B"
  link: "https://doi.org/..."
```

Let op: de regels in een blok beginnen met twee spaties, en tekst met een dubbele punt erin zet je tussen aanhalingstekens.

## Foto's

Zet de foto's in `assets/img/` (Add file → Upload files) met dezelfde namen als in `_data/profiel.yml`: `portret.webp`, `lezing.webp`, `collegezaal.webp`.

## Teksten

De vaste teksten (hero, Over mij, Contact) staan in `index.html`. De Engelse pagina staat in `en/index.html`.

## Blog

De oude blogs van larsvantuin.nl staan in `_posts/`, onder dezelfde adressen als op WordPress. Nieuwe blog: maak in `_posts/` een bestand `JJJJ-MM-DD-korte-titel.html` (of `.md`) met bovenaan:

```
---
title: "Titel"
---
```

Oude WordPress-pagina's (proefschrift, lezingen, over-lars …) verwijzen via de map `oud/` door naar hun nieuwe plek.

Het pdf-artikel bij "Stop met motiveren!" verschijnt zodra `assets/pdf/tvc-2022-02-12-Lars-v-Tuin.pdf` er staat.
