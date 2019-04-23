# Initializace repozitáře pomocí příkazové řádky

## Vytvoření serverového repozitáře

Otevřete [GitHub.com](https://github.com/) (a přihlaste se, pokud nejste přihlášeni)

Pomocí tlačítka New vytvoříme nový repozitář

![NewButtonGitHub](Media/RepoCreation.png) 

Repozitář pojmenujeme dle naší libosti

![GitHubRepoNaming](Media/RepoNaming.png) 

![GitHubBareRepo](Media/RepoRepos.png) 

## Initializace repositáře ve VSC

Než začneme potřebujeme mít vytvořenou složku, ze které vytvoříme repozitář.

Návod na initializaci dává k dispozici i GitHub, když založíme nový repozitář.

Pro úspěšný push potřebujeme mít alespoň 1 vytvořený, neprázdný soubor (nejčastěji je to README.md)

### Initializace

```git init```

```git remote add origin git@github.com:KaschiCZE/test-repo.git```

```git add .```

```git commmit -m "init commit"```

```git push origin master```

![bash-repoInit](Media/repocmdcreation.PNG)
