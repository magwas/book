# A modell leírása

## Struktúra

Az alapstruktúra egy fa, amely ideális \(a \[Dunbar szám\]\([https://en.wikipedia.org/wiki/Dunbar's\_number\)hoz](https://en.wikipedia.org/wiki/Dunbar's_number%29hoz) közeli\) méretű csoportokat tartalmaz mint leveleket, és a csomópontjainak \(a "metacsoport"oknak\) a fokszáma is az ideális körüli.

A struktúra csomópontjai opcionálisan lehetnek civil szervezetek, helyi, országos vagy nemzetközi kormányzatok. Az ilyen csomópontokhoz lehet erőforrásokat rendelni \(pl. város, ország\), és a hozzájuk tartozó alfa tagságát korlátozni tagság/állampolgárság/egyebek alapján. Máskülönben a tagok és a csoportok szabadon mozognak a struktúrában bizonyos szabályok mentén, ésa struktúra reagál ezekre a mozgásokra, hogy biztosítsa azokat a tulajdonságokat, amelyek ezáltal a megfelelő kommunikációt és döntéshozatali sebességet biztosítják.

### Csoportok

A struktúra alapvető építőköve a csoport. A jó - valódi emberi kapcsolatokra épülő - kommunikáció és döntéshozatal lehetőségének biztosítása érdekében a csoport méretének van egy alsó és felső korlátja valahol a Dunbar szám környékén, pl. 30 és 90. Ha a csoport mérete túllépi a maximumot, a csoport két csoportra válik szét. A szétváláshoz használt algoritmus alapulhat az új névre és célokra vonatkozó preferenciákon, lehet egy [minimális vágási algoritmus](https://en.wikipedia.org/wiki/Minimum_cut) a tagok egymás iránt megadott preferenciáira alapozva, vagy a fentiek kombinációja. Ha a taglétszám a minimum alá csökken, a csoport megszűnik létezni a formális struktúrában.

Egy egyén részt vehet több csoportban is, így követheti különböző érdeklődési köreit. Pl. valaki egy település polgára, érdekli a környezetvédelem, bélyegeket gyűjt, és szeret repülővel repülni, ezért négy olyan csoportnak a tagja, amelyek ezen érdekek mentén szerveződtek. Van egy limit arra, hogy egy egyén hány csoportban vehet részt, hogy csökkentsük az egyének lehetőségeit a strulktúra rombolására.Egy egyén bármikor megszüntetheti a tagságát egy csoportban, vagy kérheti felvételét egybe.

Alapértelmezésben a csoprtba való felvétel automatikusan elfogadásra kerül, de lehetnek csoportok, amelyek csak alkalmas tagokat vesznek fel. Az alkalmassági kritérumok példái: a helyi önkormányzattal foglalkozó csoportok csak helyi polgárokat vesznek fel, a repülőklub tagjainak be kellfizetni a repülők üzemeltetési költségeit fedező tagdíjat. Ha valakinek az alkalmassága megszűnik, automatikusan megszűnik a csoport tagjává válni.

Létezik egy "alapértelmezett" \("default"\) csoport, amelynek azok a tagjai, akik még nem csatlakoztak egyetlen csoporthoz sem, vagy minden más csoportban megszűnt a tagságuk. Ez az a pont, ahol a rendszer használatát problémásnak találó emberek segítésére vonatkozó aktivitásokat koncentrálni lehet.

### Csomópontok, metacsoportok, szervezeti csomópontok

A csomópont a modell egyik absztrakciója. A csoport egyfajta csomópont. A csoportok csoportja - a metacsoport - szintén egyfajta csomópont.

A csomópont szót abban az értelemben használjuk, ahogyan a gráfelméletben szokás. Tehát a csomópontoknak lehet szülője és lehetnek gyermekei, egy részfát definiálnak, és a teljes struktúra is egy fa, pontosan egy gyökér csomóponttal. A "felfelé" irányt a gyökér csomópont irányába értjük.

A csomópontok megfeleltethetőek az emberek különböző szervezeteinek: helyi, országos vagy nemzetközi kormányzatoknak, kluboknak, mozgalmaknak, akár cégeknek is \(noha meglehetősen szoci dolog lenne ezt a formális struktúrában tenni\).

A csomópontoknak lehetnek tulajdonságai, alkalmassági kritériumai, szabályai és hivatalnokai.

A metacsoportoknak azonban nem lehetnek közvetlen tagjai egyének, csak csoportok vagy más metacsoportok. A metacsoportok tagjainak száma legalább egy, és van egy felső limit is, pl. 90.

Ha egy csoport kettéválik, az így keletkező csoportok mind az eredeti szülő csomópont gyermekei lesznek, ha az alkalmassági kritérium ugyanaz. Egyébként az eredeti csoport helyén egy új metacsoport képződik, és az új csoportok annak lesznek a gyermekei.

A "szervezeti csomópont" egy azonos alkalmassági kritériumokkal rendelkező részfa legfelső csomópontja. A gyökér csomópont egy szervezeti csomópont.

A csomópontok dönthetnek úgy \(a lentebb leírt döntéshozatali mechanizmusok segítségével\), hogy mozognak a struktúrán belül. annak érdekében, hogy a fa kiegyensúlyozott maradjon, a mozgások olyan módonkorlátozottak, hogy egy csoport nem mozdulhat közelebbre a szervezeti csomópontjához, mint a mozgás előtt ahhoz legközelebb lévő csoport.

Egy csoport automatikusan örökli a szülő metacsoporttól az alkalmassági kritériumot, és minden rá vonatkozó olyan szabályt, amely nem lett helyileg felülírva.

### Informális struktúra, végrehajtó szervezetek

A fenti rész a formális struktúrát írta le. A formális struktúrában minden csomópontra vonatkoznak azok a szabályok, amelyek ebben a dokumentumban le vannak írva. Van egy alternatív fa is, amelyben a formális struktúra minden szabálya opcionális, és a döntések csak azokra az egyénekre kötelezőek, akik annak a részfának a tagjai, ahol a döntéseket hozták.

Az informális struktúra csomópontjai nem vesznek részt aformális döntéshozatali folyamatban \(de a tagok mint egyének kezdeményezhetnek döntéseket a formális csoportjaikban, az itt megjelenő igények alapján\).

Az formális struktúra csomópontjai tulajdonolhatnak csomópontokat az informális struktúrában. Ez lehetővé teszi, hogy nem-demokratikus szervezeteket \(intézményeket, cégeket\) építsenek ki a demokratikus szervezetek támogatására, miközben rendelkezésükre áll az eszközök összessége, amennyiben arra szükség van.

## Kulcsszereplők és hivatalok

A fő célok a kulcsszereplők és hivatalok szerepének megtervezésekora következőek voltak:

* A hatalom koncentrációjának elkerülése
* A kulcspozíciókat olyan egyének töltsék be, akiknél magas a valószínűsége, hogy birtokolják a szükséges szaktudást és képességeket
* Az egyének ösztönzői elsősorban a hivatal missziójának irányába hatnak

Ezért egy olyan rendszert javaslunk, amelyben:

* A hatalmi ágak elválasztásra kerülnek. Javasoljuk legalább a törvényhozó, végrehajtó, igazságszolgáltatás és kontroll hatalmi ágak használatát. Ez a kalsszikus _trias politica_ ágaihoz a kontroll hatalmi ágat adja hozzá, mert a procedurális felelősségre vonhatóság \(procedural accountability\) a hatékony működés biztosításának módja a teljes struktúrában.
* Míg a procedurális felelősségre vonhatóság a folyamatok hatékonyságát biztosítja, a stratégiai összehangoltságot a hatalmi ágak indirekt kontrollja biztosítja, a jogszabályalkotáson és a legfelső vezető közvetlen megválasztásán keresztül. A szervezeti integritást a legfelső vezető minimum hivatali ideje és az a tény védi, hogy a törvényhozó hatalmi ág csak szabályokat és célokat \(a "mit", és nem a "hogyant"\) szabhat más hatalmi ágak számára, és maga is kontrollálva van az igazságszolgáltatás által.
* A kulcsszereplők ösztönzői pénzügyi úton kerülnek kialakításra \(lásd Pénzügyek\), és egy olyan életpályamodellen keresztül, amelyben az alacsonyabb szinteken szerzett tapasztalat szükséges a magasabb szintek eléréséhez. Ez egyben stabilitást is hoz a modellbe.

### Képviselet \(törvényhozó hatalmi ág\)

A képviselők olyan választott hivatalnokok, amelyek a jogszabályalkotási folyamat minőségéért felelősek. A szerepük és felelősségeik a jogszabályalkotási folyamatnál kerülnek kifejtésre.

A képviselők száma egy csomópontban elegendően kevés ahhoz, hogy a szavazólapok ne legyenek túlzottan hosszúak, de elegendően sok ahhoz, hogy a különböző nézeteket képesek legyenek képviselni, mivel [a véleményeltérés fontos hajtóereje a jó döntéseknek](https://www.researchgate.net/profile/Stefan_Schulz-Hardt/publication/6653857_Group_Decision_Making_in_Hidden_Profile_Situations_Dissent_as_a_Facilitator_for_Decision_Quality/links/02e7e528b0b4141ce0000000/Group-Decision-Making-in-Hidden-Profile-Situations-Dissent-as-a-Facilitator-for-Decision-Quality.pdf) \(pl. 5\).

A döntéshozatali folyamat tulajdonsága, hogy minden javaslatnak van egy "ügyképviselő"je. Az ügyképviselő az az egyén, aki egy adott javaslatot kezdeményezett. Az ügyképviselőnek az adott ögyben futó döntéshozatali folyamatra vonatkozóan ugyanazok a jogai vannak, mint a választott képviselőnek.

A következő személyek választhatóak képviselőként:

* egy szinttel lentebbi csomópont v'lasztott képviselői
* olyan személyek, akik az adott csomópontban már voltak választott- vagy ügyképviselők

### További hatalmi ágak

A szervezeti csomópontoknak az összes többi hatalmi ághoz létezik egy megválasztott hivatalnokuk. Ez legalább a végrehajtó, igazságszolgáltató és kontroll hatalmi ágakat jelenti.

Minden típusú hivatalhoz tartozik egy minimum és maximum hivatali idő. Minden hivatalhoz tartozik egy minimális képzettség. Ezt a képzettséget úgy kell megválasztani, hogy valószínűvé tegye, hog y a jelöltnek vannak a hivatalhoz szükséges képességei és tapasztalatai, de lehetővé teszi, hogy sikerüljön megtalálni több olyan jelöltet, amely a tagok szerint megfelelő a hivatalra. Például csak bírók lehetnek az igazságszolgáltató hatalmi ág választott vezetői.

A magasabb csomópontokon követelmény lehet az alacsonyabb csomópontokon való gyakorlat.

### Választások

A választások a szokásos döntéshozatali folyamat keretein belülkezdeményezhetőek a minim hivatali idő letelte után. A maximum hivatali idő leteltekor a folyamat automatikusan megindul.

### Értékek és hosszú távú stratégia

Ennek az írásnak néhány szerzője amellett érvel, hogy szükség van egy hatalmi ágra, amely az értékekért és a hosszú távú stratégiai összehangoltságért felelős, amelynek legfelső vezetője az egységet, az értékeket és a szervezet tradícióit reprezentálja, hosszú minimális hivatali idővel és maximális hivatali idő nélkül, akár örökölhető hivatallal. Ennek a hatalmi ágnak leginkább konzultációs és reprezentatív jogosítványokkal és nagyon limitált, túlnyomóan felülírható vétóerővel kell rendelkeznie.

Ennek a hatalmi ágnak az ötlete a modern európai királyságok, a Dalai Láma és a gyenge prezidenciális rendszerek történelmi példáira épít.

## Jogszabályalkotási folyamat

### Jogszabályok

Minden csomópontnak saját szabályai vannak, a szokásos hierarchiában: A magasabb szintű csomópontok jogszabályai kötelező érvénnyel bírnak az alacsonyabb szinteken hozott döntésekkel és szabályokkal szemben.

Mivel a jogszabályalkotás kiterjed a döntéshozatali folyamatra és a struktúrára magára is, mindent meg lehet változtatni, ha arra szükség van. Hogy biztossá tegyük azt, hogy az alapvető értékek nem sérülnek, és hogy a hibás döntésekből fel lehessen épülni, a legfelső csomópontban kétmegváltoztathatatlan szabály van:

1. Az Emberi jogok Egyetemes Nyilatkozata minden más szabályt felülír
2. A döntéshozatali folyamatra és a struktúrára vonatkozó szabályok bármikor felülírhatóak egy "Debian Standard Resolution" folyamatban, ahol a szponzorok minimális száma sqrt\(n\) és a vitaperiódus ceiling\(ln\(n\)\) hét, ahol n a csomópont alatti egyének száma.

### Döntések

Az egyének jogosultak közvetlenül döntéseket kezdeményezni és szavazni jogszabályalkotási kérdésekben, amely magában foglalja a célok és a költségvetés meghatározását, és a választást a megfelelő képzettségű jelöltek közül a különböző hatalmi ágak vezető pozícióiba.

A döntéseket a fa csomópontjaiban lehet kezdeményezni, és azok "felúsznak" amíg el nem érik azt a csomópontot, amelyben relevánsak. Bárki kezdeményezhet döntést a saját csoportjában, és a választott képviselők abban a metacsoportban, amelybe megválasztották őket.

A döntéshozatali folyamat építőköve a "[Debian Standard Resolution Procedure](https://www.debian.org/vote/howto_follow)"-ra épül, megfelelő paraméterekkel. Ez egy bevált folyamat, amely magában foglalja a formális döntéselőkészítést, és úgy lett megtervezve, hogy mind a releváns elméleti eredményeket, mind a nyílt forrású mozgalom több évtizedes tapasztalatait figyelembe veszi.

A döntéselőkészítés abból áll, hogy összegyűjt egy menüt a döntés lehetséges alternatíváiból. Egy döntési alternatíva akkor lesz része a menünek, ha megfelel néhány kritériumnak \(megfelelő számú támogató egy csoportban, ametacsoportokban pedig a képesség, hogy felússzon addig\). Az alternatívát javasló egyén lesz annak ügyképviselője.

a csoportokban a döntéselőkészítés közvetlenül történik, míg a metacsoportokban a választott- és ügyképviselők folytatják a vitákat, és velük szemben elvárás a visszajelzések begyűjtése.

A szavazás [Condorcet módszer](https://hu.wikipedia.org/wiki/Condorcet-m%C3%B3dszer)rel történik, egy kitöltő, "a lenti alternatívák nem elfogadhatóak" alternatíva hozzáadásával, annak érdekében, hogy a teljes döntési teret lefedjük, és lehetőséget adjunk az elfogadhatóság  határainak jelzésére.

Amikor egy bizottságra szavazunk, a [CIVS Proporcionális reprezentációs módszer](http://civs.cs.cornell.edu/proportional.html)ét alkalmazzuk a tagok meghatározására. Acsomóponthoz tartozó részfa minden tagja egy szavazattal bír, akkor is, ha több csoportnak tagja. annak érdekében, hogy az egyének meg tudják határozni a saját bevonódási szintjüket, és egyben biztosítsuk a jó döntéseket, a szavazatok likvid demokratikus módon delegálhatóak, de csak választott-  vagy ügyképviselőknek.

### Döntési folyamat



