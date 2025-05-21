# Tesztautomatizálási kérdések

## Tesztelési alapok (ISTQB-hez kapcsolódó)
<img src="https://www.mindsmapped.com/wp-content/uploads/2016/06/ISTQB.jpg" alt="image" width="300" height="220">

#### ✅ Mi a tesztelés célja? Mi nem az?
A hibák felderítése és a szoftver minőségének biztosítása a cél. A hibák kijavítása nem az. 
#### ✅ Mik a tesztelési alapelvek?
 Korai tesztelés, hibaklaszterek, végtelen tesztelés lehetetlensége kontextusfüggőség.
#### ✅ Mi az egységtesztelés (unit testing)? Ki felelős az egységtesztek írásáért?
Egyedi kódrészek tesztelése. Felelősők: tesztelők.
#### ✅ Mik a tesztszintek, és mi a különbség köztük?
 Egység, integrációs, rendszer, elfogadási teszt. Különbség: Scope és cél (pl. egység: kód, rendszer: teljes rendszer).
#### ✅ Mi a különbség a verifikáció és a validáció között?
specifikáció vs. felhasználói igények.
#### ✅ Mik a tesztelési típusok, és mi a különbség köztük?
Funkcionális, nem funkcionális (pl. teljesítmény, biztonság). Különbség: Mit tesztelnek (funkciók vs. jellemzők).
#### ✅ Mi a különbség a fehér doboz, szürke doboz és fekete doboz tesztelés között?
Belátás a kódba (fehér), részleges (szürke), nincs belátás (fekete).
#### ✅ Mi a különbség a felhasználói elfogadási teszt (UAT) és a rendszerteszt között?
UAT: végfelhasználók, üzleti igények; rendszerteszt: teljes rendszer működése.
#### ✅ Sorolj fel különbségeket a regressziós tesztelés, a füsttesztelés és az újratesztelés között!
Regressziós: régi funkciók, füst: alapvető működés, újrateszt: javított hibák.
#### ✅ Mi a különbség a statikus és dinamikus tesztelés között?
Kód elemzése futás nélkül vs. futási időben tesztelés.
### ✅ Hasonlítsd össze a V-modellt, a vízesés modellt és az Agile megközelítést a tesztelés szempontjából!
V: tesztek párhuzamosan fejlesztéssel, vízesés: szekvenciális, Agile: iteratív, folyamatos tesztelés.

<img src="https://t4.ftcdn.net/jpg/03/90/15/65/360_F_390156585_8w1lsOyICIAOvDCU8tExXW2QwLCOFwXD.jpg" alt="image" width="550" height="400">


<img src="https://i.imgur.com/S38EBJw.png" alt="image" width="550" height="400">   <img src="https://segedletek.level14.hu/assets/img/modszertan-vizeses.svg" alt="image" width="550" height="400">


<img src="https://promanconsulting.hu/wp-content/uploads/2022/03/agilis-modszertanok-optimized.jpg" width="550" height="400">





## Reporting, Bugs
<img src="https://moolya.com/blog/wp-content/uploads/2023/05/Bug-Report.png" alt="image" width="300" height="220">

#### ✅ Milyen lépéseket követnél egy hiba megtalálásakor?
Elsönek leirnám az információkat majd a lépéseket amiket tettem hogy megtaláljam majd ezeket az információkat bejelentem
#### ✅ Beszélj a gyakori tesztjelentésekről és részleteikről!
Legtöbbször valami elvan irva vagy valami kis hiba van a programban.
#### ✅ Mit tartalmaz egy hibajelentés?
A hiba leírását, maga a hibát, rangsorolását, és lépéseit
#### ✅ Hogyan rangsorolnál egy hibát?
Lehet kritikus, kozepes, vagy alacsony besorolású

## Test Automation, Selenium
<img src="https://media.licdn.com/dms/image/C4D12AQE3GOyVsZazOw/article-cover_image-shrink_600_2000/0/1583830696602?e=2147483647&v=beta&t=bYHbKyhMoWsMgtEug6eSf3m0db5ZtGEl437TeS1qkfI" alt="image" width="320" height="220">

#### ✅ Melyik teszteseteket érdemes automatizálni és melyiket nem?
Egy egy funkciót érintő teszteket érdemes automatizálni hisz azok nem olyan komplikáltak.
#### ✅ Írj le egy jó automatizált tesztet!
```
Open Browser    https://www.saucedemo.com    firefox
Input Text    //*[@id="user-name"]    standard_user
Input Password    //*[@id="password"]    secret_sauce
Click Button    //*[@id="login-button"]
Close Browser
```
#### ✅ Mi a Selenium, Selenium IDE és Selenium WebDriver?
A Selenium automatizálja a browsereket.
Selenium Webdrive segit nekünk a browsereket automatizálni.
A selenium IDE Segít nekünk ezeket az automatizációkat elkészíteni.
#### ✅ Hogyan lehet azonosítani a webes elemeket?
HTML-es id vagy classok alapján.
#### ✅ Hogyan lehet várni az elemekre, és mi lehet a probléma? Gyűjtsd össze a lehetséges hibákat és okokat!
```
new WebDriverWait(driver, TimeSpan. FromSeconds(20))
```

Időtúllépés, nem található elem, nem kattintható.

Okok: Lassú betöltés, hibás lokátor, aszinkron műveletek.
#### ✅ Hasonlítsd össze a POM és a Keyword Driven Testing megközelítéseket!
POM: Objektummodell, kód alapú, karbantartható.
Keyword Driven: Táblázatvezérelt, kevés kód, kevésbé technikai felhasználóknak.
#### ✅ Mi a különbség a TDD és BDD között?
TDD:Fejlesztői tesztelés (unit tesztek előre).
DBB:Közös nyelv (Gherkin), üzleti és fejlesztői együttműködés.
#### ✅ Mi az API tesztelés és miért hasznos?
 Backend kommunikáció tesztelése. 
 Hasznos: Gyors, független a GUI-tól, magas lefedettség.
#### ✅ Mi az adatvezérelt tesztelés és miért hasznos?
Tesztesetek különböző adatokkal futtatása. 
Hasznos: Hatékony, nagyobb lefedettség, kevesebb kódismétlés.

[Szoftvertesztelés pdf](https://aries.ektf.hu/~gkusper/SzoftverTeszteles.pdf)

[Selenium](https://www.selenium.dev/)

[Viselkedés vezérelt fejlesztés](https://hu.wikipedia.org/wiki/Viselked%C3%A9svez%C3%A9relt_fejleszt%C3%A9s)