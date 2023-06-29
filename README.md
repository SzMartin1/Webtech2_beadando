>## Webtechnológiák 2 beadandó

># A feladat témája

A weboldaman témájának egy külföldi magyaros étterem online felületét szerettem volna létrehozni (ez meg is magyarázza miért angol az oldal), ahol lehet regisztrálni, rendeléseket leadni, különbőző tradícionális magyar ételek közül lehessen választani.

A felhasználó regisztrálhat, bejelentkezhet (a regisztrációs adatokat a MongoDB Atlas tárolja) megtekintheti, hogy mely ételeket adta hozzá a kosárhoz (Cart), mennyiségeket állíthat be, valamint számolnia sem kell, hiszen automatikusan kiszámolja az oldal a fizetendő összeget.

Ezután ha a felhasználó rámegy a Proceed to payment gombra, egy összegzés lesz látható a rendeléséről, ahol beállíthatja,hogy hova szállítsa ki majd az étterem az ételt. Próbáltam a PayPal-t hozzárendelni a projektemhez, de sajnos az még nem sikerült.

># A projekt indítása

1. Klónozás
2. A backend/src mappában létre kell hozni egy .env fájlt, ahol meg kell adni a MONGODB URL-t.
3. Függöségek letöltése az npm install segítségével
4. Backend elindítása (npm start) (http://localhost:5000)
5. Frontend elindítása (npm start) (http://localhost:4200)

># Opciók

A projekt elindítása után a Homepage fogad majd minket nagyon finom ételekkel. A Jobb felső sarokban lehet bejelentkezni. Ha az illető még nem regisztrált, itt van egy olyan opció, ahol megteheti.A regisztrálással egy POST kérést küldünk a backend-nek, amely létrehoz egy adatbázis bejegyzést a megadott felhasználói adatokkal. A regisztrációs oldalon az oldal kérni fogja az email címet, jelszót és a felhasználó címét. Ügyeljünk arra, hogy két ugyan olyan felhasználót nem lehet létrehozni.

Belépés után (ami szintén egy POST kérés a backend felé), mint említettem, a felhasználó hozzáadhatja a a kívánt ételeket a kosarához, megtekintheti a kosarát, állíthatja a mennyiséget. A Proceed to Payment gomb megnyomásával egy összegzés fog előjönni a rendelésről. Itt a felhasználó beállíthatja az oldalon megjelenő térkép segítségével, hogy hova szállítsa ki az étterem a rendelését. Mint említettem itt az oldal megakad, mivel nem sikerült rendesen hozzákapcsolnom még a PayPal funkciót az oldalamhoz.

Ha a felhasználó befejezte a rendelést és vissza szeretne térni a Főoldalra, akkor a bal felső sarokban lévő Hungarian Fine Dining feliratra kattinta ezt meg is teheti.

># Roadmap és betekintés

A Roadmap fájlban található a projektem "útja", vagyis az, hogy hogyan is miként készítettem el. A betekintes.pdf fájl tartalmaz az oldalamról pár képet.
