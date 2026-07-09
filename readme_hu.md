#  Pixerllr
#dataset #physics-prior #video-generation #benchmark
#A generatív videónak nincs szüksége több fantáziára. Több valóság kel!#
> **Valóságlenyomatok AI-videókhoz — gravitáció, fény, mozgás, szél, víz és anatómia tanítása valódi felvételekből...**

A hat ujjú kéz nem művészi döntés.
A lebegő test nem stílus.
A rossz irányba eső árnyék nem hangulat.

**Hiba — és te fizetsz érte minden elégetett kreditnél, minden kukázott generálásnál.**

Az AI-videógenerátorok nem tudják a fizikát.
Nem azért, mert buták — azért, mert soha senki nem tanította meg nekik.

A tanítóadatukban stúdiófény van, szélgép, drót és keverőpult.
A modell azt tanulja, amit lát: **mozifizikát**.

A mozifizika pedig hazudik.

**A pixerllr ezt a gyökérokot kezeli — nem a tüneteket foltozza.**

---

## Mit csinál?

Valódi felvételekből — élő szereplős filmből, természetfilmből, candid videóból — kinyeri a valóság törvényeit:

* **Anatómia és gravitáció**
  Hogyan mozog egy valódi test.

* **Öregedés**
  Hogyan merevedik a járás, hogyan ráncosodik a bőr évtizedek alatt.

* **Természetes fény**
  Hova esik az árnyék, ha a Nap világít.

* **Szél**
  Hogyan hajlik a nád, a lomb, a haj.

* **Víz**
  Hogyan terjed a hullám, ha senki nem rendezte meg.

* **Tér**
  Mélység a képben, zengés a hangban — nyílt vagy zárt a világ.

A kinyert törvény lenyomatként kerül tárolásra:

```text
csontváz-szekvencia
válaszgörbe
tér-lenyomat
```

Egyetlen JSON-rekord videónként.

**A kép megy a kukába. A törvény marad.**

Ebből épül a mintakönyvtár, amiből generatív modellek megtanulhatják, amit ma nem tudnak:

**élethű filmet készíteni.**

Nem életszerűt.
**Élethűt.**

---

## A gép

```text
FORRÁS      → archív ág: film, természetfilm
             + crowd ág: saját kamera

KINYERÉS    → könnyű réteg CPU-n
             + nehéz réteg ingyenes GPU-n

LENYOMAT    → JSON-rekord, hash-kulccsal, kép nélkül

KÖNYVTÁR    → törvénygörbék:
               szél ↔ lomb
               nap ↔ árnyék
               kor ↔ járás

CSOMAG      → prior-modulok
             + loss-könyvtár
             + mutató-dataset

VALIDÁCIÓ   → mérhetően kevesebb fizikai hiba,
               vagy nem ér semmit
```

Minden alkatrész kész, nyílt eszközre épül.

Semmit nem találtunk fel, ami már működik — csak összekötöttük, amit eddig senki.

---

## Két üzemmód — a valóság-kapu

### 1. Mérőműszer

Bármilyen videót pontoztathatsz, AI-generáltat is.

Megtudod, hol hazudik fizikát:

* kéz
* árnyék
* szél
* lebegés
* mozgás
* tér
* konzisztencia

Számokban.

A kukázott generálásod így tanulsággá válik.

**Riport jön. Tárolás nulla.**

---

### 2. Tanító

A könyvtárba kizárólag valódi felvétel léphet be.

Háromrétegű kapu őrzi:

1. **Eredet-ellenőrzés**
2. **Metaadat-koherencia**
3. **Fizikai korreláció**

A valódi felvétel korrelál a mért széllel és a kiszámított napállással.

A generált nem.

Ami elbukik, nem kerül be.

> **A kukázott generálásod tanulság.
> A referenciafelvételed kincs.**

---

## Mit kapsz — és mit kap a közös?

Futtatod a műszert, azonnal riportot kapsz.

**Ingyen. Feltétel nélkül.**

Ha valódi felvételed lenyomata átmegy a kapun, contributor vagy.

Contributor-ként kapsz:

* teljes felbontású hozzáférést a mintakönyvtár összes görbéjéhez;
* név szerinti, hivatkozható acknowledgmentet;
* korai hozzáférést a prior-csomagokhoz;
* előre betanított fizikatudás-modulokat, amelyeket a saját workflow-dba köthetsz;
* kevesebb selejtet;
* kevesebb elégetett kreditet.

A licenc a szerződésünk.

Az adat és a könyvtár:

```text
CC BY-NC-SA 4.0
```

Mindenkinek szabad nem-kereskedelmi célra.

Aki termékbe építené, kereskedelmi licencet vált.

**Te építed, te használod ingyen.
Aki pénzt csinál belőle, az hozzájárul a fenntartásához.**

Ez az OpenStreetMap-modell, és húsz éve működik.

---

## Mit nem csinálunk?

* **Videót nem tárolunk és nem terjesztünk. Soha.**
  A rekord metaadat és mutató — ugyanaz a modell, amire a legnagyobb nyílt datasetek épülnek.

* **Arcot, személyt, jelenetet nem őrzünk.**
  A lenyomatban nincs kép, nincs biometrikus adat — csak az, ami bármely domainben igaz.

* **AI-generált anyagot nem tanítunk.**
  Mérünk belőle — tanulni a valóságból tanulunk.

* **Kevert hangsávból zenét, szinkront nem tanítunk.**
  A helyszíni hang tér-lenyomata — zengés, nyílt vagy zárt tér — viszont törvény, és bekerül.

---

## Indulás — nulla telepítés

1. Nyisd meg a lenyomat-űrlapot:

   ```text
   Issues → New
   ```

2. Illessz be egy videó-URL-t.

3. Küldd el.

4. A mi gépünk dolgozik.

5. Te linket kapsz a riportodról.

6. A lenyomat magától a könyvtárba kerül, ha átmegy a valóság-kapun.

Visszatérő vagy, és saját gépen futtatnád?

**Forkold a repót — a többit a user-guide mondja el.**

---

## Kapcsolódó minta

Ez a README a [`Human2ai-intent-codec`](https://github.com/NullCodeLabs/Human2ai-intent-codec) irányából épített, narratív-technikai GitHub-formátumot követi:

* erős nyitó állítás;
* emberi probléma;
* technikai válasz;
* tiszta működési modell;
* contributor-érték;
* világos etikai határok;
* azonnali indulási út.

---

## Státusz

```text
v0.1 — építés alatt
```

Kész:

* séma;
* repo-váz;
* forráshierarchia.

Következik:

* kinyerő scriptek;
* validátor workflow;
* első törvénygörbék.

---

## Hozzájárulás

Ha látod benne, amit mi:

**Star.**

Ha használnád:

**Fork.**

Ha hibát találsz vagy jobb utat tudsz:

**Issue — azt olvassuk el először.**

---

## Licenc

© Infinity Possibility Media Co. | NullCodeLabs

Adat és dokumentáció:

```text
CC BY-NC-SA 4.0
```

Kereskedelmi felhasználás külön licenc alapján.

---

## Kapcsolat

* Email: `istvan.taubert@gmail.com`
* GitHub: [`@NullCodeLabs`](https://github.com/NullCodeLabs)
