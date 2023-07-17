# Git Masterclass : exercice avec GitHub

Bievenue dans ce projet de démonstration de Git et GitHub.

Voici le travail que vous devez mener :

- créez un ticket `Ajout du fichier demo-<VOTRE-NOM>.sh`.
- clonez localement ce projet.
- créez une branche `feat-<NUMERO-TICKET>`.
- Premier commit : créez le fichier `demo-<VOTRE-NOM>.sh` avec le contenu ci-après. Faites en sorte que ce fichier soit exécutable (`chmod +x demo-<VOTRE-NOM>.sh`)
- Second commit : créez le fichier `test-<VOTRE-NOM>.sh` avec le contenu ci-après dont vous aurez changé le contenu `./demo-<VOTRE-NOM>.sh`. Faites en sorte que ce fichier soit exécutable (`chmod +x test-<VOTRE-NOM>.sh`)
- Partagez sur le serveur.
- Créez une demande de fusion pour votre branche (_Merge Request_).

La demande de fusion va échouer car l’intégration continue lance le test qui pointe une erreur dans le fichier `demo-<VOTRE-NOM>.sh`.

- Corrigez-le en remplaçant `KO` par `OK`. Créez le commit associé et partagez.
- Validez la fusion.
- Récupérez localement les mises à jour du projet et vérifiez l’historique.

## Contenu du fichier `demo-<VOTRE-NOM>.sh`

```bash
#! /bin/bash

echo KO
```

## Contenu du fichier `test-<VOTRE-NOM>.sh`

```bash
#! /bin/bash

# Si exécuter `demo-<VOTRE-NOM>.sh` affiche OK, quitter avec code de sortie 0.
# (Sinon quitter en non-zéro, ex. 127)
./demo-<VOTRE-NOM>.sh | grep -q OK
```
