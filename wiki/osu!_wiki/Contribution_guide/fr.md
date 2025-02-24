---
outdated: true
outdated_since: 21c7550caa7a994c12617cc08e94cb46d04ff3dd
---

# Guide de contribution au osu! wiki

Merci de votre intérêt à vouloir rendre le osu! wiki meilleur ! Cet article couvre le processus de contribution étape par étape. Si vous êtes familier avec GitHub, n'hésitez pas à suivre le feature-branch workflow pour proposer des changements et passez directement à la section concernant le [self-check](#self-check).

Si vous avez besoin d'astuces ou de conseils à n'importe quelle étape, n'hésitez pas à demander dans le salon de discussion `#osu-wiki` du [serveur Discord osu!dev](/wiki/Community/osu!dev_Discord_server).

## Domaines d'intérêt

Si vous voulez aider, mais ne savez pas par où commencer, consultez [Maintenance du osu! wiki § Routines](/wiki/osu!_wiki/Maintenance#routines) pour obtenir une liste des tâches qui doivent être effectuées régulièrement, et pour savoir comment aider les autres éditeurs du wiki. Pour vous familiariser avec le langage de formatage utilisé sur le wiki, consultez la [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) d'Adam Pritchard.

## Modifier le wiki

*Pour un processus de contribution généralisé, voir [GitHub flow - GitHub Docs](https://docs.github.com/en/get-started/quickstart/github-flow)*

Les articles du osu! wiki sont stockés sur [GitHub][osu_wiki]. Pour contribuer, procédez comme suit :

0. [Créez](https://github.com/signup) un compte GitHub.
1. Ouvrez le dépôt [`ppy/osu-wiki`][osu_wiki] et cliquez sur `Fork` dans le coin supérieur droit pour faire une copie contrôlée du wiki. Pour revenir à votre fork, allez sur [`ppy/osu-wiki`][osu_wiki] et cliquez à nouveau sur `Fork`.

  - Si vous avez créé un fork il y a quelque temps, synchronisez-le conformément aux [Bonnes pratiques § Synchronisation d'un fork](/wiki/osu!_wiki/Contribution_guide/Best_practices#synchronisation-d'un-fork).

2. Lisez [Bonnes pratiques § Faire des modifications](/wiki/osu!_wiki/Contribution_guide/Best_practices#faire-des-modifications) et effectuez les modifications nécessaires. Bien que vous soyez libre d'utiliser l'application de votre choix, le osu!wiki contient des instructions détaillées sur deux outils :

  - [Éditeur web de GitHub](/wiki/osu!_wiki/Contribution_guide/GitHub_web-based_editor) (en ligne, aucune installation requise).
  - [GitHub Desktop](/wiki/osu!_wiki/Contribution_guide/GitHub_Desktop) (hors ligne, offre plus de contrôle).

## Self-check

Lorsque vous avez terminé la review, prenez le temps de relire votre travail. Passez en revue la liste de contrôle rapide suivante :

- **Le ton de la prestation** : les articles du osu! wiki, à de rares exceptions près, doivent être rédigés dans un registre neutre.
- **Le style et la grammaire** : les articles doivent être clairs, compréhensibles et ne demander aucun effort mental important au lecteur. Soyez cohérent et évitez les phrases trop compliquées ou abruptes. Utilisez des éditeurs dotés de correcteurs orthographiques intégrés, tels que [Google Docs](https://docs.google.com), pour mettre en évidence les fautes de frappe et les erreurs grammaticales ou syntaxiques.
- **[La parité de contenu](/wiki/Article_styling_criteria/Formatting#parité-de-contenu)** : les traductions doivent contenir les mêmes informations que les articles originaux (des différences de ponctuation, de formulation ou de formatage sont évidemment attendues). Au lieu de modifier le contenu de la traduction, [ouvrez un issue](https://github.com/ppy/osu-wiki/issues/new) ou une demande de modification supplémentaire pour l'original si vous estimez qu'il est incomplet, inexact ou obsolète.
- **Structure et mise en forme** : prévisualisez votre article à l'aide d'un outil tel que [jbt's Markdown Editor](https://jbt.github.io/markdown-editor/) pour vous assurer qu'il se présente exactement comme vous le souhaitiez.
- **Toutes les images et autres fichiers non textuels** doivent être [inférieurs à 1 mégaoctet](/wiki/Article_styling_criteria/Formatting#taille-du-fichier). **Les captures d'écran** doivent utiliser le skin d'osu! par défaut et les [paramètres spécifiques](/wiki/Article_styling_criteria/Formatting#captures-d'écran-de-gameplay), y compris les dimensions maximales de 1280×720.

Pour une liste complète des règles, lisez les [critères de mise en forme des articles](/wiki/Article_styling_criteria).

## Pull request

Une fois que les modifications ont été vérifiées, validées et push vers votre fork, vous devez les proposer aux maintainers du wiki en ouvrant une pull request :

1. Dans **votre fork** du osu! wiki, trouvez la liste déroulante avec d'écrit `master↓`, et sélectionnez la branche avec vos changements.
2. Cliquez sur le bouton `Contribute↓` et sélectionnez `Open pull request`.
3. Remplissez les détails selon les [Bonnes pratiques § Ouvrir une pull request](/wiki/osu!_wiki/Contribution_guide/Best_practices#ouvrir-une-pull-request) et cliquez sur `Create pull request`.

## Review

Toutes les modifications apportées au osu! wiki sont modérées. Pendant cette étape, les autres collaborateurs signalent les erreurs possibles et les moyens de les corriger, soit sous forme libre, soit en suggérant des modifications directes de la pull request Comme pour toute autre review, vous devez répondre aux commentaires en appliquant les suggestions ou en expliquant pourquoi vous préférez garder les choses telles quelles.

Si personne ne s'est manifesté après quelques jours, essayez ce qui suit :

- Assurez-vous d'avoir résolu toutes les suggestions - les gens peuvent attendre vos réponses.
- Demandez aux autres rédacteurs du osu! wiki sur le [serveur Discord osu!dev](/wiki/Community/osu!dev_Discord_server) (canal `#osu-wiki`) ou dans les commentaires de GitHub.
- Pour obtenir de l'aide pour la traduction, consultez quelques pull requests fusionnées pour votre langue et contactez leurs réviseurs et/ou auteurs ([exemple de requête GitHub](https://github.com/ppy/osu-wiki/pulls?q=is%3Apr+is%3Amerged+%5BFR%5D+)).
- Demandez à vos amis d'y jeter un coup d'œil !

En plus d'un processus de révision manuelle, le dépôt osu! wiki possède [un ensemble de vérifications automatisées](/wiki/osu!_wiki/Maintenance#ci-checks), qui garantissent que vos modifications respectent le style commun du wiki et sont exemptes d'erreurs de formatage. Pour voir leur statut, ouvrez l'onglet `Actions` de votre pull request et suivez les messages de diagnostic sous les erreurs, s'il y en a.

## Merge

Vos modifications seront éventuellement vérifiées par l'un des [wiki maintainers](/wiki/osu!_wiki/Maintenance/List_of_maintainers), généralement après avoir été review par d'autres collaborateurs. Si rien ne se passe après un laps de temps raisonnable, demandez dans les commentaires de la pull request, ou dans le canal `#osu-wiki` du [serveur Discord osu!dev](/wiki/Community/osu!dev_Discord_server). Vos modifications apparaîtront sur le osu! wiki peu de temps après la fusion (dans de rares cas, cela peut prendre jusqu'à cinq heures).

[osu_wiki]: https://github.com/ppy/osu-wiki
