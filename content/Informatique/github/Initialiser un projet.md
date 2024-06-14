# Coment initialiser un projet github

> [!INFO]
> Quand je parle d'initialiser un projet, je parle de créer une repo en local pour ensuite l'envoyer sur Github ou Gitlab

- Tout d'abord on se rend dans le dossier dossier cible puis on l'initialise :
```
cd monprojet/
git init
```

- Ensuite on doit ajouter les fichiers à la repo puis on commit le tout :
```
git add trucmuch/*
git commit -m "J'ai ajouté le contenu de trucmuch"
```

- On lie ensuite la repo distante à la locale :
```
git remote add origin git@github.com:Timtonix/cartes.git
git remote -v
```

- Puis on push
```
git push
```

