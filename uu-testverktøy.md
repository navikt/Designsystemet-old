# Verktøy for uu-testing

## Testing med skjermleser

Det finnes flere forskjellige skjermlesere. Vi anbefaler at du tester med en eller flere skjermlesere, og at du i tillegg brukertester med noen som bruker skjermleser til daglig.

VIKTIG!
Før du tar i bruk noen av verktøyene nedenfor, må du huske at sikkerhet og personvern SKAL ivaretas. Sørg derfor for at du tester på testmiljøer og lignende som har fiktiv testdata. En av grunnene til dette er at noen av utvidelsene til nettlesere KAN sende data til servere utenfor NAV.

### Voice over
https://youtu.be/5R-6WvAihms
https://youtu.be/bCHpdjvxBws
-   [Using VoiceOver to Evaluate Web Accessibility](https://webaim.org/articles/voiceover/)
-   Innebygd (gratis) skjermleser i Mac / iPhone

### NVDA
https://youtu.be/Jao3s_CwdRU
-   [Using NVDA to Evaluate Web Accessibility](https://webaim.org/articles/nvda/)
-   [Download NVDA](https://www.nvaccess.org/)

### JAWS
-   Mye brukt. Standard-skjermleser til våre interne ansatte på jobb.
-   [Using JAWS to Evaluate Web Accessibility](https://webaim.org/articles/jaws/)

### TalkBack
https://youtu.be/0Zpzl4EKCco
-   Gratis skjermleser på android-telefoner

## Validering av kode mot W3C-standarder

### Chrome DevTools (F12)
![Chrome DevTools på nav.no](https://trello-attachments.s3.amazonaws.com/590c618893f382eb61038bae/5ce698a6c8f4177fb0819822/c4770718f8d01578898e4f2a10f48178/webdev.png)
-   Chrome DevTools er et sett med webutviklerverktøy som ligger integrert i Google Chrome-nettleseren.
-   DevTools kan hjelpe deg med å redigere/manipulere en hvilken som helst nettside/tjeneste og raskt diagnostisere problemer.
-   Kan bygges ut med diverse andre utvidelser.
-   Gratis

### Audits/Lighthouse (aXe)

![Lighthouse på nav.no](https://trello-attachments.s3.amazonaws.com/590c618893f382eb61038bae/5ce698a6c8f4177fb0819822/1222fd55564188113b38632b9b77b7f1/lighthouse1.png)
![Lighthouse resultatdashboard](https://trello-attachments.s3.amazonaws.com/5ce698a6c8f4177fb0819822/761x812/f32119a329afce2cd133c3b3c0971560/Lighthouse2.png)
https://youtu.be/b0Q5Zp_yKaU

-   Lighthouse er åpen kildekode og et automatisert verktøy for å forbedre kvaliteten på nettsidene, både åpen og bak innlogging. Du kan kjøre verktøyet mot en hvilken som helst nettside. Den har evalueringsmuligheter for ytelse, tilgjengelighet/uu, progressive webapps, beste praksis, søkemotoroptimalisering for både mobile enheter og desktop.
-   Du kan kjøre Lighthouse i Chrome DevTools, fra kommandolinjen, eller som en nodemodul. Du gir Lighthouse en URL for å revidere, den kjører en del sjekker mot siden, og så genererer den en rapport som inneholder hvor godt siden gjorde det. Derfra bruker du de revisjonene som indikatorer på hvordan du kan forbedre siden. Hvert revisjon har en referansedokument som forklarer hvorfor revisjonen er viktig, samt hvordan det skal løses.
-   Gratis
-   [Download Lighthouse (axe, for chrome)](https://chrome.google.com/webstore/detail/lighthouse/blipmdconlkpinefehnmjammfjpmpbjk)

### Web Developer Toolbar
-   Toolbar med et hav av muligheter til å manipulere og konfigurere løsningen.
-   Gratis
-   [Download Web Developer Toolbar (for chrome)](https://chrome.google.com/webstore/detail/web-developer-toolbar/deeboegbjcnfgidliakhpoapnpomphji)

### ARC Toolkit
![ARC Toolkit på foreldrepengersiden](https://trello-attachments.s3.amazonaws.com/590c618893f382eb61038bae/5ce698a6c8f4177fb0819822/3a0690006ee532cc09ba3f5c2968f356/arc.png)![ARC viser overskriftsstruktur på foreldrepengersiden](https://trello-attachments.s3.amazonaws.com/590c618893f382eb61038bae/5ce698a6c8f4177fb0819822/51e6646ec39e80e352d15d7660b852c7/arc2.png)
-   Gir både oversikt og man kan gå i dybden
-   Mulighet for å teste reflow og text spacing (WCAG 2.1)
-   Gratis
-   [Download ARC Toolkit (for chrome)](https://chrome.google.com/webstore/detail/arc-toolkit/chdkkkccnlfncngelccgbgfmjebmkmce)

### Visual Aria
![Visual Aria på nav.no](https://trello-attachments.s3.amazonaws.com/5ce698a6c8f4177fb0819822/818x747/4946a00441b200d3f233257a3b54394e/VisualAria.png)
-   Viser ARIA som brukes i webteknologi, inkludert live region og widget roles, riktig nesting og fokushåndtering.
-   Gratis
-   [Download Visual Aria (for chrome)](https://chrome.google.com/webstore/detail/visual-aria/lhbmajchkkmakajkjenkchhnhbadmhmk)

### WAVE
![WAVE på nav.no](https://trello-attachments.s3.amazonaws.com/5ce698a6c8f4177fb0819822/1135x805/f896fdb516addce24a0a11b2b066d960/Wave.png)
-   Evaluerer tilgjengelighet direkte i en nettside
-   Veldig visuell
-   Gratis
-   [Download WAVE](https://wave.webaim.org/)

### AXE Coconut
https://youtu.be/1uyQdC3LqLo
-   fra Deque, kjøpt opp av Google
-   Tilgjengelighetstesting i Chrome Developer Tools
-   Gratis
-   Kan også teste shadow dom
-   [Download Axe Coconut (for chrome)](https://chrome.google.com/webstore/detail/axe-coconut/iobddmbdndbbbfjopjdgadphaoihpojp)

### SortSite
![SortSite på nav.no](https://trello-attachments.s3.amazonaws.com/590c618893f382eb61038bae/5ce698a6c8f4177fb0819822/ac7ffee05e048731f54576f30311b0ca/sortsite.png)
-   Godt verktøy for validering av grensesnittkode opp mot W3C-standarder som WCAG 2.0/2.1, HTML5, CSS3, etc. Gir en god oversikt sammen med en god beskrivelse av hva som er feil, hvor feilen er og hvordan den kan fikses.
-   Pris ca NOK 8000,- per lisens

### SiteImprove

-   Godt verktøy som gir deg en lettfattelig og god oversikt over problemer og forbedringsområder. Som f.eks. dårlig kodekvalitet og kvalitetsfeil som brutte lenker og stavefeil, kontrastforhold som er for dårlig, m.m. Verktøy tester opp mot W3Cs standarder som f.eks. HTML5 og WCAG 2.0/2.1 og man kan filtrere funnene på roller (utvikler, redaktør, etc). God beskrivelse for hva som er feil og hvordan det kan fikses.
-   Ikke gratis

### SiteImprove Accessibility Checker
![SiteImprove på nav.no](https://trello-attachments.s3.amazonaws.com/5ce698a6c8f4177fb0819822/1138x729/e5b6c6baccb549e8fa880af5eb2af7ca/Siteimprove.png)  
- Bra verktøy for å vurdere en nettside opp mot WCAG.
-   Gratis
-   [Download Siteimprove Accessibility Checker (for chrome)](https://chrome.google.com/webstore/detail/siteimprove-accessibility/efcfolpjihicnikpmhnmphjhhpiclljc)

### Total Validator Pro
![Total Validator rapport](https://trello-attachments.s3.amazonaws.com/5ce698a6c8f4177fb0819822/728x861/cad38525ffc77bdd5e2679850b3d4b55/Totalvalidator.png)
![Innstillinger Total Validator Pro](https://trello-attachments.s3.amazonaws.com/5ce698a6c8f4177fb0819822/590x526/eaa41dc3d7fa2e6c857bbf806a15417b/tvp1.png)
-   Har vært ett av de bedre verktøyet til validering av kildekode og støtte for universell utforming.
-   [Download Total Validator](http://www.totalvalidator.com/)
-   Pro-versjonen til kr 250,- (NAV har 30 lisenser)

### HTML Validator for Mozilla Firefox
-   Verktøylinje (toolbar) for Mozilla Firefox som legger til HTML validering i Vis kildekode i nettleseren. Valideringen gjøres av Tidy fra W3C.
-   [Download HTML Validator for Firefox](https://addons.mozilla.org/en-US/firefox/addon/249)

### Adobe Acrobat DC (PDF)
-   Validering av PDF-skjema opp mot W3C standarder som WCAG 2.0/2.1 (Verktøy>Tilgjengelighet>Tilgjengelighetskontroll eller Full kontroll. NAV har lisenser på dette. [Mer info om tilgjengelighetskontroll Adobe Acrobat DC](https://helpx.adobe.com/no/acrobat/user-guide.html?topic=/no/no/acrobat/morehelp/accessibility_tags_and_reflow.ug.js)

## Lese- og skrivevansker
-   Dyslexia Formatter, gjør det enklere å tilegne seg informasjon og bruke nettbaserte tjenester for folk med dysleksi
-   Gratis
-   [Download Dyslexia Formatter (for chrome)](https://chrome.google.com/webstore/detail/dyslexia-formatter/kggkghfhlppjclojgphbploiaipgogoc)

## Kontrastforhold
-   [http://contrastchecker.com/](http://contrastchecker.com/)  - her kan du legge inn fargekodene dine og få et konkret svar om kontrastforholdet er i tråd med WCAG-kravene. Du kan også se gråtoner som fargeblind (arkfaner øverst til høyre). Gratis
-   [https://webaim.org/resources/contrastchecker/](https://webaim.org/resources/contrastchecker/). Gratis
-   [http://accessible-colors.com/](http://accessible-colors.com/). Gratis

## Mobil- og nettleserkompatibilitet
-   BrowserStack - Instant access to 1200+ real mobile devices and browsers. Ship mobile apps and websites that work for everyone, every time… Lisenser kjøpt inn. Ikke gratis
-   Sauce Labs - tester om løsningen fungerer på kjente nettlesere, operativsystem og enheter. Lisenser på gang. Ikke gratis
