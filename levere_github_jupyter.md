{% include navbar_open.html %}

# Slik leverer du arbeidskrav på github fra jupyter notebook

Vi vil her vise hvordan du lager et githubrepositorie der du skal levere dine arbeidskrav.

## Lag et nytt git-repositorie til innleveringene dine

Del 1-3 kan du hoppe over dersom du har gjort det før.

1. Logg på din githubkonto
2. Logg på `jupyter.uit.no`, og åpne ny Terminal (+), og naviger dit du vil ha repositoriet på jupyter med `cd <mappenavn>` (se [tips og triks.md fra SOK-1003](https://github.com/uit-sok-1003-h21/notebooks/blob/main/tips_og_triks.md) for hvordan du navigerer i Terminal.) 
3. Konfigurer git med e-posten til kontoen og ditt brukernavn (bytt ut klammeparentesene med e-posten og brukernavnet til githubkontoen):
```
git config --global user.email "<e-post>"
git config --global user.name "<brukernavn>"
```

4. Gå til **Repositories**, trykk **New**, gi repositoriet navnet <sok-1005-v22> og velg **Private** eller **Public**. Merk at < og > skal ikke være med i navnet, og du skal benytte små bokstaver.
5. Hold denne fanen åpen, for du skal bruke html-adressen til denne siden.
6. Sørg for at du har et token. Gå eventuelt til [https://github.com/settings/tokens/new](https://github.com/settings/tokens/new) for å generere nytt token. *Hold fanen åpen for å ha tokenet tilgjengelig.* Under "Select scopes", huk av for "repo".
7. I jupyter terminal, kjør `git clone https://<token>@github.com/<sti>` der \<token\> er tokenet er det du fikk i 6. og \<sti\> er det som kommer etter **github.com/**  i html-adressen i 5.

Du kan nå redigere repositoriet ditt
 
## Gi tilgang til faglærer/seminarleder
Du må også gi oss tilgang, slik at vi kan se repositoriet og arbeidet ditt. Det gjør du slik:

Når du er på nettsiden til repositoriet, gåt til "Settings", og så "Manage access", og legg til "espensirnes" og "oysteinm"
 
## Dytte repositoriet til github:
Dette gjør du ETTER at du har lagret en jupyter-fil i mappen til det klonede repositoriet. Sørg for at du lagrer i riktig mappe!

1. Naviger til repositoriemappen i Terminal (se [tips og triks.md](https://github.com/uit-sok-1003-h21/notebooks/blob/main/tips_og_triks.md) for hvordan du navigerer i Terminal.) 
2. Kjør i Terminal:
```
git add .
git commit -m "Første commit til repositoriet"
git push 
```
Om du gjør endringer, og skal oppdatere repositoriet senere, kjører du samme prosedyre som over, men du kan endre teksten "Første commit til repositoriet" til noe som beskriver oppdateringen.  

 
