# Initializace repozitáře pomocí Visual Studio Code

## Vytvoření serverového repozitáře

Otevřete [GitHub.com](https://github.com/) (a přihlaste se, pokud nejste přihlášeni)

Pomocí tlačítka New vytvoříme nový repozitář

![NewButtonGitHub](Media/RepoCreation.png) 

Repozitář pojmenujeme dle naší libosti

![GitHubRepoNaming](Media/RepoNaming.png) 

![GitHubBareRepo](Media/RepoRepos.png) 

## Initializace repozitáře ve VSC

Než začneme potřebujeme mít vytvořenou složku, ze které vytvoříme repozitář.

### Initializace

Otevřeme složku ve VSC.

![VSC-open](Media/VscOpen.png)

Po přepnutí do náhledu pro GIT můžeme initializovat repozitář.

![VSC-repos](Media/VscInit.png)

Vybereme složku, kde chceme initializovat. (Nabízí se jako první současná složka)

![VSC-repoInit](Media/VscInitRepo.png)

### Přidání remote

Pro přidání *remote* potřebujeme zobrazit paletu příkazů.

![VSC-remote1](Media/VscRemote1.png)

Pomocí vyhledávání nalezneme příkaz pro přidání *remote* (stačí zadat remote)

![VSC-remote2](Media/VscRemote2.png)

Nyní zadáme jméno remote (pro výchozí remote je typické jméno *origin*)

![VSC-remote3](Media/VscRemote3.png)

Vložíme URL, které získáme z GitHub

![VSC-remote4](Media/VscRemote4.png)

### Přidání commitu a jeho publikace

Pod *Changes* vydíme soubory, které jsou upravené, ale nejsou přidané do **stage**. tyto soubory přidáme pomocí malého plus, které se zobrazí, když na soubor najedeme myší.

![VSC-stage](Media/VscStage.png)

Soubory ve **stage** commitujeme pomocí fajifky. Je nutné zadat commit message.

![VSC-commit](Media/VscCommit.png)

Pomocí ikonky vedle jména větve v dolní liště VSC provedeme synchronizaci se serverovým remote.

![VSC-publish](Media/VscPublish.png)