# Prinsipper Innholdsstruktur

Denne siden inneholder:

* Hvorfor strukturert innhold?
* Tre ting du skal vite om innhold på nett
* h1- og tittel-elementer
* Strukturér siden hierarkisk
* Tenk på framtiden og gjenbruk ved å skrive modulært
* Ofte-stilte spørsmål *(blir nok erstattet av ekte seksjoner)*


## Hvorfor strukturert innhold?

Denne siden handler om innholdsstrukturering som legger opp til at:

* brukeropplevelsen blir mer konsekvent og universelt utformet
* det ønskete innholdet blir lettere å finne (SEO, lenketekst, søketreff, med mer)
* brukeren skjønner fort om de er på riktig sted
* innholdet blir lettere å vedlikeholde og gjenbruke
* vi rigger for framtidens innhold. 

Hvordan skrive enkelt, konsekvent og tilgjengelig dekkes av (Slik skriver vi)[https://design.nav.no/resources/language]. 

 
### Tre ting du skal vite om innhold på nett

1. Alle nettsider skrives og leses i et språk som heter HMTL, som er en forkortelse for *hypertext markup language*. Du trenger ikke å kunne HTML selv, men du burde ha en viss forståelse for at det finnes, for det har mye å si for hvordan innhold struktureres.  

2. HTML omfatter både selve ordene du leser på nett, og såkalt 'metadata', som er innhold *som beskriver* selve innholdet (derfor 'meta'). Metadata brukes blant annet til å markere hvilke ord utgjør overskriften, hvilke er mellomoverskrifter, og hvilke er brødtekst. Metadata skrives ved å pakke ordene som brukeren leser inn i 'tags', som brukeren ikke ser. For eksempel, når vi skal navngi en nettside, skriver vi `<title>Bla bla</title>`. Brukeren leser kun 'Bla bla' på nett.

3. Når vi skriver innhold og metadata i HTML, er dette stort sett uavhengig av *utseendet på nett*, nemlig farge, størrelse, posisjon, og så videre. Utseendet løser vi på en annet sted ved å lage en 'frontend', der vi bestemmer, for eksempel, hvor stor alle tittelene eller brødtekstene blir. Men det er innholdet som er kjernen vår :) 

## h1- og title-elementer

Når vi oppretter en ny side, finnes det to måter å navngi den i HTML:

1. `<title>The title attribute</title>`. 

2. `<h1>The h1 attribute</h1>`

### Om title-elementet

`title` brukes til søkeoptimalisering (SEO), der google og andre vil hente ut det som sidens innhold handler om, ut fra det som skrives i `title`-elementet. Her er det viktig med en god match mellom title og faktisk innhold, for at brukeren ikke skal villedes. 

`title` konsumeres også av nettleseren din (Chrome, Internet Explorer, og lignende). I nettleseren finner du den lille fanen i topp, der det står `Person - nav.no`. Denne beskrivelsen hentes fra `title`-attribute'n.

`title` trekkes inn av sosiale medier når de skal forhåndsvise innholdet som lenkes til. 

I sum blir `title`-elementet brukt andre steder, som reklame eller veiskilt for sidens innhold. Derfor er det viktig med en `title` som faktisk speiler innholdet.

### Om h1-elementet

`h1` brukes til orientering når først du havner på en bestemt nettside. `h1` skal være den aller første tingen du leser (om det er visuelt eller med skjermleser). Sånn sett må den gi en godt og helst kort oversikt over hva siden handler om.

`h1` skal være unik, og la seg skille fra alle andre sider på tvers av hele nettstedet. Her er det ofte til hjelp å tenke på hvordan nettstedet ville blitt opplevd av noen som bruker skjermleser, hadde hen kun navigert ved `h1`-elementer. Alle tjenes av å ha unike, tydelige `h1`-elementer.

**Det skal kun finnes én `h1` pr. side.** Alt annet innhold på den siden må være på `h2`-nivå eller lavere.

### Hvorfor finnes både title og h1?

Du skal bruke begge deler, men ikke til akkurat samme mål.

#### Bruk `title` for å gi brukeren kontekst i det hele, og det fjerne
Se for deg at noen oppdager nav.no sitt innhold via Google eller sosiale medier. Hen skal vite, før hen velger lenken, om den kan være relevant eller ei. Eller tenk på den som blader gjennom alle de 30 åpne fanene i nettleseren for å finne tilbake til noe. Kanskje står det faner som viser flere forskjelle sider fra nav.no. Her kan det være til hjelp å vite at alle de fanene inneholder innhold på nav.no, kontra andre nettsteder. Derfor for eksempel `Sykepenger – nav.no` og `Foreldrepenger – nav.no`. 

#### Bruk `h1` til orientering når brukeren navigerer aktivt
Tenk deg hvor kjedelig det ville vært dersom alle titlene du leste på tvers av nav.no enten hadde begynt eller sluttet med "nav.no". Dette ville lagt opp til mye unødvendig støy. Derfor bruker vi `h1` til orientering når en navigerer fra, for eksempel, "Hva er din situasjon?" til "Sykdom i familien". Ut fra `h1` på ankomst-siden skal brukeren vite hvor hen er kommet fram til.

Er du i tvil, kan du bruke akkurat samme tekst til både `h1` og `title`, men tenk gjerne over hvordan de henholdsvis ville blitt opplevd i de tilfellene nevnt ovenfor.

### Videre lesning

(SEO and the title tag – moz.com) [https://moz.com/learn/seo/title-tag]
(Heading elements – Mozilla.org)[https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements]
(Page title and h1: best practices – Web developer network)[https://wdn.unl.edu/page-title-h1-best-practices]


## Strukturér siden hierarkisk

`h` betyr "heading". Den brukes i HTML til å bygge opp informasjonshierarkiet på nettsiden.

Hierarchien bygges ved å bruke `h1` som viktigste element, `h2` som nest viktigst, osv. Bortsett fra `h1`, som skal være øverst, handler ikke strukturen om rekkefølgen nedover siden, men heller grenene til et tre. Du skal kun ha én `h1` (trestamme), men du får ha så mange `h2` (grener) du vil. Trenger du enda et nivå under hver enkelt `h2`, kan du bruke `h3` (kvister), osv. 

Vær streng med hvordan du organiserer hierarkiet. Ikke strukturér innholdet slik at innen en `h1` seksjon plutselig dukker opp en `h3`, uten at du først har truffet en `h2` på vei dit. Det finnes stort sett ingen kvister uten grener.

Ikke skap dype hierarkier. Det holder nesten alltid med `h1` til `h3`, men du kan til tider kjenne behov for `h4`. Er siden så kompleks at du er helt ned på `h6`, kan det være lurt å helst omstrukturere innholdet til en side med flere undersider. Dermed slipper brukeren å måtte forholde seg til mye leting opp og ned gjennom nivåene på samme side.


### Utseendet skal speile semantikken

Som sidens viktigse og mest informasjonsbærende element, ville det vært veldig sjelden at `h1` *ikke* utgjør den største teksten. `h2` pleier å være noe mindre, `h3` tar enda mindre plass, og så videre. Størrelsen fungerer som ledetråd når brukeren prøver å fatte hva som er viktigst på siden.

Ikke bruk hierarki som erstatning for akkurat den typografien du vil ha på enkelte overskrifter. Sånn ødelegger du for navigasjon gjennom hierarkiet. Tenk for eksempel på skjermleserbrukere, som navigerer ved `h`-overskrifter og mellomoverskrifter, og som må vurdere om de vil "drill down" eller gå videre. Bruk kun `h`-elementer av semantiske grunner.


### Videre lesning

(Page structure: headings – W3.org)[https://www.w3.org/WAI/tutorials/page-structure/headings/]


## Tenk på framtiden og gjenbruk ved å skrive modulært

### Det historiske blikket: overskrifter, lange tekster, og duplisert innhold
En gang i tid var det greit å ha en lang nettside med `h1`, et par `h2`, og masse brødtekst. Men dersom du hadde behov for å finne noe spesifikt på den siden, måtte du ploge gjennom alt innholdet fram inntil du fant akkurat det du let etter. Ved søk ville du heller ikke funnet noe bedre en én lenke til hele den siden. I dag finnes mye av dette igjen fra før.

Et annet arvegods fra de gode gamle dager er gjentakelse av samme innhold flere sider. Dette legger opp til dobbeltarbeid ved å måtte vedlikeholde innhold om samme ting på flere steder. Det gjør også at brukerne lurer på hva som kan være forskjellen mellom flere tekster som nevner samme sak, men som er beskrevet på hver sin måte.

### I dag kan vi bruke mellomoverskrifter til spisset søk
Selv om `h1` er viktigst for søkemotorer, er det i disse dager også lurt å skrive gode mellomoverskrifter, nemlig `h2` og nedover. Dermed legger vi opp til en brukeropplevelse der brukeren taster inn "Hvor lenge foreldrepenger" i søkeboksen, og får et treff som heter "Hvor lenge kan du få foreldrepenger?". Lenken leder til akkurat den seksjonen brukeren lurer på, framfor å måtte gå til toppen av "Om foreldrepenger" og lese seg gjennom alt. **Obs!** Dette fine bildet gjelder kun dersom siden er riktig strukturert, og dersom søkemotoren rigges tilsvarende.

### Ved godt-strukturert innhold kan vi få til "rediger ett sted, få lest på flere"
Når vi bygger dagens systemer og skriver dagens innhold, skal vi sørge for at tekster gjenbrukes framfor dupliseres. Er det behov for at noe skal stå flere steder, er det åpenbart smart å skrive teksten én gang og så gjenbruke, hvis det lar seg gjøre. Slik kutter vi dobbeltarbeid hos redaksjon, og unngår dupliserte tekster som begynner likt men som med tid utvikler seg forskjellig. I samme slange kutter vi forvirring og leting hos brukeren, som så senker antall henvendelser til kundesenteret.  

### I framtiden kommer enda smartere løsninger
Se for deg at enkelte seksjoner av nettsiden kunne gjenbrukes av en nav.no chatbot. Brukeren taster "hvor lenge varer foreldrepenger?" og chatbot-en kan svare med hele den "Hvor lenge kan du få foreldrepenger?"`h2`-seksjon, eller eventuelt lenker videre til flere mulige `h3` elementer som hører hjemme under den opprinnelige`h2`, som for eksempel "Far og mor", "Bare far har rett", og så videre. Igjen får brukeren hjelp til å finne akkurat det de lurer på. Chatbots er sikkert kun én blant flere måter å utnytte stukturert innhold på.


## Ofte-stilte spørsmål

Jeg misliker egentlig ofte-stilte spørsmål, og vil helst at de omfattes av egne seksjoner. Work in progress. 


### Folk snakker om hodeløst, men hva er det egentlig?

"Hodeløst innhold" betyr at selve innholdet og hvordan innholdet brukes og settes sammen er helt (eller delvis) frakoblet. Tanken er at det er bedre å ha små biter med godt strukturert innhold, som så kan settes sammen på nye måter ved behov, framfor å ha rigide sider (typisk sett maler) som ikke kan tas fra hverandre når det kun er en del som er relevant.

Du kan ha lest om "hodeløst CMS", der CMS står for Content Management System. Et CMS innebærer ofte at det finnes et redaksjonsgrensesnitt der det går an å opprette og redigere innholdsbiter (eventuelt hele sider, eventuelt hele sider som selv er en sammensetning av diverse innholdsbiter).

Har teamet bygget egen web-app, kan det hende at det ikke finnes eget redaksjonsgrensesnitt. I så fall er nok enten innholdet hentet fra en annen kilde, eller hard-kodet (det vil si at du må inn i selve HTML for å redigere teksten).


### Hva er SEO for noe, og hvordan fungerer det?

 Vi har behov for at søkemotorer oppdager innholdet som treffer det som brukerne søker etter, om det er google eller nav.no sitt internt søk. Det å tiltrekke oppmerksomheten til søkemotorer kalles for søkemotoroptimalisering (også kjent som *search engine optimisation*, forkortet SEO). 
 
 *Bla bla, her kommer mer tekst.*

### Hvordan skal vi håndtere innhold som ligger i en blanding av CMS'er, skreddersydde web-apper, med mer? 
You tell me. Men her kommer litt tankemat:
1. Jo bedre oversikt vi har over alle disse systemene, desto lettere det blir å forstå hvordan vi kan bedre dagens situasjon. Jobb for at alle får en bedre oversikt, og blir ikke satt fast i egen gullgruve.
2. Det er litt styr å få systemer til å snakke sammen, men man skal ikke se bort fra de store gevinstene som kan oppstå som følge av arbeidet — for eksempel færre henvendelser til kundesenteret. Vi burde (do the hard work to make it simple)[https://www.gov.uk/guidance/government-design-principles#do-the-hard-work-to-make-it-simple]
3. Det om at dagens systemer ikke alltid snakke sammen er en slags teknisk gjeld (engelsk: (technical debt)[https://en.wikipedia.org/wiki/Technical_debt]). Dette arbeidet kan ikke forskyves i all evighet. Hvorfor ikke begynn på det nå? 
