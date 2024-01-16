Hemsidor analys av laddningstider och användbarhet
=======================

Urval
-----------------------

Wowhead, Warcraftlogs och Raider.io. Jag valde dessa sidor eftersom jag själv använder dem ofta och de har alla ett gemensamt tema eller snarare gemensam inriktning/målgrupp samt att jag använde dessa sidor i kmom04.

Metod/verktyg
-----------------------
Pagespeed

<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQgJjAPq1N5DWkfnNg3oPDNnAfKNdRPuWCSnoh3w8ppOQVv2vzMQNI2ji-q_R-BBEYoNoAdtu26WLuJ/pubhtml?widget=true&amp;headers=false"></iframe>

Resultat
-----------------------
![Wowhead](%assets_url%/img/wowhead.jpg)
![Warcraftlogs](%assets_url%/img/warcraftlogs.jpg)
![Raiderio](%assets_url%/img/raiderio.jpg)

Wowhead
Hemsidan är väldigt illa uppgyggd för mobila enheter då den inte passerar pagespeeds test (failed) vilket man också kan bekräfta efter att besökt hemsida genom en mobil enhet, sidan är långsam vilket också bekräftas genom pagespeed 
(First Contentful Paint: 7.8s). Något som jag bara kan spekulera till att vara anledningen är den stora mängd requests hemsidan gör varje gång den laddas (average 157st requests).

Warcraftlogs
Hemsidan hade inte samma problem som föregående (wowhead) när jag kollade genom networkstabben och därför kan jag inte riktigt påpeka vad sidan skulle kunna göra bättre utöver att den fick underkänt av pagespeed.

Raiderio
Hemsidan fick underkänt i både mobil samt desktop versionen i Pagespeed något jag anar beror på den stora mängd resource requests som sker varje gång man laddar sidan (256 average) lite samma problem som Wowhead.

Analys
-----------------------

Den mest framstående förbättringsåtgärden för sidorna verkar för mig generellt vara antalet resource requests som sker vid varje hämtning av hemsidan. Vad jag skulle kunna tro är många av dessa requests är för reklam (även om jag blockerar reklam i min webbläsare) specifikt då jag sedan inna är medveten om att samtliga sidor har väldigt aggresiv popup reklam (om man inte väljer att blockera det).

Rangordning
-----------------------

#1 Warcraftlogs
#2 Raiderio
#3 Wowhead

Min motivering för ovanstående rankning är framförallt baserad på helhetsintrycket av samtliga resultat i min google/excell. Warcraftlogs har lägst antal requests som sker i varje omladdning av hemsidan och har även den lägsta genomsnittliga laddningstiden. Att rangordna nummer två och nummer tre är lite svårare, raiderio har en avsevärt mycket längre laddningstid vid vaje omladdning och mer requests men har en stabil rankning i pagespeed över både desktop och mobil vilket jag bedömmer är viktigare, speciellt om man testar att använda Wowhead på en mobil enhet (ingen trevlig upplevelse). 

Genrellt upplever jag inte någon skillnad i verklig användning på dessa laddningstider och anser inte att de har någon positiv eller negativ bemärkelse egentligen, men då jag saknar annnan data att rangordna hemsidorna på så får rankningen stå fast. 
Förmodligen är det andra aspekter som gör exempelvis Wowhead till en dålig hemsida på mobilenheter (den känns trög, hänger sig och har ingen bra layout för mindre skärmar).

Övrigt
-----------------------

Adam Grimmehed