---
Title: Laddningstid
Description: Laddningstid
Template: analysis
---

Analys av laddningstid
=======================

Denna rapport handlar om att testa olika webbplatser för att mäta hur snabbt de laddas och om de innehåller några saker som kan förbättras med tanke på laddningstid och användbarhet.

Urval
-----------------------

Jag fortsätter i samma linje med urvalet från föregående rapport, dvs Polisen, Försäkringskassan och Skatteverket.

<div class="screen-shots">
    <img src="../image/polisen_page.png?w=600" alt="Skärmdump från polisen.se">
    <img src="../image/forsakringskassan_page.png?w=600" alt="Skärmdump från www.forsakringskassan.se">
    <img src="../image/skatteverket_page.png?w=600" alt="Skärmdump från skatteverket.se">
</div>

Metod
-----------------------

Jag har avnänt mig av Google Pagespeed som är ett bra verktyg för utvecklare att använda sig av för analysera sina webbplatser och få tips och råd på hur man kan optimera dem och få dem att laddas snabbare.

Jag har även använt mig av "devtools"-fliken i Chrome för att se vilka resurser som laddas in och hur lång tid det tar.

Jag har sammanställt mina mätresultat i dokumentet här nedan.

Resultat
-----------------------

<div class="spread-sheet">
    <iframe title="Sammanställning av mätvärden" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQbWp_Lb4wqZUNrahzYNkmocob1tPd_TCiZxtaI2QpBnjO8tGyDPYELMwQD6tJkDuO-5BY1KGhbZFU-/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false"></iframe>
</div>


Analys
-----------------------

Som vi kan se av mätningarna så vinner Polisens webbplats då den har i särklass bästa betyg i alla kategorier och snabbast laddningstid. På delad sistaplats kommer Försäkringskassan och Skatteverket. Jag har reflekterat över hur detta kan komma sig. Jag har en teori om att Polisen sida mest presenterar information medan de övriga sidorna har mer interaktiv funktionalitet när det gäller att exempelvis logga in och sköta olika ärenden.

Det man kan se är att de långsammare sidorna laddar in betydligt mer resurser allt ifrån CSS till bilder och JS. De rekommendationerna som Google Pagespeed rekommenderar och som jag kommer att försöka ta med mig framöver är att försöka fokuserna på att prioritera den första renderingen av sidan dvs att infoga nödvändig JS-/CSS-kod direkt på sidan och skjuta upp inläsningen av JS-kod/formatmallar som är mindre viktiga. Försäkringskassans webbplats skulle uppskattningsvis kunna spara 1,52 sekunder och Skatteverket 1,35 sekunder på detta enligt Google Pagespeed. Polisen däremot hade bara en uppskattad besparing på 0,14 sekunder. 

Vad gäller gräns för absolut laddningstid så skulle jag nog säga att min gräns går vid en sekund, därefter tycker jag att det går trögt. Jag vet att många andra kan ha en tolerans upp emot tre sekunder men jag håller inte riktigt med där, otålig som jag är. Här är det bara Polisen som klarar min gräns.

Referenser
-----------------------
https://pagespeed.web.dev/

https://polisen.se

https://www.forsakringskassan.se

https://skatteverket.se

Övrigt
-----------------------
Jag har varit ensam vid framtagande av denna rapport.