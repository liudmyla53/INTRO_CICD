# Demo - Introduction au Github Action

## Mise en lpace
-Initialiser le repo git
 -Pousser le repo sur Github
 -Créer une action `.github>workflows>first-action.yaml`

 ## Syntaxe de base
 Fichier `yaml` -> Fichier structuré par tabulation

 ```yaml
 # Nom du workflow
 name: exampe_syntaxe
 # Triggers
on:
workflow_dispatch:
push : [main]

 # Travaux à réaliser
 jobs:
   job_name:
     ...

 ```

 ### Triggers
 Ensemble des events écoutés
 - Manuellement -> Bouton pour lancer le tratement
 - Push d'un branche
 - Etc...

Liste des events [ici]()

### Travaux à réaliser
L'ensemble d'action à faire
- Runner ->Machine virtuel "pretée" par github
- Acrion à faire :
  - Script(Synatxe qui depend du terminal!!!)
  - Utilisation d'action _(ça sera vue plus tard)