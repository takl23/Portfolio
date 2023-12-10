---
Title: Webbplatsers laddningstid och användbarhet
Description: This is my report page about websites' loading time and usability
Template: report
---

# Webbplatsers laddningstid och användbarhet

I denna rapport har webbplatsers laddningstid och användbarhet analyserats. I analysen har det testats mot hur snabbt de laddar om i analysen har det även kikats på förbättringar med avseende på laddningstid och användbarhet.


Urval
-----------------------

Urvalet i denna studie är baserad på samma urval som är gjord i studien [Webbplatsers färgval och känslan de signalerar][01] där webbplatser har valts som de flesta i Sverige känner igen. Urvalet har landat på en myndighetssida, [Försäkringskassan][02], en streaming sida, [SVT play][03] och en e-handelssida, [H&M][04]. 

Metod
-----------------------
Följande webbläsare har använts vid analys:
[Firefox Develeoper verison 120.0b9 64-bit][05]

I analysen har inspekteringsverktyget används i vald webbläsare för studien där data hämtats i fliken Nätverk. Parametrar som var av intresse var "DOM Content Loaded" som visar tid då heal DOM trädet lästs in och "load" som visar tiden det tar då allt har lästs in så som stylesheets, scripts, bilder etcetera . Även överförd mängd bokfördes.

För att utvärdera användarvänlighet och förbättringsförslag har [PageSpeed Insights][06] använts. För att läsa mer i detalj om hur detta verktyg funkar så följ länken [About PageSpeed Insights][07].

Resultat
-----------------------
Nedan presenteras mätvärdena samt skärmklipp på webbplatserna som analyserats.

### Mätvärden

<div class="container">

<iframe class="responsive-iframe" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vTwcMR7e1aCDIDXtvrTi4trVdtsfpU0ys8jNui4gpXEHldZxHwzBKX6FQoRQNIMDyU1SVlOGpGN8vAb/pubhtml?widget=true&amp;headers=false" title="Mätvärdern laddningstider på en hemsida"></iframe>

</div>

### Försäkringskassan
![forsakringskassan_Screenshot](../image/forsakringskassan_Screenshot.png "forsakringskassan_Screenshot")
 
 Lägst poäng i PageSpeed Insights får Försäkringskassan på prestanda både för desktop, men framförallt mobila enheter. Övriga parametrar har höga poäng. Förbättring för denna webbplats är att fokusera på att ta bort resurser som blockerar renderingen och hantering av bildelement där det saknas width och height på sina ställen.
 
### SVT Play
![SVT_Screenshot](../image/SVT_Screenshot.png "SVT_Screenshot")

För SVT är det prestandan som får lägst poäng i PageSPeed Insights där både mobila enheter och desktop har låg poäng. Övriga parametrar har höga poäng. Förbättringar för denna webbplats är att minsak arbetsbelastning på modertråden, minska körtiden för JavaScript och reducera JavaScript och CSS som inte används och använda bilder med rätt storlek.

### H&M
![HM_Screenshot](../image/HM_Screenshot.png "HM_Screenshot")

H&Ms hemsida får låga poäng på prestanda för både mobila enheter och desktop. Övriga parametrar har höga poäng. Förbättringar som kan föras är att reducera JavaScript som inte används, minska serverns första svarstid, minska arbetsbelastningen på moder tråden och hantering av bildelement där det saknas width och height på sina ställen. PageSpeed Insight uppmanar också till att undvik ett onödigt stort DOM-träd.


Analys
-----------------------
Det man kan säga för alla tre hemsidor så är det prestandan som alla har lägst poäng på där H&M sticker ut markant.
Generellt för alla hemsidor verkar det som att förbättring går att göra på Javascript och CSS biten där det har föreslagits att reducera kod som inte används. Återkommande har också varit att alla bilder inte har "width och height" vilket är en enkel åtgärd att göra för att förbättra prestanda. 

H&M som var den sidan som fick absolut lägst prestanda poäng kan man även nämna att prestandan går att förbättra genom att minska DOM-trädet, men frågan är om det går då denna sidas ändamål ska sälja kläder och då kan man ju tänka sig att DOM-trädet kommer innehålla många bilder. 

Tittar vi bara på alla värden i tabellen ovan så måste man ändå säga att snitt både från PageSpeed Insights samt mätningar som är gjorda med inspeteringsverktyget så tycker jag att Försäkringskassan är den som presterat bäst, men dessa sidor är helt olika typer av sidor så ska man vara lite kritisk så kan man inte riktigt jämföra sidorna mot varandra utan urvalet borde göras om där likvärdiga sidor ställs mot varandra. 

Generellt så väljer man att sitta på en desktop som har en större skärm när man ska skicka in myndighetsärenden, vilket jag också tycker yttrar sig i att Försäkringskassan får ett betydligt högre prestanda värde på just desktopanalysen. Att H&M, men även SVT-play får ganska låga värden på prestandapoäng från PageSpeed Insights men även längre laddningstider på parametern "load" och "DOM Content Loaded" tror jag beror på att det innehåll dom behöver ladda in på sin sida är betydligt tyngre, bilder och video, vilket inte är fallet för Försäkringskassan som framförallt behöver tillhandahålla information. 

Jag tycker att det är svårt att säga en absolut laddningstid som jag uppfattar som snabb eller långsam för en webbplats baserat på de tre webbplatser jag analyserat. Har aldrig riktigt funderat i dessa banor. Har använt alla dessa siter och aldrig tidigare tänkt på laddningstiden. Så med det sagt får absolut laddningstid som jag uppfattar som långsam vara baserad på data med hög laddningstid (3,86sekunder). Jag säger att allt över 4 sekunder är långsamt. Rätt eller fel det vet jag inte. Beror nog på hur bråttom man har. 

Referenser
-----------------------

<i>Referenser senast kontrollerade 2023-11-30.</i>

[01]: http://www.student.bth.se/~takl23/dbwebb-kurser/design/me/portfolio/analysis/01_colors

[02]: https://www.forsakringskassan.se/

[03]: https://www.svtplay.se/

[04]: https://www2.hm.com/sv_se/index.html

[05]: https://www.mozilla.org/en-US/firefox/120.0beta/releasenotes/?utm_source=firefox-browser&utm_medium=firefox-desktop&utm_campaign=about-dialog

[06]: https://pagespeed.web.dev/?utm_source=psi&utm_medium=redirect

[07]: https://developers.google.com/speed/docs/insights/v5/about

<b>Webbplatsers färgval och känslan de signalerar </b>: http://www.student.bth.se/~takl23/dbwebb-kurser/design/me/portfolio/analysis/01_colors

<b>Försäkringskassan</b>: https://www.forsakringskassan.se/

<b>SVT play</b>: https://www.svtplay.se/

<b>H&M</b>: https://www2.hm.com/sv_se/index.html

<b>Firefox Develeoper verison 120.0b9 64-bit</b>: https://www.mozilla.org/en-US/firefox/120.0beta/releasenotes/?utm_source=firefox-browser&utm_medium=firefox-desktop&utm_campaign=about-dialog 

<b>PageSpeed Insights </b>: https://pagespeed.web.dev/?utm_source=psi&utm_medium=redirect

<b>About PageSpeed Insights</b>: https://developers.google.com/speed/docs/insights/v5/about


Övrigt
-----------------------

Tamara Kljajic deltog i att författa rapporten (takl23).