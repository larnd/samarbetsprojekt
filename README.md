# Samarbetsprojekt med Collaborators
Projekt där vi övar på att samarbeta med hjälp av Git. 

Lathund: https://www.git-tower.com/blog/git-cheat-sheet/

Förutsättningar: 
 1. Du har ett privat konto på https://github.com
 2. Git installerat på datorn https://git-scm.com/downloads
 3. Ditt användarnamn på Github är tillagd som "collaborator" till projektet *https://github.com/larnd/samarbetsprojekt.git*
  
Läs mer: https://help.github.com/en/github/collaborating-with-issues-and-pull-requests 

## Klona samarbetsprojektet

1. Klona förvaret (repository) till en mapp på din hårddisk *git clone https://github.com/larnd/samarbetsprojekt.git*

## Skapa en gren på din dator (lokalt repo)

1. Skapa en gren (branch) i projektet: *git branch <namn på gren>*. I detta samarbetsprojekt döper du grenen till ditt förnamn.
2. Gör den nya grenen till den aktiv a: *git checkout <namn på gren>*.

## Gör ändringar i lokal gren

1. Kontrollera att rätt gren är aktiv: *git branch*. Om inte skriv *git checkout* och namnet på den gren du ska redigera.
2. Ändringar: 
  a/ Skapa en ny HTML-fil och spara den med ditt förnamn som filnamn. (T.ex. om jag heter Henrik ska filen heta 'henrik.html').
  b/ Lägg till en länk i index.html till din fil du just skapade.
3. Förbered för kommit: *git add .* (Kontrollera med *git status* före och efter).
4. Kommitta: *git commit -m "Lagt till HTML-fil"*. (Ändringarna är nu tillagda till ditt *lokala* repo)

## Lägg till grenen på Github (fjärr-repo)
1. Lägg till din lokala gren (local branch) till fjärrförvaret (remote repository): *git push --set-upstream origin <namn på gren>*.
2. I fortsättningen behöver du bara skriva *git pull* (för att "dra ned" uppdateringar) och *git push* (för att uppdatera fjärr-repot med dina ändringar).

Arbetsgång när grenen är tillagd: *Gör ändringar* --> *git add .* --> *git commit -m "Uppdaterat filer"* --> *git pull* --> *git push*

## Skapa förfrågan om att lägga till grenen till huvudprojekt (*pull request*)

1. Under fliken "<> Code" finns två knappar. Med den första (*Branch: <namn på gren>*) väljer du den gren som innehåller förändringarna.
2. Klicka på den andra knappen "*New pull request*"
3. Du blir ombedd att skriva en titel och förklaring på förändringarna.
4. Klicka sedan på den gröna knappen "*Create pull request*".
5. Nu kan deltagarna i projektet se och diskutera dina föreslagna förändringar.

## Slå ihop grenen med huvudprojektet (*merge*)

1. Fliken "Pull request" har nu en liten siffra som har ökat med ett. Klicka på fliken så visas alla öppna förfrågningar.
2. Nedanför diskussionstråden finns en grön knapp "*Merge pull request*". Klicka på knappen för att slå samman förändringen i grenen med huvudgrenen.
3. Innehållet i grenen är nu detsamma som i huvudgrenen och det visas en lila knapp. Grenen kan därför raderas genom att klicka på den röda "papperskorgen" under fliken *<>Code - branches*. Radera din gren.
