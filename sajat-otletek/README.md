# 🎓 Pedagógiai ötletből interaktív taneszköz 
## Módszertani segédlet

Ez a segédlet abban támogat, hogy **programozói és játéktervezői előismeretek nélkül**, a saját tanórai céljaidból kiindulva készíts mobilbarát, böngészőben futó digitális taneszközöket az AI segítségével.

---

### 🧩 Hogyan gondolkodj taneszköz-tervezőként?

Egy jó digitális taneszköz tervezése pont olyan, mint egy **óravázlat** elkészítése. Neked csak a **pedagógiai célt és a tananyagot** kell hoznod – a játékmechanika kitalálását és a programozást bízd az AI-ra!

A folyamat 3 építőelemből áll:
1. **A) Játéktípus** *(Mi a keret?)*
2. **B) Játékmenet** *(Mit csinál pontosan a diák?)*
3. **C) Tartalom** *(A te szaktárgyi tudásod és tananyagod)*

---

### 🗺️ Pedagógiai fordítókulcs: Milyen célhoz milyen játék illik?

Ha nem tudod, milyen játékot kérj az AI-tól, keresd ki a táblázatból a tanórai célodat!

| Pedagógiai cél (Amit a tanár tud) | Ajánlott játéktípus (A) | Játékmenet lényege (B) |
| :--- | :--- | :--- |
| Fogalmak, szakszavak, évszámok rögzítése | Kártyapárosító / Memória | Két oszlopban kattintással összeköthető párok, azonnali visszajelzéssel. |
| Folyamatok, időrend, hierarchia gyakorlása | Sorrendbe rakó (Idővonal) | Összekevert lépések/események rendezése fel/le gombokkal a helyes sorrendig. |
| Kategorizálás, tulajdonságok szétválogatása | Kétirányú válogató | Középen megjelenik egy állítás vagy kép, a diák két gomb közül választ (pl. *Igaz / Hamis* vagy *Savas / Lúgos*). |
| Ok-okozati összefüggések, döntéshozatal | Szituációs döntéshozó | Rövid helyzetleírás + 2-3 választási lehetőség, ahol minden döntés megváltoztat egy mérőszámot (pl. *erőforrás, elégedettség*). |
| Gyors felismerés, kivételek keresése | Kakukktojás-kereső | 4-6 elem közül ki kell választani azt az egyet, amelyik nem illik a sorba, majd elolvasni az indoklást. |
| Szövegértés, definíciók és kulcsszavak használata | Lyukas szöveg (Cloze test) | Hiányzó szavak behelyettesítése egy szövegbe egy megadott szóbankból kattintással. |
| Idegen szavak, kulcsfogalmak helyesírása | Akasztófa / Szókitaláló | Fogalmak vagy szavak betűnkénti kitalálása korlátozott próbálkozással, vizuális visszajelzéssel. |
| Fogalmak felidézése meghatározások alapján | Keresztrejtvény / Szókereső | Rácsban elrejtett kulcsszavak megkeresése vagy beírása a megadott definíciók alapján. |
| Összefüggések keresése, rendszerező gondolkodás | Kategória-mátrix (Connections) | 16 összekevert fogalomból kell négy darab 4-es tematikus csoportot alkotni kattintással. |
| Térképi tájékozódás, ábrák és részek azonosítása | Címkéző (Hotspot / Képfelismerő) | Egy ábra vagy térkép megjelölt pontjaira kattintva kell kiválasztani a megfelelő megnevezést. |
| Összetettebb rendszerezés több szempont szerint | Többirányú válogató (Kosárba rakó) | Megjelenő elemek szétválogatása 3-4 különböző gyűjtődobozba (pl. *emlősök, hüllők, madarak*). |
| Kritikus olvasás, hibajavítás, szabályalkalmazás | Hibakereső (Debug / Lektor) | Egy hibás szövegben, képletben vagy kódrészletben kell rákattintani a hibás elemekre. |
| Tudásszint felmérése, fokozatos mélyítés | Lépcsőzetes kvíz (Milliomos) | Egyre nehezedő kérdések segítségekkel (pl. felező), ahol egy hiba megszakítja a sorozatot. |
| Gyorsaság, automatizálás, reflexszerű tudás | Villámkvíz (Time Attack) | Minél több helyes válasz megadása 60 másodperc alatt, folyamatos kombó-pontozással. |
| Komplex problémamegoldás, logikai láncolatok | Szabadulószoba (Mini Escape Room) | 3-4 egymásra épülő logikai feladvány, amelyek megoldása egy-egy számjegyet ad a végső lakatkódhoz. |

---

### 🚀 Kétlépcsős munkafolyamat az AI-val

Ne próbálj meg elsőre tökéletes kódot kérni, ha még bizonytalan vagy a játék működésében! Használd ezt a két lépést:

#### 1. Lépés: Játékmechanika tervezése (Ötletelő prompt)
Másold be ezt a promptot az AI-nak, töltsd ki a `[szögletes zárójeles]` részeket, és válassz a felkínált ötletek közül!

```text
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

Még ne írj kódot, csak a 3 koncepciót mutasd meg, hogy kiválaszthassam a legjobbat!
```

---

#### 2. Lépés: A kész taneszköz legenerálása (Kivitelező prompt)
Miután kiválasztottad a legszimpatikusabb ötletet (vagy már eleve tudod, mit szeretnél), használd ezt a sablont a kész `index.html` fájl elkészítéséhez:

```text
Készíts egy interaktív, böngészőben futó oktatójátékot egyetlen önálló HTML-fájlban (index.html), amely tartalmazza a teljes HTML, CSS és JavaScript kódot is, mindenféle külső fájl vagy telepítés nélkül.

A taneszköz adatai:
- Tantárgy és témakör: [pl. Biológia – Az emberi emésztőrendszer részei]
- Célcsoport / életkor: [pl. 7. osztályos diákok, 13-14 évesek]
- Pedagógiai cél: [pl. A szervek sorrendjének és fő feladatainak rögzítése]

Játékmechanika és működés:
- Játéktípus: [pl. Kártyapárosító / Idővonal-rendező / Kétirányú válogató]
- Játékmenet: [Ide másold be az 1. lépésben kiválasztott játékmenetet, vagy írd le röviden, mire kattint a diák!]
- Tartalom (ezeket használd a játékban):
  1. [Elem 1 - pl. Nyelőcső: Továbbítja a falatot a gyomorba]
  2. [Elem 2 - pl. Gyomor: Savas közegben bontja a fehérjéket]
  3. [Elem 3 - pl. Vékonybél: Itt történik a tápanyagok felszívódása]
  (Adj meg legalább 6-8 elemet vagy kérdést!)

Design és technikai követelmények:
- Legyen 100%-ban reszponzív, okostelefonon álló nézetben is kényelmesen nyomkodható (nagy gombok, olvasható betűk, kattintás alapú irányítás a húzd-és-ejtsd helyett).
- Legyen barátságos, modern, diákbarát a látványvilága (használj releváns emojikat is).
- Tartalmazzon pontszámlálót vagy előrehaladás-jelzőt, a végén pedig egy összegző képernyőt "Újrajátszás" gombbal (ami megkeveri az elemeket).
- A kód legyen átlátható és jól kommentezett, hogy a tananyag (a szópárok/kérdések listája) később egyetlen helyen, könnyen átírható legyen a kódban.
- Kizárólag a teljes, azonnal bemásolható HTML-kódot add vissza!
```

---

### 💡 3 aranyszabály a kipróbáláshoz

1. **Mindig teszteld mobilon!** A diákok többsége telefonon nyitja meg a QR-kódot vagy a linket. Ha valami túl apró vagy lelóg a képernyőről, írd vissza az AI-nak: *"Tedd nagyobbá a gombokat és igazítsd a nézetet álló mobilképernyőhöz!"*
2. **Ne félj finomítani!** Az első verzió csak egy kiindulópont. Bátran kérj módosításokat: *"Adj hozzá minden jó válasz után egy 1 mondatos magyarázatot!"* vagy *"Legyen benne 3 élet (szív), ami hibánál elfogy."*
3. **Használd újra a kódot!** Ha egy játékmechanika bevált, nem kell újraprogramoztatni: nyisd meg a GitHubon az `index.html` fájlt, keresd meg a kód elején a szavakat/kérdéseket tartalmazó listát, és írd át őket a következő óra anyagára!
