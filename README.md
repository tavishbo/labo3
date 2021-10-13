# LaboReeks Git
## **Labo 3**

In dit derde labo gaan we werken met branches.

We zullen ook hier de lokale wijzigingen gaan koppelen aan een remote git repository (GitHub). 
Alles wat gevraagd wordt dien je lokaal toe te voegen en vervolgens via de nodige commando's ook in de online repository te brengen.

**Let er in het bijzonder op dat alle aangemaakte branches juist gesynct worden met de remote.**

#### **Aanvullende toets op Leho**
Na het afwerken van dit labo heb je op Leho een aanvullende toets met betrekking tot het labo en de leerstof gekoppeld aan het labo.
Je kan/mag de aanvullende toets steeds afleggen gebruik makend van alle bronnen (cursusmateriaal, labo, online bronnen, ...)

### **Labo 3:** *Takenlijst*
- [ ] Open de Git Bash Console op de locatie waar je dit labo wil gaan clonen. Dit kan via een rechtermuisklik op de locatie in kwestie en vervolgens de keuze **Git Bash Here** te selecteren.
>**Tip!** Indien deze optie niet beschikbaar is dan heb je een stap in de aanbevolen installatie overgeslaan.

- [ ] Zorg ervoor dat de startsituatie *(deze repository)* van het labo op jouw pc **gecloned** wordt. Maak hiervoor gebruik van het passende git commando. 

- [ ]  Ga **na het clonen** via de console naar de gecloonde repository. Dit kan/mag je uiteraard ook doen door de nieuwe aangemaakt folder aan te klikken en hier opnieuw een Git Bash console te openen via de **Git Bash Here** optie.
>**Tip!** Controleer voor je verder werkte of je al dan niet in de juiste git repository zit! Je kan dit snel visueel vaststellen in je console.

### Deel 1: aan de slag met **branches**

- [ ] Voer een git commando uit dat het overzicht toont van alle lokale branches.
      Dit zou er momenteel slechts 1 mogen zijn: de master-branch.

- [ ] Maak in je lokale repository nu een nieuwe branch aan.
      Deze nieuwe branch geef je als naam **dev** mee. Ga vervolgens naar deze nieuwe aangemaakte branch. 
>**Tip!** Denk er aan voor je naar de volgende stap doorgaat om zeker te controleren dat je **niet** langer op de **master** branch aan het werk bent!

- [ ] Zorg met een passend git commando dat je remote repository (GitHub) deze **dev** branch, alsook de inhoud ervan, ook binnenkrijgt en tevens linkt aan je lokale branch. 

- [ ] Vanuit je **dev branch** maak je vervolgens **2 feature branches** aan. Deze branches geef je volgende namen:
    -  **feature/home-page**
    -  **feature/contact-form**
>**Tip!** Zorg er zeker voor dat je je op de **dev** branch bevindt voor je aan de slag gaat met het aanmaken van nieuwe branches.

- [ ] Switch een voor een naar deze nieuwe branches en zorg met een passend git commando dat je remote repository *(GitHub)* deze branches, alsook de inhoud ervan, ook binnenkrijgt en tevens linkt aan je lokale branches. 

- [ ] Ga naar de **feature/home-page** branch.
      Maak een bestand `index.html` aan en voorzie hierin een geldige HTML5 pagina met inhoud naar keuze, bv. "Welkom op deze website".

- [ ] Zorg ervoor dat het nieuwe bestand `index.html` opgenomen wordt in je lokale git repo.
      Synchroniseer hierna je lokale repository met je remote repository.
>**Tip!** Denk aan de conventies rondom naamgeving van de commit messages!

- [ ] Ga naar de **feature/contact-form** branch en maak een nieuw bestand `contact.html` aan.
      Voorzie in dit bestand een geldige HTML5 pagina met inhoud naar keuze, bv. 

```
    <a href="mailto:someone@example.com">Contacteer ons</a>
```

- [ ] Zorg ook hier dat de nieuwe file `contact.html` opgenomen wordt in git.
      Synchroniseer hierna je lokale repository met je remote repository.
>**Tip!** Denk aan de conventies rondom naamgeving van de commit messages!

- [ ] Ga naar de **dev** branch en voer onderstaande commandos uit:
```
clear
git branch
git log --oneline
```

- [ ] Neem een screenshot van het resultaat. Deze screenshot plaats je in de **lokale** Screenshots folder. *(Op jouw PC/laptop dus!)* Geef deze screenshot de naam **deel1** (met extensie naar keuze).

- [ ] Maak gebruik van passende git commando's om alle lokale bestanden te commiten naar git. **Synchroniseer** vervolgens je lokale repository met de online repository op GitHub.
>**Tip!** Denk aan de conventies rondom naamgeving van de commit messages!

### Deel 2: afronden van feature branch

- [ ] Merge vervolgens de wijzigingen die je in de **feature/home-page** aangemaakt hebt in de **dev** branch.
- [ ] Voer opnieuw onderstaande commando's uit:
```
clear
git branch
git log --oneline
```

- [ ] Neem een screenshot van het resultaat. Deze screenshot plaats je in de **lokale** Screenshots folder. *(Op jouw PC/laptop dus!)* Geef deze screenshot de naam **deel2A** (met extensie naar keuze).

- [ ] Maak gebruik van passende git commando's om alle lokale bestanden te commiten naar git. **Synchroniseer** vervolgens je lokale repository met de online repository op GitHub.
>**Tip!** Denk aan de conventies rondom naamgeving van de commit messages!

- [ ] Zorg er nu voor dat de branch **feature/home-page** verwijderd wordt, zowel **lokaal** als **remote**, m.b.v. de nodige git commando's.
- [ ] Voer opnieuw onderstaande commando's uit:
```
clear
git branch
git log --oneline
```

- [ ] Neem een screenshot van het resultaat. Deze screenshot plaats je in de **lokale** Screenshots folder. *(Op jouw PC/laptop dus!)* Geef deze screenshot de naam **deel2B** (met extensie naar keuze).

- [ ] Maak gebruik van passende git commando's om alle lokale bestanden te commiten naar git. **Synchroniseer** vervolgens je lokale repository met de online repository op GitHub.
>**Tip!** Denk aan de conventies rondom naamgeving van de commit messages!

### Deel 3: vervolg contact feature

We willen nu graag een link leggen van de home page naar de contactpagina,
maar de home page is nog niet beschikbaar op de bijhorende feature branch **feature/contact-form**.
De home page feature is echter wel degelijk reeds afgerond en aanwezig op **dev**.
We zullen nu dus eerst onze contact feature up to date brengen met de meest recente versie van **dev**.

- [ ] Keer terug naar de branch **feature/contact-form**.
- [ ] Merge de nieuwe versie van **dev** in **feature/contact-form**.
      Controleer dat de home page `index.html` nu ook beschikbaar is op deze branch.

- [ ] Open het bestand `index.html` in een editor naar keuze en voeg onderaan een link toe die verwijst naar de contactpagina, bv.
```
<a href="contact.html">Contactpagina</a>
```
- [ ] Open de home page even in je browser om te testen dat de link goed werkt.
- [ ] Gebruik de gepaste git commando's om je wijziging aan `index.html` op te nemen in de lokale git repo, en te syncen met de remote.
>**Tip!** Denk aan de conventies rondom naamgeving van de commit messages!

- [ ] Voer opnieuw onderstaande commando's uit:
```
clear
git branch
git log --oneline
```

- [ ] Neem een screenshot van het resultaat. Deze screenshot plaats je in de **lokale** Screenshots folder. *(Op jouw PC/laptop dus!)* Geef deze screenshot de naam **deel3** (met extensie naar keuze).

- [ ] Maak gebruik van passende git commando's om alle lokale bestanden te commiten naar git. **Synchroniseer** vervolgens je lokale repository met de online repository op GitHub.
>**Tip!** Denk aan de conventies rondom naamgeving van de commit messages!

De contact feature blijft nog even in ontwikkeling (buiten scope van het labo).
We gaan dus de branch **feature/contact-form** nog **NIET** mergen naar **dev** en ook **NIET** verwijderen.

### Afronden labo

- [ ] Ga terug naar de **dev** branch.
- [ ] Na het voltooien van alle taken editeer je deze README.md file.
      **LET OP!** dit doe je opnieuw in je lokale README.md file!
      Plaats alle tasks op voltooid door de markup te wijzigen van [ ] naar [x].
>**Tip!** Je kan hier gerust VS Code gaan gebruiken. Deze heeft ook een preview mode om met markdown aan de slag te gaan.

- [ ] Maak gebruik van git commando's om vervolgens deze wijzigingen aan je lokale git repository toe te voegen.
      Sync de lokale **dev** branch vervolgens naar de remote.

- [ ] Ga naar de **master** branch en zorg ervoor dat deze branch geüpdatet wordt met de huidige inhoud van de **dev** branch.

- [ ] Zorg ervoor dat je lokale repository nu ook nog een laatste keer gesynchroniseerd wordt naar deze GitHub repository toe.
