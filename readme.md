# Utilisation de variable d'environnement

## Configurer les Secrets et variable
[La définition de l'action](./.github/workflows/env-var.yaml) a besoin de configurer 2 choses


* Une variable `ENV_CONTEXT_VAR`
* Un secret `SECRET_VAR`

1) Pour cela il faut aller dans github sur votre projet
2) Dans le menu `Settings`
3) Menu de gauche `Secrets and variables`
4) Puis dans `Actions`
5) Vous avez alors accès à l'onglet `Secrets` et l'onglet `Variables`, ajouter les 2 nécessaires avec les valeurs que vous souhaitez.


## Comment exécuter ?

Il suffit d'activer le trigger de l'action à savoir un "push". 

Cependant pour push il faut pouvoir avoir un commit.

Vous connaissez peut être les "dummy commit" qui sont des modifications mineurs, un espace par ci, juste pour pouvoir créer un commit.


Mais ici, on fait les choses proprement pourquoi faire un faux commit quand on peut faire un commit vide ?!

```bash
git commit --allow-empty -m "Commit totalement vide !"
```

Il suffit alors de push tout ça vers Github

```bash
git push
```

Il reste à aller voir l'interface de Github pour observer le résultat dans les actions.

## Formation sur GitHub Actions

Ce projet fait partit d'une formation sur l'utilisation de GitHub Actions et découvrir comment automatiser vos intégrations continues sur Udemy : [Automatiser tout sur vos projets avec Github Actions](https://www.udemy.com/course/automatiser-tout-sur-vos-projets-avec-github-actions/?referralCode=268A353A1CAE10611EBD).

N'hésitez pas à explorer les fonctionnalités de Chromatic et de Storybook pour améliorer la qualité et la robustesse de vos composants d'interface utilisateur. Happy coding! 🚀