# Git CheatSheet

## Inicializace nového repozitáře

```git init```
 - inicializuje repozitář ve složce, ve které se nacházíme

```git remote add origin``` *URL webového repozitáře*
 - přidá výchozí remote pro repozitář, porti kterému se budeme synchronizovat
   - *URL_webového_repozitáře* získáme z GitHub

```git add .```
 - přidá všechny soubory ve složce do *stage*

```git commmit -m "init commit"```
 - vytvoří commit se zprávou *init commit*

```git push origin master```
 - nahraje commity na remote s názvem *origin* do větve *master*

## Klonování repozitáře

```git clone``` *URL_webového_repozitáře*
 - naklonuje do současného místa repozitář z *URL_webového_repozitáře*

## Lokální úpravy + jejich stage + přidání do commitu

```git status```
 - zobrazí stav repozitáře (změny, nové soubory, odstraněné soubory)

```git add .```
 - přidá všechny změněné soubory v repozitáři do stage

```git add``` *cesty k souborům*
 - přidá všechny změněné soubory v repozitáři do stage

```git commit -m "```*zpráva popisující úpravy v commitu*```"```

## Publikace úprav
```git push```
 - nahraje commity do aktuální větve

## Tagování verzí a jejich synchronizace s webem
```git tag``` *jmeno_tagu* ```-m "``` *zpráva popisující verzi*```"```
 - vytvoří tag se jménem *jmeno_tagu*
 - parametr ```-m``` je nepovinný

```git push --tag```
 - nahraje poslední tag do online repozitáře

```git push --tags```
 - v případě, že jesště nebyly nikdy tagy synchronizovány s online repozitářem, nahraje všechny tagy

## Získání úprav z repozitáře
```git fetch```
 - podívá se do webové verze repozitáře, a zjistí úpravy, stáhne je, ale neaplikuje je

```git pull```
 - stáhne změny a aplikuje je (může způsobit konflikty)
   - na pozadí provádí příkazy ```fetch``` a ```merge```

## Větvení
```git branch -v```
 - vypíše všechny větve v repozitáři

```git branch``` *jméno_větve* ```[```*revize*```]```
 - vytvoří novou větev se jménem *jméno_větve*
 - možnost nepovinného parametru revize, který značí commit, ze kterého se větev vytvoří
   -  výchozí revize je ```HEAD```

```git checkout``` *jmeno_vetve*
 - přepne se do větve *jmeno_vetve* (tato větev musí existovat)

```git checkout -b``` *jméno_větve* ```[```*revize*```]```
 - vytvoří novou větev se jménem *jmeno_vetve* z revize kterou můžeme specifikovat pomocí *revize* (výchozí parametr je ```HEAD```) a rovnou do ní přepne

## Mergování
```git merge``` *jmeno_slucovane_vetve*
 - sloučí *jmeno_slucovane_vetve* do větve, ve které se nyní nacházíme
 - ```--no-ff``` --> vezme pouze poslední commit ve *jmeno_slucovane_vetve* (nepřenáší kompletní historii commitů)
   - používá se například při mergování do *master* větve, aby se zaručila spustitelnost