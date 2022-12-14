# Követelményspecifikáció

## 1. Áttekintés
Cégünk egy nemzetközileg is ismert utazási iroda, amely most legkinkább az itthoni ügyfeleink igényeinek felmérését célozza meg.
A projekt segítségével lehetőség nyílik a magyar utazni vágyók érdekeinek megismerésére és ez által minnél hatékonyobb segíségére.
Célunk megvalósításához egy olyan weboldal szükséges, ahol munkatársaink könnyedén tudnak kérdőíveket felvinni, illetve szerkeszteni azokat.
A különböző kérdőívekből a regisztrált felhasználóink válaszaiból pedig könnyedén felmérhetjük ügyfeleink szokásait/igényeit. 
Ezen statisztikák ismeretével a kínálatot az e fajta prioritások alapján végezzük.


## 2. Jelenlegi helyzet
Jelenleg egy jól működő utazási irodaként munkálkodunk, ahol próbálunk az alacsony ár és biztonságos utazások biztosítása mellett, a naprakészségben is kiválóan teljesíteni.
Ehhez elengedhetetlen az ügyefeleink megismerése és az Ő általuk megítélt legnépszerűbb utazási célpontok információinak begyűjtése. Ám ennek szegmensnek eddig nem túl sok profitja volt, ezért kezdenénk bele ebbe a projektbe. Ugyanis a projekt segítségével ezekre mind lehetőségünk nyilna. Nem csak egy-egy felhasználó cél országát, vagy települését tudnánk ezzel felmérni, hanem a kimutatott statisztikákkal könnyebben és pontosabb ajánlatot tudnánk ezáltal az ügyfeleinknek nyújtani.


## 3. Vágyálom rendszer
Egy olyan weboldalra, illetve rendszerre van szükségünk, ahol ügyfeleink igényeit ismerjük meg.
Ehhez azonban elengedhetetlen a letisztult, reszponzív dizájn és a figyelemet fenntartó tartalom.
Éppen ezért kifejezetten alapos munkát igényel a felhasználó-barát elrendezés és a megfelelő megjelenés.
Továbbá szolgálatatásunkat hasonló interface keretében egy mobil appon keresztül is elérhetővé szeretnénk tenni.
Mindezenmellett, megszeretnénk könnyíteni elkötelezett munkatársaink dolgát is.
A kérdőívek létrehozásánál lehetőség van személyreszabható opcionális minta megadására a válaszok feltöltésénél.
A háttérfolyamatok, mérések és statisztikák egyszerű kezelésére a gép által automatikusan generált diagrammok és ábrák segítenek majd. 


## 4. Funkcionális követelmények
- **Bejelentkezés gomb:** felhasználónév és jelszó együttes megadásával beléphetünk a saját fiókunkba.
- **Regisztrációs gomb:** az itt megadott adatainkkal kitöltve tudunk fiókot létrehozni.
- **Kérdőív feltöltése gomb:** kérdőívek feltöltésére szolgál.
- **Kérdőív szerkesztése gomb:** kérdőívek utólagos szerkesztése miatt.
- **Kép feltöltése gomb:** képek feltöltése.
- **Statisztika gomb:** kérdőívekre adott válaszok statisztikája.
- **Keresés gomb:** kérdőívek közötti keresést biztosítja.
- **Visszaigazolókód nyomtatása gomb:** lehetőséget nyújt a kérdőív kitöltése után a visszaigazolókód kinyomtatására.
- **Statisztika nyomtatása gomb:** statisztikák nyomtatására szolgál.


## 5. Rendszerre vonatkozó törvények, szabványok, ajánlások
### Törvények
- AZ EURÓPAI PARLAMENT ÉS A TANÁCS (EU) 2016/679 RENDELETE

- Az információs önrendelkezési jogról és az információszabadságról szóló 2011. évi CXII. törvény 4.§ (1) és (2) bekezdései.

### Rendszerszabványok, ajánlások
- A web felület szabványos eszközökkel készüljön, html/css/javascript/php
- A képek jpg/jpeg/png/gif formátumúak lehetnek
- A felhasznlókat azonosító weboldalak esetében szükséges jogszabályokat be kell tartani: GDPR
- A rendszer bíztosítsa a kérdőívet kitöltő személy teljes anonimítását
- Mindenképp biztosítsa a rendszer az elkezdett, de valamilyen okból félbeszakadt kérdőív kitöltésének folytatását.
- Legnépszerűbb böngészők támogatása (Chrome, Firefox, Edge, Opera, Safari)

- Trello (kanban tábla)
- Discord (kommunikáció)
- Github (a kóddal való együttműködés)
- Visual Studio Code (a kódoláshoz használt IDE)
- Sublime Text (a dokumentáció kidolgozásához)
- PHP (backend)
- HTML, CSS (a frontend és a design)
- Javascript (backend, frontend)
- Uizard prototype (képernyőtervhez)
- MySQL (adatbázis)
- Laravel (php keretrendszer)


## 6. Jelenlegi üzleti folyamatok modellje
A mai világban egyre több ember használ kérdőíveket. Ez által, a mi csoportunk célja az, hogy egy minél átláthatóbb, könnyen kezelhető weboldalt hozzunk létre, kérdőívet használók számára. 
A kivitelezésnél segítenek a folyamatok, különböző ábrákkal, diagrammokkal lesznek a végén szemléltetve egy adott kérdőív válaszai.


## 7. Igényelt üzleti folyamatok
![Kövspec - 7. Igényelt üzleti folyamatok](https://media.discordapp.net/attachments/1019343618131120319/1039235605772640276/Kovspec_7_-_Igenyelt_uzleti_folyamatok.jpg)


## 8. Követelménylista
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
| Nyomtatás | K9 | Visszaigazolókód Nyomtatása | 1.0 | A visszaigazolókód nyomtatás gomb lehetőséget nyújt a kérdőív kitöltése után a visszaigazolókód kinyomtatására, letöltésére PDF formátumban. |
| Nyomtatás | K10 | Statisztikák Nyomtatása | 1.0 | A statisztikák nyomtatása gomb lehetőséget nyújt az adott kérdőíhez tartozó statisztikák nyomtatására, letöltésére PDF formátumban. |


## 9. Riportok
- **Q:** Mi lenne a szoftver lényege?
- **A:** A szoftver egy felmérő lenne, ahol a munkatársaink űrlapokat állíthatnak össze, amire az esetleges ügyfeleink válaszolhatnak. A válaszok statisztikába rendezhetőek és a kapott adatok alapján képesek vagyunk bemérni, hogy a kitöltőnek melyik hely a legoptimálisabb. 

- **Q:** Milyen adatokat fog a program bekérni a felhasználótól a kérdéssor előtt?
- **A:** Nevet, e-mail címet és jelszót. Ezzel a felhasználó egy fiókot fog létrehozni, ami segítségével elérhetjük őt és az eredmény alapján keletkezett ajánlatokat el tudjuk hozzá juttatni. Fiók nélkül a kitöltés nem lehetséges.

- **Q:** A statisztikák elérhetőek lesznek a kitöltők számára? 
- **A:** A kérdőivekre lebontott összegzett statisztika csak a munkatársaink számára lesz elérhető, akik ezeket képesek kinyomtatni. A felhasználó kezdetben csak egy kinyomtatható igazoló kódot fog kapni, az eredményeket és az ajánlatokat csak utólagosan kapja meg a kiértékelés után.

- **Q:** A meglévő kérdéssorok törölhetőek és frissíthetőek?
- **A:** A kérdéssorokat a munkatársaink tudják módosítani: képesek kérdéseket hozzáadni, a meglévő kérdések szövegeit átírni, a meglévőeket törölni a létező kérdéssorokból. Teljes kérdéssorok törlésére is van lehetőség.

- **Q:** A kérdéssorokhoz lehet képeket és egyéb médiákat beszúrni?
- **A:** Igen, a kérdéssorokhoz és az egyéni kérdésekhez csatolhatóak képek, viszont hangok, videók és egyéb állományok nem.
