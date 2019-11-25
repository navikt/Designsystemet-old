# Alternative tekster (alt-tekster) på nav.no

## Hva er en alt-tekst?

En alt-tekst (kort for alternativ tekst) er en tekst som vises eller leses opp når bildet ikke vises for brukeren. Dette kan være fordi:

-   Bildet ikke ble funnet
-   Brukeren har skrudd av bildenedlasting
-   Brukeren har dårlig internettoppkobling
-   Brukeren bruker en skjermleser (for eksempel blinde)
-   Brukeren bruker en tekst-only browser

Alle meningsbærende bilder skal ha en beskrivende alt-tekst. (Dette er også lovpålagt, se forskrift om universell utforming av IKT, WCAG 1.1.1.). Bilder som er ren pynt skal ha tomt alt-attribut (`alt=""` ). Se alt-tekst-beslutningstre under.

/infoboks!
Hva er et bilde?
Begrepet "bilder2 favner i den her konteksten både fotografier, illustrasjoner, logoer, ikoner, grafer, infografikk og annen type grafikk.
/

/Ekspanderbar panel

Og hva er da title, tooltip, bildetekst og longdesc?

**Title** er informasjonen som ofte vises som  **tooltip**  ved mouse-over i nettleseren. Det er IKKE samme som alt-teksten, og kan ikke brukes istedenfor. Mens beskrivende alt-tekst er lovpålagt, er det frivillig å bruke title.

Noen ulemper med title:
-   Fungerer ikke på mobil og nettbrett.
-   Fungerer dårlig for hjelpemiddelteknologi som skjermlesere. Noen brukere får lest opp både alt-tekst og title, da er det irriterende hvis det er samme tekst. Noen får bare lest opp alt-tekst.
-   Dårlig nettleserstøtte får å få vist tooltipen når man navigerer med tastatur.
- Se gjerne [https://developer.paciellogroup.com/blog/2013/01/using-the-html-title-attribute-updated/](https://developer.paciellogroup.com/blog/2013/01/using-the-html-title-attribute-updated/)

Vi anbefaler å ikke bruke title. Det kan være unntak, for eksempel i verktøylinjer som bare bruker ikoner uten synlig label. Da kan det være til hjelp for seende brukere som ellers kan ha vanskelig å forstå ikonene (bruk helst ikoner med synlig label for å unngå problematikken).

Har du mer utfyllende informasjon til bildet bør den være tilgjengelig for alle brukere. Bruk gjerne  **bildetekst**, altså  **synlig tekst under eller ved siden av bildet** for dette:

![Bilde av tre gamle tretraller med tilhørende alt-tekst og figcapture, se kodeeksempel under](https://trello-attachments.s3.amazonaws.com/5c0146cd37715d284e75a4f3/577x480/cdccaa065cc372ed173dfaedcb843dc0/grafikk_02.png)

```html
<figure>
<img src="[https://uu.difi.no/traller.jpg](https://uu.difi.no/traller.jpg)" alt="Tre gamle tretraller. Foto.">
<figcaption>Gamle tretraller regnes av mange som antikviteter.</figcaption>
</figure>
```

**Longdesc** er en lengre beskrivelse av bildet, for eksempel for komplekse grafer. Den kan enten være på en egen URL, eller til et sted på samme side.

/Slutten av ekspanderbar panel

## Anbefalt prosess

-   Den som skriver innholdet på siden lager alt-teksten
-   Velg etter kontekst om bildet skal ha alt-tekst eller ikke, se beslutningstreet under

## Enkle huskeregler - Skal bildet ha en alt-tekst, og hvis ja, hvilken?

-   "Lek skjermleser": Prøv å lese opp siden som den skulle bli lest for en med skjermleser. Hvis du leser opp alt-tekst på et bilde, får brukeren mer informasjon enn uten å ha alt-tekst på bildet? Slik kan du sjekke om
    -   Bildet tilføyer informasjon
    -   Alt-teksten fungerer i konteksten
-   Hvis bildet/illustrasjon sier det samme som teksten i nærheten, skal alt-teksten være tom (`alt=""`).
-   Bruk alt-bestlutningstreet for å finne ut om/hva slags alt-tekst bildet trenger.
-   Se informasjon under "hvordan skrive alt-tekster" for å se hvordan du kan skrive alt-tekstene.

## Alt-tekst-beslutnings-tre
  
Dette beslutningstreet er basert på [W3Cs alt decision tree](https://www.w3.org/WAI/tutorials/images/decision-tree/):
Treet beskriver hvordan du bruker `alt` til `<img>` -elementet i ulike situasjoner. For noen typer bilder er det alternative tilnærminger, for eksempel å bruke CSS-bakgrunnsbilder for dekorative bilder eller webfonter i stedet for bilder av tekst. I noen tilfeller kan det også være aktuelt å bruke aria-label for å erstatte alt-tekst.

1.  **Er det bilde av tekst, det vil si er teksten del av selve bildet?**
	- **Ja** //OBS! Dette skal unngås, all tekst skal være i HTML//
		- a) ...  **og teksten er også til stede som ekte (HTML-)tekst i nærheten.** → Bruk et tomt <alt>-attributt. Se  [dekorative bilder (engelsk)](https://www.w3.org/WAI/tutorials/images/decorative/#image-with-adjacent-text-alternative)
		- b) ...  **og teksten i bildet er ikke til stede ellers.** → Bruk alt-attributtet til å inkludere teksten til bildet. Se [bilder av tekst (engelsk)](https://www.w3.org/WAI/tutorials/images/textual/)  → eksempel:  ![nav-logo](https://trello-attachments.s3.amazonaws.com/5c0146cd37715d284e75a4f3/100x64/38921ce421f7ff59e717acd2d02d98e5/nav-logo.png)   `alt="NAV-logo"` (så lenge logoen ikke er lenket, eller se lengre ned)
	- **Nei**
		- Fortsett
 2. **Brukes bildet i en lenke eller en knapp, og vil det være vanskelig eller umulig å forstå hva linken eller knappen gjør, hvis bildet ikke var der?**
	 - **Ja**
		 - → Bruk alt-attributtet til å kommunisere lenkemålet eller handlingen som er tatt. Se  [funksjonelle bilder (engelsk)](https://www.w3.org/WAI/tutorials/images/functional/)
→ Eksempel:  
			- ![ID-porten](https://trello-attachments.s3.amazonaws.com/5c0146cd37715d284e75a4f3/380x120/3bdb1f2f3fa5cf8e47fd4659b4493704/id-porten.png)`alt="Logg på med ID-porten/MinID"`
			- ![søkefelt](https://trello-attachments.s3.amazonaws.com/5c0146cd37715d284e75a4f3/547x91/470ee8cf09070ddc83fe8ece87d22222/s%C3%B8kefelt.png)  `alt="søk"`
 -  **Nei**
	 - Fortsett
3. **Tilføyer bildet ekstra informasjon til siden?**
	- **Ja**
		- a) ... og det er en  **enkel grafikk, illustrasjon, ikon eller et fotografi**. → Bruk en kort beskrivelse av bildet på en måte som formidler den informasjonen i `alt`-attributtet. Se  [informative bilder (engelsk)](https://www.w3.org/WAI/tutorials/images/informative/) og Hvordan skrive alt-tekster? (avsnitt lengre nede i teksten) → Eksempel:  ![Skjermdump fra en artikkel fra idebanken med bilde av en person i xxl-genser](https://trello-attachments.s3.amazonaws.com/5c0146cd37715d284e75a4f3/969x788/f39f066e2b33bd47bb1d0009eeea34c2/alt11-idebanken.png)`alt="Kim Daniel Skogstad i en XXL-butikk, kledd i XXL-genser"`  ![Skjermdump fra en dialog om barnehageplass i post-innboksen på DittNAV](https://trello-attachments.s3.amazonaws.com/5c0146cd37715d284e75a4f3/767x750/51c021ca52a4cc14b6112122ce6589c7/alt-meldinger.png) Det er viktig å skjønne hvem som har skrevet hvilken beskjed. Dette kommer ikke tydelig frem av teksten (spesielt det brukeren har skrevet). Brukeren er avhengig av å skjønne knytningen til ikonet. De bør derfor ha alt-tekster: `alt="NAV"` og `alt="bruker"` (alternativt `alt="/navn på bruker/"`)
		- b) ... og det er en  **graf eller kompleks informasjon**. → Bruk alt-tekst som beskriver motivet i bildet OG en tekst med detaljert informasjon om innholdet i motivet. I noen tilfeller er det best å tilby visning som  **tabell**. Se  [komplekse bilder (engelsk)](https://www.w3.org/WAI/tutorials/images/complex/) → Eksempel:  ![grafisk planlegging av foreldrepenger](https://trello-attachments.s3.amazonaws.com/5c0146cd37715d284e75a4f3/667x133/88da7b68ebc87abf347b304c86e3f7c4/alt-9-utsettelse.png) `alt="Tar du for eksempel 2 uker ferie i foreldrepengerperioden, forskyves sluttdatoen med 2 uker. Skjematisk illustrasjon"`![Graf med en svart og en grønn linje som sier noe om antall arbeidsledige og ledige stillinger fra 2017-2018](https://trello-attachments.s3.amazonaws.com/590c618893f382eb61038bae/5c0146cd37715d284e75a4f3/cad9890d44461eb163b601c5e477dc95/alt12-kompleksergraf.png) Eksempel på en graf som alternativ bør kunne vises som tabell. `alt="Oversikt over arbeidsledige og ledige stillinger de siste 13 måneder."`
		- c) ...  **og det viser innhold som sier det samme som ekte (HTML-)tek`st i nærheten.** → Bruk et tomt alt-attributt. Se  [(redundante) funksjonelle bilder (engelsk)](https://www.w3.org/WAI/tutorials/images/functional/#logo-image-within-link-text) → Eksempel:  
			- ![](https://trello-attachments.s3.amazonaws.com/5c0146cd37715d284e75a4f3/964x543/f155931eada35224e5298db4d17e8d6f/alt2-chat.png) Her viser bildet en dame på telefon foran en laptop, som skal vise at man kan ringe eller chatte. Samme informasjon står som ren tekst rett ved siden av bildet ("Ring eller chat med oss om økonomi"). Å gjenta dette kan oppfattes som støy, og gir ikke noen nyttig ekstra-informasjon. Bildet skal derfor ha et tomt alt-attributt.
			- ![Spørsmål i en søknadsprosess, med en snakkeboble med grønn hake over](https://trello-attachments.s3.amazonaws.com/5c0146cd37715d284e75a4f3/770x406/899dc9b8bca3f4f3108ab11b8edb207b/erfaring.png) OBS! Her kan en alt-tekst potensielt forvirre brukeren: En slik grønn hake står ofte for "godkjent" eller "ferdig". Har man med noe liknende i alt-teksten her, kan brukeren få inntrykk av at prosessen ar avsluttet. Siden bildet bare skal illustrere erfaringen man har, og dette står rett under, burde bildet ha et tomt alt-attributt.
			- ![Skjermdump fra foreldrepenger som viser illustrasjoner som understøtter teksten](https://trello-attachments.s3.amazonaws.com/5c0146cd37715d284e75a4f3/716x593/7976b324d8088742f7ef1c6cd81ebb55/foreldrepengerengangsst%C3%B8nad.png) Både veiviseren i toppen, og figurene for mor, far og medmor vises rett ved siden av tekst som sier akkurat det samme. De skal derfor ha tomt alt-attribut.
- **Nei**
	- Fortsett
4.  **Er bildet rent dekorativt/pynt eller ikke beregnet for brukeren?**
- **Ja**
	- → Bruk et tomt alt-attributt eller legg bildet inn i CSS. Se [dekorative bilder (engelsk)](https://www.w3.org/WAI/tutorials/images/decorative/) → eksempel: prikk, skillelinje, punkt
- **Nei**
	- Fortsett
5.  **Er bildet ikke nevnt ovenfor, eller det er uklart hva alt-tekst skal gi?**
- Dette beslutningstreet dekker ikke alle tilfeller. For detaljerte opplysninger om levering av tekstalternativer, se  [bildekonsept-siden (engelsk)](https://www.w3.org/WAI/tutorials/images/).

# Hvordan skrive alt-tekster
(oversettelse fra  [https://www.w3.org/WAI/tutorials/images/tips/](https://www.w3.org/WAI/tutorials/images/tips/)  pluss info om tomt alt-attributt)

Vi anbefaler å ta [Difis gratis e-læringskurs for redaktører og skribenter](https://uu.difi.no/krav-og-regelverk/kom-i-gang/e-laeringskurs-om-universell-utforming-av-nettinnhold). Kurset ligger også inne i NAVs læringsportal.

## Tomt alt-attributt
Dekorative bilder skal ha et tomt alt-attribut ( `alt=""` ). Det er ikke anbefalt å bare fjerne alt-attributet helt, siden noen skjermlesere da leser opp filnavnet eller kilde-URLen til bildet.

## Velge passende tekstalternativer
Tenk deg at du leser websiden høyt over telefonen til noen som trenger å forstå siden. Dette bør hjelpe deg med å bestemme hva (hvis noe) informasjon eller funksjon bildene har. Hvis de ser ut til å ha ingen informativ verdi og ikke er koblinger eller knapper, er det sannsynligvis trygt å behandle dem som [dekorative](https://www.w3.org/WAI/tutorials/images/decorative/) .

## Prioritere informasjon i tekstalternativ
Sats på å sette viktig informasjon i begynnelsen.

## Tekstalternativets lengde
alt-teksten skal beskrive bildets formål så konsis som. Hvis det er behov for noe mer enn noen få ord eller en setning, vil det være bedre å bruke en av de lange beskrivningsmetoder som diskuteres i [komplekse bilder](https://www.w3.org/WAI/tutorials/images/complex/) .

## Tegnsetting innen alt-attributter
Tegnsetting kan gjøre det lettere å forstå informasjon i tekstalternativet, akkurat som i andre tekster. Husk spesielt å legge til mellomrom i alt-teksten når det ikke er mellomrom mellom bildet og den nærliggende teksten, for å unngå at ord løper sammen når de leses av en skjermleser.

Hvis du bruker et null (tomt) tekstalternativ ( `alt=""` ) for å skjule dekorative bilder, må du sørge for at det ikke er mellomrom mellom siterne. Hvis et mellomrom er til stede, kan det hende at bildet ikke er effektivt skjult fra hjelpeteknologi. For eksempel vil noen skjermlesere fortsatt kunngjøre tilstedeværelsen av et bilde hvis et mellomrom er satt mellom anførselstegnene.

## Overflødig informasjon i tekstalternativet
Vanligvis er det ikke nødvendig å inkludere ord som "bilde", "ikon" eller "bilde" i alt-teksten. Folk som kan se vil vite dette allerede, og skjermlesere kunngjør tilstedeværelsen av et bilde. I noen situasjoner kan det være viktig å skille mellom malerier, fotografier eller illustrasjoner, etc., men det er best å unngå mer generisk bruk av betingelsene.

## SVG-grafikk
SVG-grafikk kan refereres i `src` attributtet til et `<img>` -element som andre bildeformater (PNG, JPEG, GIF). I dette tilfellet kan eksemplene på denne opplæringen også brukes sammen med SVG.

Som SVG-bilder består av tagger som HTML, kan koden også brukes direkte i HTML5. I dette tilfellet kan du gi et tekstalternativ i et `<title>` -element i SVG-bildet. For å forbedre tilgjengelighetsstøtten bør denne tittelen refereres fra et `aria-labelledby` attributt til `<svg>` -elementet, for eksempel:

`<svg aria-labelledby="svgtitle1"> <title id="svgtitle1">Settings</title> [other svg code] </svg>`

## Logos
Logo-bilder med tekst er unntatt fra noen av tilgjengelighetskravene. For eksempel er det ikke noe minimumskrav til kontrast.
