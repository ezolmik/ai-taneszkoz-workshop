# Csoportosító játék – generáló prompt

```markdown
Készíts egyszerű szófaj szerinti csoportosító gyakorlójátékot
felső tagozatos diákoknak!

A játék címe: „Melyik csoportba tartozik?”

A feladat: sorold a szavakat három csoportba:
főnév, melléknév, ige!

Ezeket az egyértelmű példákat használd:
- Főnév: kutya, ceruza, erdő, barátság
- Melléknév: piros, vidám, puha, savanyú
- Ige: fut, olvas, nevet, alszik

A játék működése:
- Egyszerre egy szó jelenjen meg, jól olvasható kártyán.
- A tizenkét szó véletlenszerű sorrendben következzen,
  egy körön belül mindegyik pontosan egyszer.
- A kártya alatt három nagy gomb legyen:
  „Főnév”, „Melléknév”, „Ige”.
- A játékos a megfelelő csoport gombjára kattintva válaszoljon.
- Hibás válasznál adj rövid visszajelzést, és engedd
  ugyanannál a szónál újrapróbálni. Ne áruld el a megoldást.
- Helyes válasznál jelezd a sikert, és tedd a szót
  a megfelelő csoport látható szógyűjteményébe.
- Ezután egy „Következő szó” gombbal lehessen továbblépni.
- Egy helyesen besorolt szót többé ne lehessen újra besorolni.
- Mutasd, hány szót sorolt már be helyesen a játékos
  a tizenkettőből.
- Az utolsó helyes válasz után jelenjen meg gratuláció,
  és maradjon látható mindhárom csoport teljes szógyűjteménye.
- Legyen „Újrakezdés” gomb, amely törli az eredményt,
  kiüríti a csoportokat és újrakeveri a szavakat.
- Ne legyen időkorlát.

A felület legyen magyar nyelvű, letisztult, jól olvasható,
telefonon és okostáblán is kényelmesen használható.
A válaszadás kattintással vagy érintéssel működjön,
húzás nélkül. A visszajelzések szövegesek is legyenek,
ne csak színek jelezzék az eredményt.

A teljes játék egyetlen önálló index.html fájlban legyen,
a CSS-sel és JavaScript-kóddal együtt. Külső függőség
és internetkapcsolat nélkül, helyi fájlként megnyitva is működjön.

A csoportokat és a hozzájuk tartozó szavakat a kód elején,
egy jól megjelölt adatszerkezetben tárold, hogy később
más tantárgyhoz is könnyen átírható legyen.

A válaszban a teljes index.html kódját add meg.
```