# Test Gitflow 2

Voici comment on utilise Gitflow avec les commandes `git` et `git flow`.

1. Créez un nouveau projet Xcode et initialisez un dépôt Git local en utilisant la commande `git init`. ✅
2. Configurez Gitflow en utilisant la commande `git flow init`. Utilisez les options par défaut pour le nom de la branche principale (develop) et le préfixe des branches de fonctionnalités (feature/). ✅
3. Créez une nouvelle branche de fonctionnalité en utilisant la commande `git flow feature start <nom_de_la_fonctionnalité>`. Par exemple, `git flow feature start player` pour créer une branche de fonctionnalité pour le lecteur de média. ✅
4. Ajoutez et commitez vos modifications sur la branche de fonctionnalité. Par exemple, vous pouvez ajouter une vue de lecteur de média à votre application. ✅
5. Une fois que vous avez terminé de travailler sur la fonctionnalité, fusionnez-la dans la branche develop en utilisant la commande `git flow feature finish <nom_de_la_fonctionnalité>`. Cela va fusionner votre branche de fonctionnalité dans la branche develop et supprimer la branche de fonctionnalité. ✅
6. Ajoutez une autre fonctionnalité à votre application en créant une nouvelle branche de fonctionnalité en utilisant la commande git flow feature start <nom_de_la_fonctionnalité>. Par exemple, git flow feature start playlist pour créer une branche de fonctionnalité pour la gestion des listes de lecture.
7. Ajoutez et commitez vos modifications sur la branche de fonctionnalité. Par exemple, vous pouvez ajouter une vue pour gérer les listes de lecture.
8. Pendant que vous travaillez sur cette fonctionnalité, vous réalisez qu'il y a une erreur sur la branche develop. Vous pouvez créer une branche de correction en utilisant la commande git flow hotfix start <nom_de_la_correction> et corriger l'erreur sur cette branche.
9. Une fois que vous avez terminé la correction, fusionnez-la dans les branches develop et master en utilisant la commande git flow hotfix finish <nom_de_la_correction>. Cela va fusionner votre correction dans les branches develop et master et supprimer la branche de correction.
10. Une fois que vous avez terminé de travailler sur la fonctionnalité de gestion de listes de lecture, fusionnez-la dans la branche develop en utilisant la commande git flow feature finish <nom_de_la_fonctionnalité>.
11. Enfin, publiez votre projet sur un dépôt Git distant en utilisant la commande git remote add origin <url_du_dépôt> pour ajouter le dépôt distant, puis git push -u origin develop pour pousser la branche develop vers le dépôt distant.