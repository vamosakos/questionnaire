# Rendszerterv

## 1. A rendszer célja
A rendszer célja, hogy a felhasználó könnyedén tudjon kérdőívekeket keresni, kitölteni. Az adminisztrátor (munkatárs) ezek mellett, egyszerűen tud saját kérdőívet is létrehozni, sőt akár ki is tudja nyomtatni azt. Ha viszont az adminisztrátor bele szeretne nyúlni a saját kérdőívébe, akkor azt roppant egyszerűen tudja szerkeszteni, mivel erre is van lehetőség. A már beregisztrált felhasználók, kitölthetnek kérdőíveket, amik bekerülnek az adatbázisba. Fontos, hogy a felhasználó könnyen eltudjon igazodni a felületeken, ezért minimalista felhasználói felületet kap a weboldal. Mivel ez egy weboldal, tervünk, hogy alkalmazkodjon az eszközhöz, tehát mobilon (Android/IOS) és számítógépen is könnyedén kezelhető legyen.

### Vágyálom rendszer
Egy olyan weboldalra, illetve rendszerre van szükségünk, ahol ügyfeleink igényeit ismerjük meg.
Ehhez azonban elengedhetetlen a letisztult, reszponzív dizájn és a figyelemet fenntartó tartalom.
Éppen ezért kifejezetten alapos munkát igényel a felhasználó-barát elrendezés és a megfelelő megjelenés.
Továbbá szolgálatatásunkat hasonló interface keretében egy mobil appon keresztül is elérhetővé szeretnénk tenni.
Mindezenmellett, megszeretnénk könnyíteni elkötelezett munkatársaink dolgát is.
A kérdőívek létrehozásánál lehetőség van személyreszabható opcionális minta megadására a válaszok feltöltésénél.
A háttérfolyamatok, mérések és statisztikák egyszerű kezelésére a gép által automatikusan generált diagrammok és ábrák segítenek majd.

## 2. Projektterv
- **Developer Team**: Csanádi Balázs, Madarasi Gábor, Vámos Ákos, Vámos Márton,  
- **Developer Support**: Palotai Marcell Martin
- **Scrum Master**: Vámos Ákos
- **Product Owner**: Vámos Márton

| Funkció                     | Feladat                                   |
| ----------------------------| ------------------------------------------|
| Köv. spec                   | A megrendelő dokumentációja               |       
| Funk. spec                  | A fejlesztő csapat dokumentációja         |       
| Rendszerterv                | A rendszer átfogó dokumentációja          |      
| Adattárolás                 | Adatbázis megvalósítása                   |      
| Regisztrációs felület       | php/html                                  |      
| Bejelentkezési felület      | php/html                                  |       
| Főoldal                     | php/html                                  |
| Információs oldal           | php/html                                  |
| Keretrendszer megvalósítása | A keretrendszer megismerése, elsajátítása |
| Kérdőívek feltöltése        | php/html                                  | 
| Kérdőívek kilistázása       | php/html                                  |
| Kérdőívek módosítása        | php/html                                  |    
| Design                      | css/javascript                            |    


## 3. Üzleti feladatok modellje
![Üzleti folyamatok modellje](https://media.discordapp.net/attachments/323508728508710913/1039320672574377994/image.png?width=588&height=676)

## 4. Követelmények
### Funkcionális követelmények:
- Felhasználó adatainak tárolása
- Felhasználók csoportokba való szervezése
- Webes környezetben való mükődés
- Bejelentkezés gomb: felhasználónév és jelszó együttes megadásával beléphetünk a saját fiókunkba.
- Regisztrációs gomb: az itt megadott adatainkkal kitöltve tudunk fiókot létrehozni.
- Kérdőív feltöltése gomb: kérdőívek feltöltésére szolgál.
- Kérdőív szerkesztése gomb: kérdőívek utólagos szerkesztése miatt.
- Kép feltöltése gomb: képek feltöltése.
- Statisztika gomb: kérdőívekre adott válaszok statisztikája.
- Keresés gomb: kérdőívek közötti keresést biztosítja.
- Visszaigazolókód nyomtatása gomb: lehetőséget nyújt a kérdőív kitöltése után a visszaigazolókód kinyomtatására.
- Statisztika nyomtatása gomb: statisztikák nyomtatására szolgál.

### Nem funkcionális követelmények:
A felhasználók nem jutnak hozzá más felhasználók személyes adataihoz a nevükön és az azonosítókon kívül.

### Törvényi előírások, szabványok
- GDPR betartása.
- AZ EURÓPAI PARLAMENT ÉS A TANÁCS (EU) 2016/679 RENDELETE.
- Az információs önrendelkezési jogról és az információszabadságról szóló 2011. évi CXII. törvény 4.§ (1) és (2) bekezdései. 


## 5. Funkcionális terv
### Rendszerszereplők:
- **Vendég**
- **Felhasználó**
- **Adminisztrátor**


### Rendszerhasználati esetek és lefutásaik:
**Vendég**:
- Amennyiben rendelkezik érvényes fiókkal, bejelentkezhet a "Bejelentkezés" menü pontra kattintva
- Felhasználói fiók hiányában regisztrálhat a "Regisztrációs" fül alatt
- Megbizonyosodhat és betekintést kaphat az oldal, illetve kérdőívek céljáról a "Rólunk" nevű menüpontra kattintva

**Felhasználó**:
- Bejelentkezhet felhasználói fiókjába a "Bejelentkezés" menü pontra kattintva
- Lehetősége nyílik a "Kérdőívek" nevű gomb által kilistáznia az aktuálisan elérhető kérdőíveket
- A kérdőívek könnyebb elérése érdekében a keresés is biztosított
- A "Kérdőív kitöltése" gombra kattintva kitöltheti az általa kiválasztott kérdőívet
- Megbizonyosodhat és betekintést kaphat az oldal, illetve kérdőívek céljáról a "Rólunk" nevű menüpontra kattintva
- Kijelentkezhet fiókjából a "Kijelentkezés" gomb segítségével

**Adminisztrátor**:
- Bejelentkezhet adminisztrátori fiókjába a "Bejelentkezés" menü pontra kattintva
- Lehetősége nyílik a "Kérdőívek" nevű gomb által kilistáznia az aktuálisan elérhető kérdőíveket
- A kérdőívek könnyebb elérése érdekében a keresés is biztosított
- Továbbá jogosultsága van új kérdőívek létrehozására/feltöltésére (megírására) és a már meglévők módosítására
- Megbizonyosodhat és betekintést kaphat az oldal, illetve kérdőívek céljáról a "Rólunk" nevű menüpontra kattintva
- Kijelentkezhet fiókjából a "Kijelentkezés" gomb segítségével


### Menü-hierarchiák:
- **REGISZTRÁCIÓ**
    - Bejelentkezés *(Már van meglévő fiókja?)*
    - Rólunk *(információs lap)*

- **BEJELENTKEZÉS**
    - Regisztráció *(Még nem regisztrált?)*
    - Rólunk *(információs lap)*

- **RÓLUNK**
    - Bejelentkezés *(amennyiben vendégként látogatja az oldalt)*
    - Regisztráció *(amennyiben vendégként látogatja az oldalt)*
    - Kérdőívek
    - Kijelentkezés

- **KÉRDŐÍVEK**
    - Keresés
    - Kérdőív kitöltése
        - Visszaigazoló kód nyomtatás
    - Kérdőív szerkesztése *(adminisztrátori)*
    - Kérdőív feltöltése *(adminisztrátori)*
        - Kép feltöltése
    - Kérdőív statisztikáinak nyomtatása *(adminisztrátori)*
    - Rólunk *(információs lap)*
    - Kijelentkezés

### Menükhöz tartozó specifikációk:
| Modul | ID | Név | v. | Kifejtés |
|---|---|---|---|---|
| Jogosultság | K1 | Bejelentkezési felület | 1.0 | A felhasználó az email címe és jelszava segítségével bejelentkezhet. Ha a megadott email vagy jelszó nem megfelelő, akkor a felhasználó hibaüzenetet kap. |
| Jogosultság | K2 | Regisztráció | 1.0 | A felhasználó a teljes nevével, majd az emailjének és jelszavának megadásával regisztrálja magát. A jelszó tárolása kódolva történik az adatbázisban. Ha valamelyik adat ezek közül hiányzik vagy nem felel meg a követelményeknek, akkor a rendszer értesíti erről a felhasználót. |
| Jogosultság | K3 | Kijelentkezés | 1.0 | A bejelentkezett felhasználók a kijelentkezés gombra kattintva kitudnak jelentkezni, amely a bejelentkező felületre irányíja őket. |
| Feltöltés | K4 | Kérdőív feltöltése | 1.0 | Az általunk kiválasztott munkatársaknak lehetőségük van kérdőívek feltöltésére. |
| Feltöltés | K5 | Kérdőív szerkesztése | 1.0 | A hozzáadott kérdőívek utólagos szerkesztésének lehetősége. |
| Feltöltés | K6 | Kép feltöltése | 1.0 | Különböző képek feltöltése, mint opcionális választási lehetőségek egy-egy kérdőívnél. |
| Statisztika | K7 | Kérdőív statisztikái | 1.0 | Az adminisztrátor elér egy összesített statisztikát a kérdekre kapott válaszokról. |
| Keresés | K8 | Keresés | 1.0 | A keresés mező segítségével egyszerű kulcsaszavak megadásával kereshetünk különböző kérdőívekre. |
| Nyomtatás | K9 | Visszaigazoló kód nyomtatása | 1.0 | A visszaigazolókód nyomtatás gomb lehetőséget nyújt a kérdőív kitöltése után a visszaigazolókód kinyomtatására, letöltésére PDF formátumban. |
| Nyomtatás | K10 | Statisztikák nyomtatása | 1.0 | A statisztikák nyomtatása gomb lehetőséget nyújt az adott kérdőíhez tartozó statisztikák nyomtatására, letöltésére PDF formátumban. |


## 6. Fizikai Környezet
A teszt webes környezetben és minden böngészőben reszponzívnak készül el. Nincsenek megvásárolt komponenseink.


## 7. Fejlesztői eszközök:
- Sublime Text
- Visual Studio Code
- Laravel
- XAMPP


## 8. Architekturális terv
- A kérdőívek és a felhasználók adatai egy MySQL adatbázisban tárolódnak. 
- Az adatbázist és a weboldalt PHP-ban (Laravel) kötjük össze.
- A weboldal "vázát" HTML nyelven írjuk le, a kinézethez CSS-t használunk.


## 9. Adatbázis terv
![Adatbázis terv](https://cdn.discordapp.com/attachments/323508728508710913/1038906389533315222/image.png)


## 10. Implementációs terv

Egy kérdőív kitöltő webalkalmazást készítünk.

A kérdőíveket egy PHP keretrendszer segítségével tesszük a felhasználó számára elérhetővé egy adatbázisból kérdésenként (amik között a felhasználó egy gombnyomással tud lépkedni), jegyezzük fel a kérdésekre az adott válaszait és állítunk ezekből össze statisztikát, illetve magának a felhasználónak az adatait is ezzel regisztráljuk az adatbázisba - mindegyik külön PHP fájlokban az egyszerűbben áttekinthetőbb kód végett. 

A webalkalmazás fejlesztését külön-külön felosztjuk a csapat között, ebbe beleértve az oldal backend és frontend kódját, a designt és a vázat. 

## 11. Használt technológiák
- Trello: kanban tábla a projekt szervezéséhez és kezeléséhez
- Discord: a csapattagok közötti kommunikáció
- Git: verziókezelés (azon belül is az ezt használó GitHub oldalt használva)
- MySQL / MariaDB: adatbázisszerver
- Apache2: webszerver
- Visual Studio Code: a weboldal elemei kódjának megírásához
- HTML: a weboldal "vázát" adjuk meg
- CSS: a weboldal kinézetét határozzuk meg
- PHP / Laravel: formokhoz, az adatbázisok kezeléséhez, a statisztika előállításához
