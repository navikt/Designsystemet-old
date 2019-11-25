# Tilgjengelighet og universell utforming

Å leve med nedsatt funksjonsevne fører ofte med seg utfordringer i dagliglivet, deriblant bruk av teknologi. Når vi i NAV lager løsninger som er tilgjengelig for alle, bidrar vi til at de aller fleste kan klare seg selv.

Ved å tekste video slik at hørselshemmede kan få med seg viktig informasjon, gjør vi det også mulig for alle å se tekstet video i støyende omgivelser.

## Få en bra start i design- og utviklingsprosessen

Vi tar hensyn til krav til universell utforming (kravene i WCAG 2.0, level AA) når vi utformer og tester elementene i Designsystemet (vi jobber med WCAG 2.1). Dette gjelder for eksempel fargekontrast: Bruk de fargekombinasjonene du finner her, og du møter kontrastkravene som er satt.

Designsystemet bruker standard-HTML som gjør det mulig for de aller fleste å lese innholdet og betjene elementene, også de som bruker hjelpemidler. Der standard-HTML ikke er tilstrekkelig, har vi lagt til WAI-Aria. Elementene er testet med skjermleser.

Til hvert element finner du referanser til relaterte krav og beste praksis.  
Vær oppmerksom på at du ikke automatisk oppfyller alle krav NAV stiller til universell utforming og brukeropplevelse. Men ved å bruke Designsystemet, unngår du mange vanlige (og dyre) feil.

## Rutiner
### Design
1.  Bruk aktuell versjon av [NAVs komponent- og illustrasjonsbibliotek i Sketch](resources/new-project) når du designer.
2.  Design for grupper med spesielle behov («ytterkantene»). Spør deg selv: Hadde bestemoren min klart å bruke tjenesten? [Om inklusive design](http://www.inclusivedesigntoolkit.com/whatis/whatis.html)
3.  Husk god kontrast, både i tekst, grafer og illustrasjoner. /Lenke farger/
4.  Bilder, illustrasjoner og grafer: Husk å ha beskrivende alt-tekster. /Lenke retningslinjer alt-tekst/
5.  Når farge benyttes for å gjøre informasjon tydeligere, skal du alltid bruke noe i tillegg til farge som formidler samme informasjon. Da vil innholdet også fungere for personer som ikke kan oppfatte farge, og man kan skrive ut i svart-hvitt uten at fremhevet informasjon blir borte. [Om bruk av farge](https://uu.difi.no/krav-og-regelverk/losningsforslag-web/bruk-av-farger) 
6.  Video: Husk å ha en tekstversjon som har samme innhold som videoen på siden, samt tekste video og bruk nyeste versjon av QBrick. Snart kommer en lovendring om at videoer også må være synstolket. Det betyr at man skal tilby en audiobeskrivelse av det som vises i videoen som ikke blir tydelig av selve lydsporet. 
7.  Språk og begreper: Skriv så forståelig som mulig og test teksten. Bruk beskrivende overskrifter, deloverskrifter og punktlister der det er hensiktsmessig. Husk å ha en hovedoverskrift som beskriver hovedinnholdet på siden. [Om struktur]([https://uu.difi.no/krav-og-regelverk/losningsforslag-web/tekst-og-struktur](https://uu.difi.no/krav-og-regelverk/losningsforslag-web/tekst-og-struktur)) og [hvordan skrive for nett]([https://design.nav.no/resources/language](https://design.nav.no/resources/language)
8.  Lenker: Skriv lenketekster slik at det er tydelig hvor lenken går. Ikke åpne lenker i ny fane/vindu. [Hvordan utforme lenker](https://design.nav.no/components/lenke/accessibility)
9.  Lag gode og [beskrivende feilmeldinger](https://uu.difi.no/krav-og-regelverk/losningsforslag-web/feilhandtering)  og pass på at meldingene er i tråd med Designsystemet.
10.  Test med reelle brukere, også med personer som bruker hjelpemidler Bruk gjerne Sanselaben i Sannergata (rom 5006)

### Utvikling

1.  Bruk NAV frontend. [Ressurser på GitHub]([https://design.nav.no/resources/new-project](/resources/new-project))
2.  Sjekk at koderekkefølgen gjenspeiler den visuelle rekkefølgen – skru av CSS i nettleseren
3.  Test at alt kan betjenes med tastatur og at fokusmarkering flyttes i forventet rekkefølge. 
4.  Bruk semantisk kode
5.  Sjekk at du har med [hopp-lenkene](https://www.w3.org/TR/WCAG21/#bypass-blocks)  og at de fungerer. 
6.  Sjekk at du har med [riktig <title>](https://www.w3.org/TR/WCAG21/#page-titled)  – Formen skal være "hovedinnhold på siden -  www.nav.no" 
7.  Pass på riktig [overskriftshierarki]([https://uu.difi.no/krav-og-regelverk/losningsforslag-web/tekst-og-struktur](https://uu.difi.no/krav-og-regelverk/losningsforslag-web/tekst-og-struktur))
8.  HTML skal validere.
9.  Bruk [WAI-Aria](https://www.w3.org/WAI/standards-guidelines/aria) der HTML ikke er tilstrekkelig, for eksempel på [feilmeldinger](https://www.w3.org/TR/WCAG21/#status-messages)
10.  Sjekk jevnlig med automatiserte testverktøy som WAVE eller Sortsite.
11.  Test skjermleserfunksjonalitet. For eksempel med chrome vox, VoiceOver på mac, TalkBack på android.
12.  Hvis mulig, bruk [NAV-ally](https://www.npmjs.com/package/nav-ally) i utviklingsprosessen.
13.  Test med reelle brukere, også med personer som bruker hjelpemidler.
