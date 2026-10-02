# TDLOG — Tutoriel & Guide de Démarrage

Ce didacticiel a pour objectif de vous accompagner pas à pas dans la prise en main de l'environnement de développement et dans la maîtrise du workflow Git/GitHub.


## 📺 Tutoriels Vidéo

1. [créer un espace codespace (~1 minute)](https://drive.google.com/file/d/1o_lGNxPFrypzroC6pZV-D4gmFH8v-9um/view?usp=sharing)

2. **Comprendre le Git Workflow** *(~9 minutes)*
Découvrez les bonnes pratiques pour commiter vos modifications, créer une branche, pousser votre travail et ouvrir une *Pull Request* sur un autre repo distant.  
   👉 [Visionner la vidéo (Git Workflow)](https://drive.google.com/file/d/1fEejIHEDTmlyc100Pcxctgpe8_V9jWnv/view?usp=sharing)

## Git commands

### Git commit

```
# Vérifier l'état de vos fichiers modifiés
git status

# Les fichiers à committer sont explicites. Ajouter les fichiers modifiés au suivi (staging area)
git add <file-name>
# Ou pour ajouter tous les fichiers modifiés :
git add .

# Enregistrer les modifications avec un message clair
git commit -m "feat: description claire des modifications apportées"
```

### Git push

```
# Voir la liste des repos distants
git remote -v

# Envoyer la branche locale ( feature/${nom_branche_locale} ) sur le dépôt distant (GitHub)
git push origin feature/${nom_branche_locale}

# Utile si vous avez oublié de créer une branche
# Envoyer la branche locale ( feature/${nom_branche_actuelle} ) sur le dépôt distant (GitHub) et la renommer ( feature/${nom_sur_le_repo_distant} )
git push origin feature/${nom_branche_actuelle}:feature/${nom_sur_le_repo_distant}
```

### Git branch

```
# Créer une nouvelle branche et switcher sur cette branche
git checkout -b feature/${nouvelle_branche}
```
