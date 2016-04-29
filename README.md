Git training
------------

## Transfert des modifications

```
Repertoire      Index         HEAD
    |             |             |
    |             |             |     Gestion des modifications
    |             |             |
    o------------->             |         git add
    |             o------------->         git commit
    o--------------------------->         git commit -a
    |             <-------------o         git reset -- fichiers
    <-------------o             |         git checkout -- fichiers
    <---------------------------o         git checkout HEAD -- fichiers
    |             |             |
    |             |             |     Analyse des différences
    |             |             |
    <-------------o             |         git diff
    |             <-------------o         git diff --cached
    <---------------------------o         git diff HEAD
```
    
## Commandes de base
### Commit
- add [-p]
- rm [--cached] [–r]
- commit [-a] [–m] [--amend]
- stash [-u]  

### Communication avec les remote
- git pull [--rebase]
- git push [-u]  

### Manipulation de l'historique
- git branch [--contains]
- git diff
- git reset
- git checkout [-b]
- git rebase [-i]
- git merge [–-no-ff] [--only-ff]  

### Snapshot de l'historique
- status
- git log
- git reflog  

### Debuggage
- git blame [--someone-else]
- git bisect

## A quoi devrait ressembler un commit
```
<type>: <sujet>

<corps>

<footer>
```

- **type**: feat, fix, docs, style, refactor, test, perf
- **sujet**: description courte du changement
- **corps**: description longue du changement, doit inclure le contexte initial, le but et la démarche
- **footer**: informations importantes (breaking change, relation avec d'autres commits/PR)

## La gestion de conflits
