# 🎓 Pedagógiai ötletből interaktív taneszköz

## Módszertani segédlet

Ez a segédlet abban támogat, hogy **programozói és játéktervezői előismeretek nélkül**, a saját tanórai céljaidból kiindulva készíts mobilbarát, böngészőben futó digitális taneszközöket az AI segítségével.

### 🧩 Hogyan gondolkodj taneszköz-tervezőként?

Egy jó digitális taneszköz tervezése pont olyan, mint egy **óravázlat** elkészítése. Neked csak a **pedagógiai célt és a tananyagot** kell hoznod – a játékmechanika kitalálását és a programozást bízd az AI-ra!

A folyamat 3 egymásra épülő rétegből áll – **neked csak az elsőt kell hoznod, a másik kettőt az AI építi rá:**

1. **🎯 Tartalom és pedagógiai cél *(A te szaktárgyi tudásod)*** – Mit kell megtanulniuk vagy begyakorolniuk a diákoknak, és milyen konkrét példákon, fogalmakon keresztül?

2. **🏗️ Játéktípus *(A keret)*** – Milyen struktúra illik legjobban ehhez a tananyaghoz (pl. párosító, sorrendbe rakó, hibakereső)?

3. **⚙️ Játékmenet *(A dinamika)*** – Mit csinál pontosan a diák a képernyőn, és milyen visszajelzést kap jó vagy rossz válasz esetén?

Ha nemcsak egy működő kvízt szeretnél, hanem tudatosan terveznéd meg a diákok tanulási élményét is, érdemes az **MDA-keretrendszer** (*Mechanics – Dynamics – Aesthetics*) logikáját követni:

* **1. Szabályok és mechanikák (Mechanics):** A játék elemi építőkövei (pl. időkorlát, 3 élet, pontozás, kártyahúzás, sorrendbe állítás). Ezeket írod le a promptban.

* **2. Játékmeneti dinamika (Dynamics):** Ami a szabályok és a diák döntéseinek találkozásából születik (pl. az időnyomás gyors reflexekre ösztönöz; a limitált életek megfontoltságra nevelnek a vaktában tippelgetés helyett).

* **3. Pedagógiai hatás és élmény (Aesthetics):** A végső kognitív és érzelmi cél (pl. a felfedezés öröme, a flow-állapot elérése, vagy a biztonságos, tét nélküli hibázás élménye).

#### 🔄 Visszacsatolási hurkok (Feedback Loops) az osztályteremben

Egy jó oktatójáték kétféle visszacsatolással tartja egyensúlyban a nehézséget (Flow-csatorna):

* **Negatív visszacsatolás (Felzárkóztatás és differenciálás):** Ha a diák hibázik, a rendszer nemcsak piros X-et ad, hanem segít (pl. ad egy rávezető tippet, vagy a hibás kártyát visszateszi a pakli végére, hogy később újra találkozzon vele).

* **Pozitív visszacsatolás (Motiváció fenntartása):** Sorozatos jó válaszoknál (kombó) vizuális megerősítést ad, vagy megnyit egy nehezebb bónusz kihívást.

### 🗺️ Pedagógiai fordítókulcs (LM-GM mátrix): Milyen célhoz milyen játék illik?

A táblázat a Bloom-taxonómia kognitív szintjei szerint rendezi a pedagógiai célokat és a hozzájuk illő játékmechanikákat. Keresd ki a tanórai célodat!

| Kognitív szint (Bloom) | Pedagógiai cél (Amit a tanár tud) | Ajánlott játéktípus | Játékmenet lényege és mechanikai fókusz | 
| ----- | ----- | ----- | ----- | 
| **1. Felidézés & Megértés** | Fogalmak, szakszavak, évszámok rögzítése | Kártyapárosító / Memória | Két oszlopban kattintással összeköthető párok, azonnali visszajelzéssel. | 
| **1. Felidézés & Megértés** | Gyorsaság, automatizálás, reflexszerű tudás | Villámkvíz (Time Attack) | Minél több helyes válasz megadása 60 mp alatt, folyamatos kombó-pontozással (*időnyomás*). | 
| **1. Felidézés & Megértés** | Idegen szavak, kulcsfogalmak helyesírása | Akasztófa / Szókitaláló | Fogalmak betűnkénti kitalálása korlátozott próbálkozással, vizuális visszajelzéssel. | 
| **1. Felidézés & Megértés** | Fogalmak felidézése meghatározások alapján | Keresztrejtvény / Szókereső | Rácsban elrejtett kulcssavak megkeresése vagy beírása a megadott definíciók alapján. | 
| **2. Alkalmazás** | Szövegértés, definíciók használata kontextusban | Lyukas szöveg (Cloze test) | Hiányzó szavak behelyettesítése egy szövegbe egy megadott szóbankból kattintással. | 
| **2. Alkalmazás** | Kritikus olvasás, hibajavítás, szabályalkalmazás | Hibakereső (Debug / Lektor) | Egy hibás szövegben, képletben vagy kódrészletben kell rákattintani a hibás elemekre. | 
| **2. Alkalmazás** | Térképi tájékozódás, ábrák és részek azonosítása | Címkéző (Hotspot / Képfelismerő) | Egy ábra vagy térkép megjelölt pontjaira kattintva kell kiválasztani a megfelelő megnevezést. | 
| **3. Elemzés & Rendszerezés** | Folyamatok, időrend, hierarchia gyakorlása | Sorrendbe rakó (Idővonal) | Összekevert lépések/események rendezése fel/le gombokkal a helyes sorrendig. | 
| **3. Elemzés & Rendszerezés** | Kategorizálás, tulajdonságok szétválogatása | Kétirányú válogató | Középen megjelenik egy állítás vagy kép, a diák két gomb közül választ (pl. *Igaz / Hamis*). | 
| **3. Elemzés & Rendszerezés** | Összetettebb rendszerezés több szempont szerint | Többirányú válogató (Kosárba rakó) | Megjelenő elemek szétválogatása 3-4 különböző gyűjtődobozba (pl. *emlősök, hüllők, madarak*). | 
| **3. Elemzés & Rendszerezés** | Gyors felismerés, kivételek keresése | Kakukktojás-kereső | 4-6 elem közül ki kell választani azt az egyet, amelyik nem illik a sorba, majd elolvasni az indoklást. | 
| **3. Elemzés & Rendszerezés** | Összefüggések keresése, mintafelismerés | Kategória-mátrix (Connections) | 16 összekevert fogalomból kell négy darab 4-es tematikus csoportot alkotni kattintással. | 
| **4. Értékelés & Problémamegoldás** | Tudásszint felmérése, fokozatos mélyítés | Lépcsőzetes kvíz (Milliomos) | Egyre nehezedő kérdések segítségekkel (pl. felező), ahol egy hiba megszakítja a sorozatot. | 
| **4. Értékelés & Problémamegoldás** | Ok-okozati összefüggések, döntéshozatal | Szituációs döntéshozó | Helyzetleírás + 2-3 választási lehetőség, ahol minden döntés megváltoztat egy mérőszámot (*erőforrások*). | 
| **4. Értékelés & Problémamegoldás** | Komplex problémamegoldás, logikai láncolatok | Szabadulószoba (Mini Escape Room) | 3-4 egymásra épülő logikai feladvány, amelyek megoldása egy-egy számjegyet ad a végső lakatkódhoz. | 

### 📋 Hogyan építsd be az óravázlatodba?

Az elkészült digitális taneszköz nem önmagában álló érdekesség, hanem a **standard óravázlatod „Eszközök” oszlopának legrugalmasabb eleme**, amelyre komplett órai stratégiát építhetsz:

| Óravázlat oszlopai | Hogyan tölti meg tartalommal a saját taneszköz? | 
| ----- | ----- | 
| **Eszközök** | Saját készítésű mobilbarát webalkalmazás (QR-kóddal vagy rövid linkkel kivetítve), okostelefonok. | 
| **Munkaformák** | **Egyéni munka** (saját tempójú gyakorlás, pl. *Villámkvíz*), **páros munka** (közös érvelés és döntés, pl. *Szituációs játék*), vagy **csoportverseny** (pl. *Mini Escape Room* kódjának közös megfejtése). | 
| **Módszerek** | Gamifikáció (játékosítás), azonnali visszacsatoláson alapuló formatív értékelés, felfedeztető tanulás, differenciálás. | 
| **Tanári tevékenység** | **Facilitálás és megfigyelés**: a folyamat elindítása, a hibás válaszokból adódó tipikus tévképzetek kiszűrése és célzott megbeszélése. | 
| **Diáktevékenység** | Aktív interakció, próbálkozás és hibázás kockázat nélkül, azonnali önellenőrzés, a játékszabályokból adódó logikai következtetés. | 

> 💡 **Tipp a differenciáláshoz:** Mivel a kód a tiéd, ugyanannak a játékmotornak készíthetsz egy *alap* és egy *haladó* (pl. nehezebb fogalmakat vagy kevesebb életet adó) verziót is. Két külön QR-kóddal oszthatod ki őket az osztályban, így mindenki a saját szintjén haladhat.

### 🚀 Kétlépcsős munkafolyamat az AI-val

Ne próbálj meg elsőre tökéletes kódot kérni, ha még bizonytalan vagy a játék működésében! Használd ezt a két lépést:

#### 1. Lépés: Játékmechanika tervezése (Ötletelő prompt)

Másold be ezt a promptot az AI-nak, töltsd ki a `[szögletes zárójeles]` részeket, és válassz a felkínált ötletek közül!

```
Viselkedj tapasztalt oktatástechnológiai játéktervezőként! 
Az alábbi tananyagot szeretném interaktív, mobilon is könnyen játszható digitális taneszközzé alakítani:
- Tantárgy és téma: [pl. Történelem – Az 1848–49-es forradalom főbb eseményei]
- Korosztály: [pl. 7. osztály, 13 évesek]
- Pedagógiai cél: [pl. Az események időrendi sorrendjének és helyszíneinek rögzítése]

Javasolj 3 különböző, egyszerűen megvalósítható játékmechanikát ehhez a tananyaghoz! 
Mindegyiknél írd le röviden:
1. Mi a játék neve és lényege?
2. Mit lát és mire kattint a diák a képernyőn?
3. Mi történik jó és rossz válasz esetén?
4. Hogyan segíti a játék a lemaradó diákokat (pl. tippek, újbóli próbálkozás), és hogyan tartja fenn a gyorsabbak motivációját?

Még ne írj kódot, csak a 3 koncepciót mutasd meg, hogy kiválaszthassam a legjobbat!
```

#### 2. Lépés: A kész taneszköz legenerálása (Kivitelező prompt)

Miután kiválasztottad a legszimpatikusabb ötletet (vagy már eleve tudod, mit szeretnél), használd ezt a sablont a kész `index.html` fájl elkészítéséhez:

```
Készíts egy interaktív, böngészőben futó oktatójátékot egyetlen önálló HTML-fájlban (index.html), amely tartalmazza a teljes HTML, CSS és JavaScript kódot is, mindenféle külső fájl vagy telepítés nélkül.

A taneszköz adatai:
- Tantárgy és témakör: [pl. Biológia – Az emberi emésztőrendszer részei]
- Célcsoport / életkor: [pl. 7. osztályos diákok, 13-14 évesek]
- Pedagógiai cél: [pl. A szervek sorrendjének és fő feladatainak rögzítése]

Tartalom (ezeket használd a játékban):
  1. [Elem 1 - pl. Nyelőcső: Továbbítja a falatot a gyomorba]
  2. [Elem 2 - pl. Gyomor: Savas közegben bontja a fehérjéket]
  3. [Elem 3 - pl. Vékonybél: Itt történik a tápanyagok felszívódása]
  (Adj meg legalább 6-8 elemet vagy kérdést!)

Játékmechanika és működés:
- Játéktípus: [pl. Kártyapárosító / Idővonal-rendező / Kétirányú válogató]
- Játékmenet: [Ide másold be az 1. lépésben kiválasztott játékmenetet, vagy írd le röviden, mire kattint a diák!]
- Visszajelzés és hibakezelés: [pl. Hibás válasz esetén mutasson egy rövid segítő magyarázatot, és tegye vissza a kérdést a kör végére / Legyen 3 élet és kombó-pontozás]

Design és technikai követelmények:
- Legyen 100%-ban reszponzív, okostelefonon álló nézetben is kényelmesen nyomkodható (nagy gombok, olvasható betűk, kattintás alapú irányítás a húzd-és-ejtsd helyett).
- Legyen barátságos, modern, diákbarát a látványvilága (használj releváns emojikat is).
- Tartalmazzon pontszámlálót vagy előrehaladás-jelzőt, a végén pedig egy összegző képernyőt "Újrajátszás" gombbal (ami megkeveri az elemeket).
- A kód legyen átlátható és jól kommentezett, hogy a tananyag (a szópárok/kérdések listája) később egyetlen helyen, könnyen átírható legyen a kódban.
- Kizárólag a teljes, azonnal bemásolható HTML-kódot add vissza!
```

### 💡 3 aranyszabály a kipróbáláshoz

1. **Mindig teszteld mobilon!** A diákok többsége telefonon nyitja meg a QR-kódot vagy a linket. Ha valami túl apró vagy lelóg a képernyőről, írd vissza az AI-nak: *"Tedd nagyobbá a gombokat és igazítsd a nézetet álló mobilképernyőhöz!"*

2. **Ne félj finomítani!** Az első verzió csak egy kiindulópont. Bátran kérj módosításokat: *"Adj hozzá minden jó válasz után egy 1 mondatos magyarázatot!"* vagy *"Ha a diák hibázik, tegye vissza a kérdést a sor végére, hogy újra gyakorolhassa."*

3. **Használd újra a kódot!** Ha egy játékmechanika bevált, nem kell újraprogramoztatni: nyisd meg a GitHubon az `index.html` fájlt, keresd meg a kód elején a szavakat/kérdéseket tartalmazó listát, és írd át őket a következő óra anyagára!