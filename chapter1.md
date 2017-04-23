# A modell leírása

## Struktúra

Az alapstruktúra egy fa, amely ideális \(a [Dunbar szám](https://en.wikipedia.org/wiki/Dunbar%27s_number)hoz közeli\) méretű csoportokat tartalmaz mint leveleket, és a csomópontjainak \(a "metacsoport"oknak\) a fokszáma is az ideális körüli.

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



