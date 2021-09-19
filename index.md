---
layout: home
title: BeLin 6.0 kiadás - főokldal
---
<div class="home">

  <h1 class="page-heading">Friss hírek</h1>

  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <span class="post-meta">{{ post.date | date: "%Y. %B %-d, %a" }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
      </li>
    {% endfor %}
  </ul>

## BeLIn 6.0 kiadás - kezdőlap

Üdvözöljük a BeLIn 6.0 kiadás dokumentációs oldalán!  
  
  

## Miért készült a BeLin és miért pont ez a neve?

A cél az volt, hogy mintegy alternatív lehetőségként a látássérült
felhasználók ki tudják használni a Linux operációs rendszer nyújtotta
lehetőségeket.

Az Ubuntu név a Canonical bejegyzett védjegye, így a kiadásnak más nevet
kellett választani. A BeLin név a Beszélő Linux név rövidítése.

A rendszer számos akadálymentesen használható alkalmazást tartalmaz. Néhány
ezek közül a teljesség igénye nélkül:  
A Firefox webböngészővel kényelmesen internetezhet, az ingyenes Libreoffice
irodai programcsomag segítségével Microsoft Office dokumentumokat,
táblázatokat szerkeszthet és jeleníthet meg, a Pidgin üzenetküldő
alkalmazással számos azonnali üzenetküldő protokoll használatával cseveghet
másokkal, a Thunderbird levelezőprogram segítségével elektronikus leveleket
küldhet és fogadhat, RSS hírcsatornákat böngészhet.

## Melyik Ubuntu verzióra épül a BeLIn 6.0 kiadás?

A BeLIn 6.0 kiadás az Ubuntu 18.04.1 (Bionic Beaver) verziójára épül. Mielőtt
használatba venné az operációs rendszert, érdemes elolvasnia a következő
dokumentumot:

  * [A BeLIn 6.0 kiadás újdonságai](ujdonsagok.html)

## A rendszer első elindítása

Indítsa újra a számítógépét úgy, hogy a DVD már a DVD olvasóban van. A
számítógép a DVD-ről fog elindulni. Előfordulhat, hogy ehhez bizonyos BIOS
beállításokat módosítani kell. Erről részletesebb információkat az alaplaphoz
kapott leírásban vagy az alaplap gyártójának weboldalán találhat.

A számítógép újraindítása után, ha a BIOS beállítások megfelelőek, rövidesen
megjelenik a BeLIn 6.0 kiadás indítómenüje. Az indítómenüben található
menüpontok között a nyílbillentyűkkel mozoghat. Az indítómenü a következő
menüpontokat tartalmazza:

  * A BeLIn 6.0 kiadás kipróbálása az alapértelmezett beállítások használatával: ez az alapértelmezetten kiválasztott menüpont, ilyenkor az Ubuntu kiadásokkal megegyező módon egyetlen speciális kernelparaméter sincs használva az indítási folyamat során. Ha lenyomja az ENTER billentyűt, vagy tíz másodpercen keresztül nem tesz semmit, a live rendszer betöltődése megkezdődik. A bootfolyamat befejeződése után az asztali környezet betöltődik, és elindul az Orka képernyőolvasó.

  * A BeLIn 6.0 kiadás kipróbálása a nomodeset kernelparaméter használatával: egyes Nvidia vagy ATI videokártyák igényelhetik ennek a kernelparaméternek a használatát. Akkor érdemes a BeLIn 6.0 kiadást elindítania ezzel a menüponttal, ha az Ön számítógépén az alaprendszer betöltődése során nem indul el az asztali környezet az alapértelmezett beállítások használatával. Akkor is ezzel a menüponttal kell indítania a BeLIn 6.0 kiadást, ha a számítógépéhez nincs monitor csatlakoztatva.

  * A BeLIn 6.0 kiadás kipróbálása a kompatibilis üzemmód használatával: ha az első két indítási mód nem vezetett eredményre, érdemes elindítania a BeLIn 6.0 kiadást ennek a menüpontnak a használatával is. Ha ezzel a menüponttal indítja el a BeLIn 6.0 kiadást, olyan speciális kernelparaméterek lesznek használva az indítási folyamat során, melyek a legtöbb számítógépnél problémamentes működést eredményeznek.

  * A memória tesztelése: hasznos ez a lehetőség akkor, ha a számítógép működése során rendellenességeket tapasztal, és a számítógépben található memóriamodulokat szeretné tesztelni. A funkció használatához látó segítségre lesz szüksége.

  * Indítás az első merevlemezről: ha ezt a menüpontot választja, a számítógép első merevlemezén található operációs rendszer fog elindulni.

  
  

Ha az alapértelmezett beállítások használatával szeretné kipróbálni a BeLIn
6.0 kiadást, az indítómenü megjelenése után nyomja meg az ENTER billentyűt. A
live rendszer betöltődése ezután megkezdődik. Legyen türelmes, hiszen első
alkalommal az indulás jelentősen hosszabb ideig tarthat, mint a telepítés
után.

### Néhány billentyűparancs a rendszer kipróbálásához

Ha minden rendben volt az indítási folyamat során, akkor a rendszer elindulása
után automatikusan elindul az Orka képernyőolvasó, és az asztalra kerül. Ha
valamilyen oknál fogva nem szólalna meg a képernyőolvasó, a következő
hibaelhárítási lépéseket próbálja meg elvégezni:

Ha a számítógépében lassabb DVD olvasó van, előfordulhat, hogy nem indul el az
Orka képernyőolvasó automatikusan az asztali környezet lassabb betöltődése
miatt. Ha az asztali környezet betöltődése közben hallotta a sikeres
bejelentkezést jelző zenét, de a képernyőolvasó nem szólalt meg, nyomja le az
ALT+F2 billentyűkombinációt, gépelje be az orca --replace parancsot, majd
nyomja le az ENTER billentyűt. A képernyőolvasó ezt követően elindul, és az
asztalra fog kerülni.

Ha az asztali környezet betöltődése közben nem hallott semmilyen zenét, a
BeLin 5.01 kiadás tartalmaz három kiegészítő Orka szkriptet, melyek
segítségével a főhangerővel kapcsolatos beállításokat tudja változtatni. Ha az
Orka képernyőolvasó nem szólalt meg, a következő billentyűparancsokat
használhatja:

  * Főhangerő növelése: ORKA+PAGEUP

  * Főhangerő csökkentése: ORKA+PAGEDOWN

  * Főhangerő némításának változtatása: ORKA+END

Lehetnek olyan hangkártya típusok, melyeknél esetleg a hangerővel kapcsolatos
kiegészítő Orka szkriptek nem működnek megfelelően, például nem változik a
hangerő értéke a megfelelő billentyűparancsra, vagy továbbra is némítva marad
a hang a live rendszer elindításakor.

A BeLIn 6.0 kiadásban lehetősége van arra is, hogy bármikor elindítsa a Hang
beállítóeszközt a STARTGOMB+SHIFT+H billentyűkombináció lenyomásával.

Ha a Hang beállítóeszköz betöltődött, nyomja meg a TAB billentyűt. Ekkor a
némítás jelölőnégyzetre kerül. A Némítás jelölőnégyzet állapotát a SZÓKÖZ
billentyűvel változtathatja meg.

Ha ezt követően egy SHIFT+TAB billentyűkombinációt nyom, a kimeneti hangerő
csúszkájának értékét növelni tudja, ha többször megnyomja a PAGEDOWN
billentyűt.

Ha szeretne egy alkalmazás elindítása után az Asztalra lépni, nyomja le a
STARTGOMB+D billentyűkombinációt. Az asztalon ugyanúgy mozoghat az ikonok
között, mint ahogy a Windows operációs rendszerben már megszokhatta.

Ha szeretné megváltoztatni az Orka képernyőolvasó beállításait, az asztalra
lépés után nyomja le az INZERT+SZÓKÖZ billentyűkombinációt. Ekkor egy
többlapos párbeszédablak jelenik meg, ahol megváltoztathatja a képernyőolvasó
beállításait.

Néhány kényelmi billentyűparancs, melyet csak a BeLin kiadás tartalmaz:

  * STARTGOMB+W: webböngésző elindítása.

  * STARTGOMB+E: levelezőprogram elindítása.

  * STARTGOMB+H: saját felhasználói mappa megnyitása. 

  * STARTGOMB+O: Az Orka képernyőolvasó elindítása. 

  * STARTGOMB+SHIFT+P: Pidgin Üzenetküldő elindítása. 

  * CTRL+ALT+T: parancssor megnyitása (terminál elindítása). 

  * STARTGOMB+G: A Pluma szövegszerkesztő elindítása. 

  * STARTGOMB+R: Libreoffice Szövegszerkesztő elindítása. 

  * STARTGOMB+T: Libreoffice Táblázatkezelő elindítása. 

  * STARTGOMB+B: a Rendszerbeállítások alkalmazás elindítása.

  * STARTGOMB+C: Számológép elindítása.

  * STARTGOMB+DEL: kijelentkezés.

  * STARTGOMB+SHIFT+T: A Hang beállítóeszköz elindítása.

  * STARTGOMB+ALT+H: Az Internetes Rádió Hallgató alkalmazás elindítása.

A következő Orka gyorsbillentyűk néhány plusz funkciót kezelnek, ezek a
funkciók csak a BeLin kiadásokban érhetők el:

  * ORKA+SHIFT+A: ha hordozható számítógépet használ, az Orka képernyőolvasó képes kimondani és kiírni a braille kijelzőre az akkumulátor kapacitását. 

  * ORKA+SHIFT+I: az Információs központ aktiválása. Ez a funkció hasonlít a JAWS For Windows „Kutatás” funkciójához, különböző funkciók segítségével fontos információkhoz juthat hozzá (például részletes időjárás-előrejelzés, TV Műsor, stb).

  * ORKA+T: az Orka képernyőolvasó kimondja és kiírja a braille kijelzőre az aktuális időt. 

  * ORKA+T (kétszer gyorsan megnyomva): az Orka kimondja és kiírja a braille kijelzőre az aktuális dátumot. 

  * ORKA+N: az Orka kimondja és kiírja a braille kijelzőre az aktuális névnapot.

  * ORKA+W: rövidített időjárás-jelentés kimondása a metnet.hu RSS csatorna felhasználásával.

  * ORKA+W kétszer gyorsan lenyomva: teljes elérhető időjárás előrejelzés kimondása a metnet.hu RSS csatorna felhasználásával.

  * ORKA+SHIFT+W: Rövidített ötnapos időjárás előrejelzés kimondása a metnet.hu RSS csatorna felhasználásával. Ekkor csak a hőmérséklet és széladatok kerülnek felolvasásra.

  * ORKA+SHIFT+W kétszer gyorsan megnyomva: Teljes ötnapos időjárás előrejelzés kimondása a metnet.hu RSS csatorna felhasználásával.

  * ORKA+SHIFT+1-5: A szabadon definiált RSS csatorna információinak felolvasása.

  * ORKA+SHIFT+1-5 kétszer gyorsan lenyomva: a szabadon definiált RSS csatorna teljes tartalmának megjelenítése a Firefox webböngészőben.

  * ORKA+SHIFT+É: megjeleníti az értesítések listáját

  * ORKA+0: az utoljára elhangzott értesítés megismétlése

  * ORKA+SHIFT+0: az előző értesítés megjelenítése

  * A beszédsebesség ideiglenes növelése: ORKA+FEL

  * A beszédsebesség ideiglenes csökkentése: ORKA+LE

  * A hangmagasság ideiglenes növelése: ORKA+BAL ALT+FEL

  * A hangmagasság ideiglenes csökkentése: ORKA+BAL ALT+LE

Megjegyzés: az "ORKA" billentyű asztali billentyűzet kiosztásnál az INSERT és
numerikus INSERT, laptop kiosztásnál a CAPS LOCK billentyű.

Ha telepíteni kívánja a BeLIn 6.0 kiadást, az asztalon válassza a „BeLIn 6.0
Telepítése” parancsikont, majd nyomja meg az Enter billentyűt.

## [A rendszer telepítésének leírása](telepites.html)

## További dokumentációk és útmutatók, melyek használatához internet kapcsolat
szükséges

  * [BeLin 5.0 webböngészés és levelezés tananyag (szöveges változat)](/tananyag/BeLin_5.0_Webbongeszes_es_levelezes_tananyag.html)

  * [BeLin 5.0 webböngészés és levelezés tananyag (felolvasott változat)](http://belin.hu/letoltes/BeLin_5.0_tananyag/mp3/tananyag.m3u)

  * [Tudnivaló néhány akadálymentes alkalmazás használatáról](akadalymentes.html)

  * [A Mate asztali környezet alapvető billentyűparancsai](mate_alapveto_billentyuparancsok.html)

  * [Orka billentyűparancsok](orca/commands.html)

  * [Az Orka Képernyőolvasó kézikönyve](orca/index.html)

  * [Ubuntu közösségi dokumentáció](http://wiki.ubuntu.hu/index.php/Kezd%C5%91lap)

  * [Gyakran ismételt kérdések](gyik/gyik.html)

  * [Az OCRFeeder karakterfelismerő alkalmazás bemutatása](ocrfeeder.html)

  * [Az Infoalap Braille-szerkesztő alkalmazás kézikönyve](ibsz/index.html)

  * [A Tilitoli játék magyar nyelvű leírása](tilitoli.html)

  * [Ismert hibák](ismert%20hibak.html)

## Hol kaphatok segítséget?

Ezen dokumentációs oldal mellett akadálymentesítési problémákkal kapcsolatban
mindenki előtt nyitott a BeLin levelezési lista, melyre feliratkozhat az
alábbi címen:  
<http://linux.infoalap.eu/mailman/listinfo/linux_linux.infoalap.eu>

A listaszabályzattal kapcsolatos további tudnivalókért nézze meg a [Gyakran
ismételt kérdések](gyik/gyik.html) című dokumentumot.

Az Infoalap Braille-szerkesztő elkészítését támogatta az Invitech Solutions és
a Magyar Vakok és Gyengénlátók Országos Szövetsége.

  <p class="rss-subscribe"><a href="{{ "/feed.xml" | prepend: site.baseurl }}">Iratkozzon fel az RSS</a> hírcsatornára</p>

</div>

