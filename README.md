​CoreMentor – Scalable Mentorship for Migrant Students

A CoreMentor egy automatizált szoftvermegoldás ukrán menekült és migráns diákok mentorálására. Célunk a munkaigényes manuális koordináció felváltása egy skálázható digitális platformmal, amely 10 óráról mindössze 10 percre csökkenti a párosítási folyamat adminisztrációs idejét.

A Probléma és Megoldás
​A civil szervezetek jelenleg manuálisan próbálják összekötni a diákokat a mentorokkal, ami lassú és nehezen skálázható. A CoreMentor egy súlyozott párosítási algoritmust használ az optimális kapcsolatok létrehozásához.

Párosítási Logika
​A rendszer három fő dimenzió mentén rangsorolja a jelölteket:
​Nyelv (50% - Hard Filter): Közös nyelv nélkül nincs párosítás.
​Tantárgy (30%): Kompetencia alapú egyezés (pl. matematika, angol).
​Idősáv (20%): Heti elérhetőségek szinkronizálása.
​ Technikai Specifikációk
​A rendszer nyílt API-t biztosít, lehetővé téve más NGO-k számára az adatbázis-integrációt.

Főbb Végpontok (API Endpoints)
​POST /register-mentor: Önkéntesek regisztrációja és validálása.
​GET /match-suggestions: Rangsorolt párosítási lista pontszám-indoklással.
​PATCH /session-log: Automatikus követés és riasztás küldése 2 hét inaktivitás után.

Technológiai Stack
​Backend: Node.js / Python (FastAPI)
​Frontend: React Dashboard (NGO koordinátorok számára)
​Infrastruktúra: AWS/Azure (GDPR-kompatibilis)
​Biztonság: Zero-knowledge architektúra és rendszeres penetrációs tesztek.

Hatás és Eredmények
​Skálázhatóság: Jelenleg 100 diák és 40 mentor kezelése (havi ~350 naplózott óra).
​Hatékonyság: 98%-os csökkenés a manuális koordinációs időben.
​Transzparencia: Valós idejű dashboard a mentor nélküli diákok azonnali azonosítására.

Költségvetési Átláthatóság (Budget Summary)
​A projekt teljes költségvetése 39 450 EUR, melynek elosztása:
​Emberi tőke (78%): Senior és Medior Full-stack fejlesztők, Pilot koordinátor.
​Infrastruktúra (11%): Felhő tárhely és külső biztonsági audit.
​Automatikus Riasztás (Trigger):
​Ha egy aktív párosításnál 14 napon keresztül nem érkezik új session-log bejegyzés, a rendszer automatikus riasztást küld az NGO koordinátor irányítópultjára.


Foglalkozások Naplózása
​A mentori alkalmak követése és az inaktivitás figyelése.
​Végpont: PATCH /session-log

Impact & Social Value (Társadalmi Hatás)
​A CoreMentor nem csupán egy szoftver, hanem egy eszköz a társadalmi integráció felgyorsítására. A pilot időszak adatai alapján a következő eredményeket értük el:
​1. Operatív Hatékonyság
​Időmegtakarítás: A manuális párosítási folyamat 10 óráról 10 percre csökkent koordinátoronként.
​Hibaarány csökkenése: Az automatizált szűrés kiküszöböli a nyelvi félreértéseket és az időpont-ütközéseket a párosítások során.
Mérhető Eredmények (Pilot fázis)
​Mentorált diákok száma: 100+ aktív résztvevő.
​Aktív önkéntes bázis: 40 képzett mentor.
​Oktatási volumen: Havi ~350 naplózott mentorálási óra, amely közvetlenül támogatja a diákok iskolai előmenetelét és mentális jóllétét.
​3. Skálázhatóság & Fenntarthatóság
​Nyílt API: Bármely európai NGO integrálhatja a rendszert, így a megoldás országhatároktól függetlenül alkalmazható a menekültellátásban.
technológia célja itt nem az emberi kapcsolatok helyettesítése, hanem a bürokrácia lebontása, hogy a mentor és a diák a lényegre: a tanulásra és az egymásra figyelésre koncentrálhasson.
Adatvédelem és GDPR Megfelelés
​A CoreMentor tervezésekor az "adatvédelem beépített tervezéssel" (Privacy by Design) elvét követtük. Mivel kiskorúak és sérülékeny csoportok adatait kezeljük, rendszerünk megfelel a legszigorúbb uniós előírásoknak.
​Főbb Biztonsági Pillérek
​Zéró Tudás (Zero-Knowledge) alapú architektúra: A szenzitív adatokat titkosítva tároljuk; a rendszer csak a párosításhoz szükséges metaadatokat (nyelv, tantárgy, szabadidő) dolgozza fel.
Adatminimalizálás: Kizárólag a mentorálási folyamat elindításához elengedhetetlen adatokat kérjük be.
​Külső Biztonsági Audit: A projekt költségvetésének részét képezi egy független penetrációs teszt és adatvédelmi felülvizsgálat a kísérleti fázis indulása előtt.
​Tárhely: Kizárólag az EU területén található, GDPR-kompatibilis (AWS/Azure) szervereket használunk.
Jogkezelés
​A felhasználók (mentorok és gondviselők) számára dedikált felületet biztosítunk az alábbiakhoz:
​Hozzáférési jog: Bármikor lekérdezhetik a róluk tárolt adatokat.
​Törléshez való jog ("Az elfeledtetés joga"): A mentorálási kapcsolat lezárulása után kérhető az adatok teljes körű törlése.
​Adathordozhatóság: Az adatok exportálhatók szabványos JSON formátumban.
Jogi megjegyzés: A platformhoz tartozó teljes Adatkezelési Tájékoztató és a Közös Adatkezelői Megállapodás (a partner NGO-k számára) elérhető a dokumentációs portálunkon.
