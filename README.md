<p align="center"><img src="https://multiuploader.github.io/icon.png"></p>


# <p align="center">MultiUploader</p>
<p align="center">Játék, Konzol, Film, Sorozat, Program, Mobil, Zene, XXX és Könyv feltöltése <a href=https://predb.club/api/v1/?q=AUTODESK.MOLDFLOW.ADVISER.ULTIMATE.2023.WIN64-MAGNiTUDE>predb.club</a> és <a href=https://predb.de/api/?q=Rammstein-Adieu_(Remixes)-WEB-DE-2022-ENRiCH>predb.de</a> segítségével (emiatt lehetnek hibák, ha rossz kategóriába sorolják itt, beolvasás után váltható tetszőlegesen a kategória) egy Uploaderben egyesítve</p>

### Általános
0. Telepítsd fel tetszőleges mappába!
1. 'Read' gombbal beolvassa az összes .torrent fájlt abból a mappából amit megadtál vagy a 'Read & Create Torrent' gombbal létre hozza a .torrentet aztán beolvassa azt amit elkészített.
1.1 Megvizsgálja, hogy fent van-e az oldalon ez a konkrét release amit felszeretnél tenni szóval 1:1ben meg kell egyezzen, hogy azt mondja fent van már, ellenkező esetben nem szól! (Dupera figyeljetek!)
2. Módosítsd kedvedre a leírást.
3. Save/Save All gomb egyikével mentsd el őket.
4. Upload gomb megnyomásával pedig elkezdi őket egyesével feltölteni! 

<details>
  <summary><strong>Alapvető működési beállítások</strong></summary>
  <i><p align="center">Beállítások nagy része egyértelmű, de pl van olyan, mint a süti jelszó és az APi kulcsok...
(nem kell sehova sem " [aposztróf], ha esetleg beírnád kitörli, hogy ebből ne legyen hiba)</p></i>

* nCore Cookie Password megjelenítéshez Chrome-ra és a belépési oldalon lévő "Csökkentett biztonság" opcióra van szükséged, ha bekapcsoltad a csökkentett biztonságot és bejelentkeztél akkor az F12-es gomb lenyomása után [ITT](itt lesz majd a kép) találod.

* nCore API Token kinyeréséhez nyisd meg pl a [[Prémium]](https://ncore.pro/shop) oldalt, majd Chrome-ot használva az F12-es gomb lenyomása után [ITT](https://i.kek.sh/y00g5YkHcPL.png) találod. (60 napig érvényes)

* `Torrents folder` - .torrent fájlokat itt keresi

* `Torrent Data folder` - itt pedig a .torrent fájlokban szereplő mappát keresi meg, értelemszerűen azon belül pedig az nfo-t.

* qBittorrent WebUI használatra mondj nemet, ekkor csak a Watch folderes megoldás lesz elérhető ami annyit tesz, hogy a kliensedben megadsz egy figyelt mappát és a progi oda tölti le a fájlt.

* Kérésekben való keresést kapcsold ki ha nem ellenőrzöd a találatait!
</details>

<details>
  <summary><strong>Haladó beállítások</strong></summary>
  
* Ha qBittorrentet használsz akkor automatikusan hozzátudod adni a klienshez a fájlt WebUI-on keresztül, a kategóriákat nem szükséges kitölteni, csak ha szükséged van rá, hogy feltöltésnél a "Working category"-ban lévő cuccokat hagyja figyelmen kívül ha nincsenek készek és megállítva! (Ezek nekem voltak fontosak).
"Done Category" pedig az amiből pedig csak törli a feltöltött torrentet így elkerülve a kliensben a duplikációt.

* Ha inkább csak azt akarod, hogy feltöltés után csak leszedje az oldalról a .torrent fájlt és mappába tegye akkor a Watch folderes verziót használd.

* Tud keresni kérésekre az oldalon ez két opcióból áll, hogy ha van Release név és talált mellé Játék, Sorozat vagy Film címet akkor először csak a Release névre keres és utána akár ezekre a címekre is rátud keresni, ez sokszor hibázhat mivel nem konkrétumra keresünk vele, de csak kategórián belüli kéréseket ad vissza.
(pl.: Shoresy.S01E06.720p.WEB.h264-KOGi esetében, lefuttat egy keresést a "Shoresy.S01E06.720p.WEB.h264-KOGi" kulcsszóra illetve a "Shoresy" szóra is ha kell)

* Kitudod kapcsolni azt a funkciót is, hogy ha nem szeretnéd, hogy a sikeres feltöltés után a .torrent fájl törölve legyen.

* A feltöltések közötti szünet minimum értéke 5 másodperc, magasabbra állíthatod, kisebbre nem tudod.

* `Log file location` - ha "Log to file" opció aktív akkor mindent amit a logba ír a program kiírja neked fájlba is.

* Minden egyes hibáról hibaüzenetet az `%AppData%\MultiUploader` mappába tesz.
</details>

### <p style="text-align: center;"><strong>Kategóriák</strong></p>

<details>
  <summary><strong>Film és Sorozat</strong></summary>
  
  Ahhoz, hogy ez működjön szükséged van TMDB API kulcsra:

* TMDB API kulcsot itt tudsz igényelni: [ITT](https://www.themoviedb.org/settings/api/request), Segítség pedig: [ITT](https://kb.synology.com/hu-hu/DSM/tutorial/How_to_apply_for_a_personal_API_key_to_get_video_info) (Fake adatokat is megadhatsz, illetve elég a personal key)

#### Főbb jellemzők:

* Egyedi kép feltöltésének lehetősége (mintakép vagy infobar kép), infobar képet megfelelően átméretezi alapértelmezetten [Jobb-Klikk a képeken]

* Ha nincs NFOban Imdb link akkor név alapján megkeresi, van ehhez egy "Minimum similarity" ezt beállítod minél magasabb értékre annál pontosabb egyezéseket fogja csak visszaadni. (Ajánlott 90% vagy fölé tenni, mert akkor már elég pontos tud lenni!)

* Kategóriát megtudja állapítani magának, Film vagy Sorozat illetve SD vagy HD. (pl.: ha csak évszám van a címben akkor film lesz, ha évad vagy epizód szám illetve ha komplett dátum akkor sorozat kategória)

* Ha az Imdb-n lévő Magyar címmel megegyezik a release neve akkor az infobarban az Eredeti/Magyar címhez az Angol címet fogja írni.

* NFOban még rákeres egyéb film adatbázisokra is, azt is hozzádobja feltöltésnél. (tvmaze/thetvdb/rottentomatoes/mafab/port.hu/MyAnimeList/Netflix)

* TVmaze vagy TMDB oldaláról behúzza a plotot, illetve ha nincs kép imdb-n akkor azt is.

* 3 db mintaképet generál a film elejéről, vagy ha évad packról van szó akkor az első epizódból. (Ha nem talál videó fájlt akkor ezt a lépést kihagyja) 
  
<details>

  <summary><strong>Mivel többször is megeshet, hogy rossz ImdbID-t talál így azt a következő képpen tudod orvosolni:</strong></summary>
  <br>
  <p style="text-align: center;">Hasonló címmel rendelkező Imdb-t talál, de az hibás</p>

Érdemes rögzíteni a következőket a Settings -> Advanced Settings -> "Static ImdbID" mezőbe!

> "The Voice AU" - "tt2334429"<br>
> "The Block AU" - "tt0418372"<br>
> "Insight AU" - "tt1604928"<br>
> "World War Two Battles Won And Lost" - "tt9394316"<br>
> "Gruen" - "tt5957238"
</details>
</details>

<details>
  <summary><strong>PC és Konzol játék</strong></summary>
  
#### Főbb jellemzők:

* Egyedi kép feltöltésének lehetősége (mintakép vagy infobar kép), infobar képet megfelelően átméretezi alapértelmezetten [Jobb-Klikk a képeken]

* ISO, RIP kategóriát automatikusan sorolja be a program, a Kozol kategóriát pedig név vagy predb alapján dönti el.

* Steam, GOG és EpicGames linkeket keres NFOban és ha talál ilyent akkor mindenképpen játék kategória lesz.

* Steam és GOG API alapján van csak kitöltés így ezeken az oldalakon keresi meg a játékokat, random 3 db képet tölt le valamelyik oldalról és az infobar képet is innen veszi.

* Beállításokban lehet módosítani, hogy milyen legyen a leírása a játékoknak.

* Opcionálisan lehet állítani, hogy ha nem talál megfelelő linket NFOban és név alapján sincs találat egyik weboldalon sem a játékhoz akkor bekéri a Steam/GOG linket vagy feltölti üresen. (Üres feltöltés esetén van rá lehetőség, hogy template-et rakjon leírásba vagy sem)
</details>

<details>
  <summary><strong>Program és Mobil</strong></summary>
  
#### Főbb jellemzők:

* Egyedi kép feltöltésének lehetősége (mintakép vagy infobar kép), infobar képet megfelelően átméretezi alapértelmezetten [Jobb-Klikk a képeken]

* ISO, RIP vagy Mobil kategóriát automatikusan sorolja be a program.

* Ha talál az NFO-ban linket akkor azt a leírás végére beszúrja [Opcionális, beállításokban kikapcsolható]
</details>

<details>
  <summary><strong>Zene és Klip</strong></summary>
  
#### Főbb jellemzők:

* Egyedi kép feltöltésének lehetősége (mintakép vagy infobar kép), infobar képet megfelelően átméretezi alapértelmezetten [Jobb-Klikk a képeken]

* MP3, Lossless vagy Clip kategóriát automatikusan sorolja be a program.

* Stílust eldönti fájlból, pre oldalról lekéri ha van, ha egyik alapján sincs találat akkor bekéri.

* Zene kategória esetén teljes leírást csinál - Előadóval, Album címmel és Track listával [Opcionális, beállításokban kikapcsolható]

* Ha talál az NFO-ban linket akkor azt a leírás végére beszúrja [Opcionális, beállításokban kikapcsolható]
</details>

<details>
  <summary><strong>Könyv</strong></summary>
  
#### Főbb jellemzők:

* Egyedi kép feltöltésének lehetősége (mintakép vagy infobar kép), infobar képet megfelelően átméretezi alapértelmezetten [Jobb-Klikk a képeken]

* Magyar vagy Külföldi nyelv automatikusan kerül megállapításra a release nevéből.

* Ha ISBN alapján van találat Google Books-on akkor tud leírást csinálni. [Opcionális, beállításokban kikapcsolható]

* Mivel ebben a kategóriában nem lehet fájlból kiolvasni és még pre oldalakon sincsen címke megnevezve így ezt bekéri a program.
</details>

<details>
  <summary><strong>XXX</strong></summary>
  
#### Főbb jellemzők:

* Egyedi kép feltöltésének lehetősége (mintakép vagy infobar kép), infobar képet megfelelően átméretezi alapértelmezetten [Jobb-Klikk a képeken]

* HD, SD vagy Imageset kategória automatikusan kerül megállapításra.

* 3 db mintaképet generál az adott tartalom elejéről. (Ha nem talál videó fájlt akkor ezt a lépést kihagyja)

* Imageset esetén random 3 db képet választ ki amit feltölt, illetve opcionálisan megkeresi a cover képet és azt teszi ki infobarba.
</details>
