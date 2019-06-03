# Prinsipper Innholdsstruktur

Denne siden inneholder:

* Hvorfor strukturert innhold?
* Tre ting du skal vite om innhold på nett
* h1- og title-elementer
* Strukturér siden hierarkisk
* Tenk på framtiden og gjenbruk ved å skrive modulært
* Ofte-stilte spørsmål *(blir nok erstattet av ekte seksjoner)*


## Hvorfor strukturert innhold?

Når vi skriver strukturert innhold, gjør vi det fordi:

* det ønskete innholdet blir lettere å finne (SEO, lenketekst, søketreff, med mer)
* brukeren skjønner fort om de er på riktig sted
* brukeropplevelsen blir mer konsekvent, samt universelt utformet
* innholdet blir lettere å vedlikeholde og gjenbruke
* dermed rigger vi for framtiden. 

Hvordan skrive enkelt, konsekvent og tilgjengelig dekkes av [Slik skriver vi](https://design.nav.no/resources/language). 

 
### Tre ting du skal vite om innhold på nett

1. Alle nettsider skrives og leses i et språk som heter HTML, som er en forkortelse for *hypertext markup language*. Du trenger ikke å kunne HTML selv. Men du burde ha en viss forståelse for at den finnes, for det har mye å si for hvordan innhold struktureres, oppleves, og brukes.

2. HTML omfatter både selve ordene du leser på nett, og såkalt 'metadata', som er *innhold som beskriver selve innholdet* (derfor 'meta'). Metadata brukes blant annet til markering av hvilke ord utgjør overskriften, hvilke er mellomoverskrifter, og hvilke er brødtekst. Metadata skrives ved å pakke ord og media inn i 'elementer' som brukeren ikke ser. For eksempel, når vi skal navngi en nettside, skriver vi `<title>Bla bla</title>`. Brukeren leser kun 'Bla bla' på nett.

3. Når vi skriver innhold og metadata i HTML, er dette stort sett uavhengig av *utseendet på nett*, nemlig farge, størrelse, posisjon, og så videre. Utseendet løser vi på en annet sted ved å lage en 'frontend', der vi bestemmer, for eksempel, hvor stor alle tittelene eller brødtekstene blir. Men innholdet er kjernen :) 

## h1- og title-elementer

Når vi oppretter en ny side, finnes det to måter å navngi den i HTML:

1. `<title>The title element</title>`. 

2. `<h1>The h1 element</h1>`

### Om title-elementet

`title` brukes til søkemotoroptimalisering, også kjent som SEO. Søketjenester som Google, samt internt søk på nav.no, henter ut det som sidens innhold handler om, ut fra det som skrives i `title`-elementet. Her er det viktig med en god match mellom title og faktisk innhold, for at brukeren ikke blir villedet. 

`title`-elementet brukes også av sosiale medier når de skal forhåndsvise innholdet som lenkes til.

Sist blir `title`-elementet brukt av nettleseren din (Chrome, Internet Explorer, og lignende). Ved å åpne en nettside i nettleseren får du den lille fanen i topp, der det står `Person - nav.no`, eller hva det er. Denne beskrivelsen hentes fra `title`-attribute'n.

I sum blir `title`-elementet brukt andre steder som en slags reklame eller veiskilt for sidens innhold. Derfor er det viktig med en `title` som faktisk speiler innholdet.

### Om h1-elementet

`h1` er den viktigste "heading"-en (derfor 'h' og '1') på en nettside. `h1` bør være den aller første delen av sidens innhold du treffer, enten det er visuelt eller med skjermleser, og om du bruker tastaturet til navigering eller ei. Dermed er `h1` til orientering når først du havner på siden. Dette gjør at `h1` må gi oversikt over akkurat det som siden handler om. `h1` skal helst være temmlig kort, men det er viktigst at den gir mening. 

`h1` skal være unik, og la seg skille fra alle andre sider på tvers av hele nettstedet. Dette er særskilt viktig når brukeren skal gjennom flere sider i løpet av en søknad eller annen flyt. Her er det ofte til hjelp å tenke på hvordan nettstedet ville blitt opplevd av en som bruker skjermleser, og som dermed navigerer med utgangspunkt i `h1`-elementer. Men egentlig, når vi skriver unike, tydelige `h1`-elementer, tjener vi alle brukere. 

**Det skal kun finnes én `h1` pr. side.** Alt annet innhold på den siden må være på `h2`-nivå eller lavere. Dette legger opp til bedre søk, bedre navigasjon, og bedre tilgjengelighet.

### Hvorfor finnes både title og h1?

Du skal bruke begge deler, men ikke nødvendigvis til akkurat samme mål.

#### Bruk `title` for å gi brukeren kontekst i det hele, og det fjerne
Det er ofte nyttig å ha med "domenet", det vil si nav.no, i `title`-elementet. Den som finner NAVs innhold via Google eller sosiale medier skal vite, før hen velger lenken, om den kan være relevant eller ei. Hvilket nettsted siden ligger på er en ofte en viktig del av vurderingen. Derfor er det bra med domenenavnet i `title`-elementet, som for eksempel `Sykepenger – www.nav.no` og `Foreldrepenger – www.nav.no`. (Det kan hende at "www"-delen kommer til å forsvinne på sikt, men vi får se.)

Fanene i nettleseren bruker også `title`-elementet, og det er nyttig å ha med domenenavnet når en blader gjennom flere åpne faner i nettleseren.

#### Bruk `h1` til orientering når brukeren navigerer aktivt
`h1` skal nok ikke ha med domenet. `h1` er heller elementet som oppsummerer en side når du nylig har havnet der. Det ville vært kjedelig med overskrifter på hver eneste side som enten begynte eller sluttet med "nav.no". Tenk på `h1`-elementet som viktig orientering ved overganger. For eksempel kan en bruker gå fra "Hva er din situasjon?" til "Sykdom i familien" og vite hvor de er.

#### Kan ikke du bruke samme tekst på `h1` og `title` da?
Jo, men helst ikke som regel. Tenk hvordan `h1`- og `title`-elementene ville blitt opplevd i kontekstene nevnt ovenfor.

Finnes det et unntak, er det nok at forsiden til hele nettstedet kan ha godt av å inkludere domenenavnet i `h1`-elementet. Dette gjør for eksempel gov.uk, til orientering for de som nettopp ankom. 

### Videre lesning

[SEO and the title tag – moz.com](https://moz.com/learn/seo/title-tag)
[Heading elements – Mozilla.org](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements)
[Page title and h1: best practices – Web developer network](https://wdn.unl.edu/page-title-h1-best-practices)


## Strukturér siden hierarkisk

`h` betyr "heading". Den brukes i HTML til å bygge opp informasjonshierarkiet på nettsiden.

Hierarchien bygges ved å bruke `h1` som viktigste element, `h2` som nest viktigst, osv. Bortsett fra `h1`, som skal være øverst, handler ikke strukturen om rekkefølgen nedover siden, men heller grenene til et tre. Du skal kun ha én `h1` (trestamme), men du får ha så mange `h2` (grener) du vil. Trenger du enda et nivå under enkelte `h2`, kan du bruke `h3` (kvister), osv. 

Vær streng med hvordan du organiserer hierarkiet. Ikke strukturér innholdet slik at plutselig innen en `h1` seksjon dukker opp en `h3`, uten at du først har truffet en `h2` på vei dit. Det finnes stort sett ingen kvister uten grener.

Ikke skap dype hierarkier. Det holder nesten alltid med `h1` til `h3`, men du kan til tider kjenne behov for `h4`. Er siden så kompleks at du er helt ned på `h6`, kan det være lurt å helst omstrukturere innholdet til en side med flere undersider. Hos brukeren legger et dypt hierarki opp til mye leting gjennom de forskjellive nivåene. Dessuten er en sannsinlig følge av dypt hierarki ganske lange sider, som oppleves som vanskelig. Vær snill mot brukeren og behold strukturen enklest mulig.


### Utseendet skal speile semantikken

Som sidens viktigse og mest informasjonsbærende element, ville det vært veldig sjelden at `h1` *ikke* utgjør den største teksten. `h2` pleier å være noe mindre, `h3` tar enda mindre plass, og så videre. Størrelsen fungerer som ledetråd når brukeren prøver å fatte hva som er viktigst på siden.

Ikke bruk hierarki som erstatning for akkurat den typografien du vil ha på enkelte overskrifter. Sånn ødelegger du for navigasjon gjennom hierarkiet. Tenk igjen på skjermleserbrukeren, som navigerer ved `h`-overskrifter og mellomoverskrifter, og som må vurdere om de vil "drill down" eller gå videre. Bruk `h`-elementer kun av semantiske grunner.


### Videre lesning

[Page structure: headings – W3.org](https://www.w3.org/WAI/tutorials/page-structure/headings/)


## Tenk på framtiden og gjenbruk ved å skrive modulært

### Det historiske blikket: overskrifter, lange tekster, og duplisert innhold
En gang i tid var det greit å ha en lang nettside med `h1`, et par `h2`, og masse brødtekst. Men dersom du hadde behov for å finne noe spesifikt på den siden, måtte du ploge gjennom alt innholdet fram inntil du fant akkurat det du let etter. Ved søk ville du heller ikke funnet noe bedre en én lenke til hele den siden. I dag finnes mye av dette igjen fra før.

Et annet arvegods er gjentakelse av samme innhold flere steder på dagens nav.no. Dette legger opp til dobbeltarbeid ved å måtte vedlikeholde innhold om samme ting på flere steder. Det gjør også at brukerne lurer på hva som kan være forskjellen mellom flere tekster som nevner samme sak, men som er beskrevet på hver sin måte.

### I dag kan vi bruke mellomoverskrifter til spisset søk
Selv om `h1` er viktigst for søkemotorer, er det i disse dager også lurt å skrive gode mellomoverskrifter, nemlig `h2` og nedover. Dermed legger vi opp til en brukeropplevelse der brukeren taster inn "Hvor lenge foreldrepenger" i søkeboksen, og får et treff som heter "Hvor lenge kan du få foreldrepenger?". Lenken leder til akkurat den seksjonen brukeren lurer på, framfor å måtte gå til toppen av "Om foreldrepenger" og lese gjennom alt. **Obs!** Dette fine bildet gjelder kun dersom siden er riktig strukturert, og dersom søkemotoren rigges tilsvarende.

### Ved godt-strukturert innhold kan vi få til "rediger ett sted, få lest på flere"
Når vi bygger dagens systemer og skriver dagens innhold, skal vi sørge for at tekster gjenbrukes framfor dupliseres. Er det behov for at noe skal stå flere steder, er det åpenbart smart å skrive teksten én gang og så gjenbruke, hvis det lar seg gjøre. Slik kutter vi dobbeltarbeid hos redaksjon, og unngår dupliserte tekster som begynner likt, men som med tid utvikler seg forskjellig. I samme slange kutter vi forvirring og leting hos brukeren, som så senker antall henvendelser til kundesenteret.  

### I framtiden kommer enda smartere løsninger
Ved smart bruk av strukturert innhold på nett, muliggjør vi bedre løsninger. Brukeren taster "hvor lenge varer foreldrepenger?" og chatbot-en svarer med hele den "Hvor lenge kan du få foreldrepenger?"`h2`-seksjon. Kanskje får brukeren flere lenker videre til enkelte `h3`-elementer innen "Hvor lenge", som for eksempel "Far og mor", "Bare far har rett", og så videre. Igjen får brukeren hjelp til å finne akkurat det de lurer på. Bedre chatbot-løsninger er sikkert kun én blant flere måter å utnytte stukturert innhold på. Jo bedre strukturert innholdet vårt, desto bedre forberedt vi blir for en framtid vi ikke aner noe om ennå :) 


## Ofte-stilte spørsmål

(Ofte-stilte spørsmål kan være et tegn på at innholdet ikke er godt nok organisert, og burde helst utgjort egne seksjoner. Work in progress.) 


### Folk snakker om hodeløst, men hva er dette egentlig?

"Hodeløst innhold" betyr at selve innholdet og hvordan innholdet brukes og settes sammen er helt (eller delvis) frakoblet. Sånn sett gjør "hodeløst" at du kan trekke ut innholdet på mange mulige flater, om det er nettsider, sosiale medier, chatbots, smart-home løsninger, you name it. Men da vil du kun hente ut akkurat det innholdet som passer til anledningen. Dermed er en hel side ofte for mye innhold av gangen, eller ikke spisset nok. Det er her vi kjenner behov for strukturert innhold, for å så kunne kalle fram enkelte seksjoner, som for eksempel en `h2` samt brødteksten som hører til mellomoverskriften. Sånn sett burde en nettside vært godt strukturert.

Du kan ha lest om "hodeløst CMS", der CMS står for Content Management System. Et CMS innebærer ofte at det finnes et redaksjonsgrensesnitt der det går an å opprette og redigere innhold. Tradisjonalt sett var det typisk å bygge opp nettsteder ved å lage maler som tilsvarte hele sider, og gjenbruke malene ved innholdsskriving. Dette var helt greit, men gjorde at det var vanskelig å gjenbruke innholdsbiter mindre enn en hel side. 

Har teamet ditt bygget egen web-app, er det sannsynlig at det ikke finnes eget redaksjonsgrensesnitt. I så fall er nok enten innholdet hentet fra andre kilder, og/eller hard-kodet. Hard-kodet betyr at du må inn i selve HTML for å redigere teksten. Dette kan selv du, som ikke er særlig teknisk innstilt, få til med litt hjelp og noen kule verktøy :)


### Hva er SEO for noe, og hvordan fungerer det?

SEO står for søkemotoroptimalisering. Optimaliseringen handler om å gjøre innhold oppdagelig ved søk, om det er google eller nav.no sitt internt søk. Begge to krever en form for SEO for at riktig innhold oppdages og presenteres.
 
 *Bla bla, her kommer mer tekst. Forslag trengs!*

### Hvordan skal vi håndtere innhold som ligger i en blanding av CMS'er, skreddersydde web-apper, med mer? 

You tell me. Men her kommer litt tankemat:

1. Jo bedre oversikt vi har over alle disse systemene med innhold oppi, desto lettere det blir å forstå hvordan vi kan bedre dagens situasjon. Jobb for at alle får en bedre oversikt over innhold og hvor det ligger. Ikke bli satt fast i egen gullgruve.

2. Det er litt styr å få systemer til å snakke sammen, men man skal ikke se bort fra de store gevinstene som kan oppstå som følge av arbeidet — for eksempel færre henvendelser til kundesenteret. Vi burde [do the hard work to make it simple](https://www.gov.uk/guidance/government-design-principles#do-the-hard-work-to-make-it-simple)

3. Det om at dagens systemer ikke alltid snakke sammen er en slags teknisk gjeld (engelsk: [technical debt](https://en.wikipedia.org/wiki/Technical_debt)). Dette arbeidet kan ikke forskyves i all evighet. Hvorfor ikke begynne på det nå? 

4. Alt følger med egen [opportunity cost](https://en.wikipedia.org/wiki/Opportunity_cost). Om innholdsstrukturen bør forbedres på bekostning av andre ting, er blant det vanskeligste arbeidet som finnes. Prioritering er vanskelig arbeid. Men [break any of these rules* sooner than do anything barbaric](https://public.digital/2018/10/12/internet-era-ways-of-working/) 

_* ikke regelen om kun én `h1` element, da_