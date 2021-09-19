---
title: A BeLin 6.0 kiadás újdonságai
layout: page
---
# A BeLin 6.0 kiadás újdonságai

A BeLin 6.0 kiadás akadálymentesítési okokból az Ubuntu 18.04.1-es hosszú
támogatottságú kiadásra épül, az Ubuntu 18.04-es verzió 2023. áprilisáig
támogatott.

A BeLin 6.0 kiadás GNOME alapú változata a 3.28-as verziót, a Mate alapú
változat a Mate asztali környezet 1.20-as verzióját tartalmazza.

  
  

## Újdonságok az akadálymentesítésben

### A legfrissebb Liblouis 3.10.0 verzió

A BeLin 6.0 kiadás lemezképei már a Liblouis Braille megjelenítő komponens
legfrissebb, 3.10.0 verzióját tartalmazzák. Mind a hagyományos irodalmi
Braille megjelenítés, mind a rövid írású Braille megjelenítés
továbbfejlesztésre került a korábbi Liblouis 3.3.0 verzió óta.

  
  

### A legfrissebb Liblouisutdml 7.1-es verzió

A Liblouis összetevő mellett frissült a Liblouisutdml nyílt forráskódú
komponens, mely számos hibajavítást kapott a korábbi 3.7.0 verzió megjelenése
óta. Ezt az összetevőt használja az Infoalap Braille-szerkesztő alkalmazás is.

  
  

### A legújabb Orka képernyőolvasó

A BeLin 6.0 kiadáshoz az Orka Képernyőolvasó legfrissebb, 3.32-es verzióját
tettük elérhetővé. A korábbi BeLin 5.0 alapú kiadásokban a képernyőolvasó
3.26-os verziója volt elérhető, az azóta megjelent új verziók jelentős
fejlődések történtek.

Néhány ezek közül a teljesség igénye nélkül:

  * Tovább fejlődött a 3.26-os verzió óta a Braille-megjelenítés számos alkalmazás használatakor.  
Emellett újdonság még, hogy az Orka most már képes a hosszabb Braille-kijelzőn
megjelenő sorok tördelésére, ha a felhasználó bejelöli az Orka grafikus
Beállítások párbeszédablak Braille lapfülén a Szótörés engedélyezése
jelölőnégyzetet.

  * A webböngészéskor az ARIA párbeszédablakok most már megjelenítésre kerülnek.

  * Tovább fejlődött a webböngészés a Firefox Webböngésző használatakor, tovább fejlődött a MATH ML kifejezések kimondása is.

  * Az Orka Képernyőolvasó számos hibajavítást kapott a 3.26-os verzió óta, melyek a Libreoffice irodai programcsomagot, a Thunderbird levelező klienst, és sok más alkalmazást érintenek.

  * Ha egy felhasználó létrehoz egy új beállítási profilt az Orka grafikus beállítások párbeszédpanelen, és már nincs szüksége az adott felhasználói profilra, a létrehozott profil most már törölhető.

  * Az Orka már rendelkezik egy olyan funkcióval, aminek a segítségével lehetőség van webböngészéskor ideiglenesen váltani az objektum mód és az elrendezés mód között. Ehhez a funkcióhoz alapértelmezetten nincs definiálva billentyűtársítás, de a felhasználó ezt szükség esetén megteheti az Orka grafikus beállítások párbeszédablak billentyűtársítások lapfülén.

  * Az Orka most már rendelkezik egy olyan funkcióval, mely képes kimondani és a Braille-kijelzőn megjeleníteni egy objektum méretét és helyét, képpontokban megadva. Ehhez a funkcióhoz alapértelmezetten nincs definiálva billentyűtársítás, de a felhasználó ezt szükség esetén megteheti az Orka grafikus beállítások párbeszédablak billentyűtársítások lapfülén.  
  
  

### Alapértelmezetten engedélyezett irodalmi braille támogatás

A BeLin 6.0 kiadás használata esetén is az irodalmi braille támogatás
alapértelmezetten engedélyezve lett, és a magyar irodalmi braille tábla az
alapértelmezetten kiválasztott tábla.

### A kurzornál levő szó megjelenítése irodalmi, vagy számítógépes braille
alakban

Alapértelmezetten az Orka képernyőolvasó a Braille kurzornál levő szót
számítógépes Braille alakban jeleníti meg, mely zavaró lehet, ha hosszabb
szövegeket olvas a braille-kijelzőn. Az Orka grafikus beállító párbeszédablak
braille lapfülén a kurzornál levő szó megjelenítése számítógépes braille
alakban jelölőnégyzettel szabályozható, hogy a kurzornál levő szó milyen
formátumban jelenjen meg a kijelzőn. A BeLin 6.0 kiadásban alapértelmezetten
ez a jelölőnégyzet nincs bejelölve, így a kurzornál levő szó is irodalmi
braille alakban jelenik meg, megkönnyítve ezzel a hosszabb szövegek olvasását.

### Gyorsbillentyűk megjelenítése a braille-kijelzőn

Az Orka képernyőolvasó alapértelmezetten nem képes a különböző vezérlőelemek
gyorsbillentyű információit megjeleníteni a braille-kijelzőn. A belin 3.0
kiadásban az Orka grafikus beállító párbeszédablak braille lapfülén a
gyorsbillentyűk megjelenítése jelölőnégyzettel szabályozható, hogy a menük és
vezérlőelemek gyorsbillentyűi megjelenítésre kerüljenek-e. Ez a jelölőnégyzet
alapértelmezetten be van jelölve.

  
  

### Egyszerű akadálymentes Internetes Rádió hallgató alkalmazás

Mivel a korábban használt Radiotray alkalmazás fejlesztése leállt, ezért
kifejlesztésre került egy nagyon egyszerű akadálymentes internetes rádió
hallgatását lehetővé tevő alkalmazás. Az Internetes Rádió Hallgató alkalmazást
az Alkalmazások menü, Internet csoporton belül lehet elindítani az Internetes
Rádió Hallgató parancsikon kiválasztásával, vagy a STARTGOMB+ALT+H
billentyűkombinációval. Az alkalmazás elindítása után a felhasználónak ki kell
csak választania a megfelelő rádióállomást a rendelkezésre álló rádióállomások
közül, majd aktiválnia kell a Lejátszás gombot. Ezt követően a kiválasztott
rádióállomás lejátszásra kerül az Audacious zenelejátszóval.

Az alkalmazás mind a BeLin 6.0 GNOME, mind a BeLin 6.0 Mate alapú kiadásában
megtalálható.

Emellett kompatibilitási okokból megtartásra került a Radiotray internetes
rádió lejátszását lehetővé tevő indikátor is, de a Radiotray csomag
felhasználói kérésre kikerült az alaptelepítésből. Ha valaki mégis szeretné
használni ezt az egyszerű indikátort, a BeLin 6.0 Mate kiadás feltelepítése
után a radiotray csomagot kell csak feltelepítenie.

A Radiotray indikátorhoz is ugyanazok az állomások érhetőek el, mint az
Internetes Rádió Hallgató alkalmazáshoz. A radiotray csomag feltelepítése után
a felhasználónak ki kell jelentkeznie, majd újra be kell jelentkeznie ahhoz,
hogy használni tudja a Radiotray indikátort.

  
  

### Új alkalmazások az alaptelepítésben

A BeLin 6.0 GNOME és Mate alapú kiadások része lett az Audacious zenelejátszó
és a Vlc alkalmazás.

Akadálymentesítési okokból a BeLin 6.0 Mate kiadásból kikerült az
alapértelmezett Videók zenelejátszó, helyette filmek lejátszására használható
a Vlc lejátszó alkalmazás.

Felhasználói kérésre bekerültek még a következő alkalmazások a BeLin 6.0 GNOME
és Mate alapú kiadásokba:

  * A Leafpad szövegszerkesztő,

  * Az Inxi parancssoros rendszer-diagnosztikai program,

  * A Speedtest-cli parancssoros hálózati sebesség mérő program,

  * A Selene Média konvertáló alkalmazás.

  
  

[Vissza a kezdőlapra](index.html)

