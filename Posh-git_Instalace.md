# POZOR TENTO POPIS JE ZATÍM PRACOVNÍ !!!

# Posh-Git - Nadstavba pro PowerShell na zobrazování Git repozitářů a barevných stavů 

## Ruční instalace ==============

Zde je popsáno jak lze instalovat
https://github.com/dahlbyk/posh-git 
https://www.powershellgallery.com/packages/posh-git/0.7.3 

Mě zafungovala až ruční instalace.
Do repozitáře jsem dal podsložku 
### Install/posh-git/ ###
zde jsou zdrojové soubory pro posh-git

Následně stačí při spuštění PowerShellu provést import modulu 
Import-Module "c:\Program Files\WindowsPowerShell\Modules\posh-git\0.7.3\posh-git.psd1"


Pokud toto chci mít automaticky vždy k dispozici, přidám daný import modulu do Profilu
Kde leží profil pro aktuálního uživatele je v proměnné 
$profile.CurrentUserAllHosts

Takto jej mohu modifikovat
notepad $profile.CurrentUserAllHosts
Pokud tam není soubor Profile.ps, stačí jej založit a přidat do něj řádek s importem