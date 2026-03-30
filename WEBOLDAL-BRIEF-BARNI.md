# Scroll Studio – Weboldal fejlesztési brief

> **Készült:** 2026.03.26.
> **Címzett:** Kicsák Barnabás (frontend, webépítés)
> **Döntéshozó:** Tösmagi Eszter (CEO)
> **Cél:** A scrollstudio.hu (vagy scrollstudio.com) teljes weboldal megépítése – a 3 üzletág bemutatása + konfigurátor árazás

---

## 1. MI EZ ÉS MIÉRT SÜRGŐS

A Scroll Studio weboldalának KELL állnia **április 1-re**, mert:
- Viktor és Nóri aznap kezdenek hideghívni → kell hova küldeni az ügyfelet
- A konfigurátor online leadeket generál → ez a sales egyik lába
- Hitelesség: weboldal nélkül nincs bizalom

**Scope:** Egy weboldal, ami bemutatja a 3 üzletágat (Studio, Digital, Learning), és tartalmaz egy interaktív konfigurátort ahol az ügyfél maga állítja össze a csomagját.

---

## 2. OLDALTÉRKÉP (sitemap)

```
scrollstudio.hu
├── / (Főoldal)
├── /studio (Studio – Social Media konfigurátor)
├── /digital (Digital – Weboldal konfigurátor)
├── /learning (Learning – Challenge landing)
├── /rolunk (Rólunk – csapat, misszió)
├── /kapcsolat (Kontakt form + adatok)
├── /referencia (Case study-k) [opcionális, lehet a főoldalon is]
├── /adatvedelem (GDPR)
└── /aszf (ÁSZF) [később]
```

---

## 3. VIZUÁLIS IRÁNYELVEK

### Színek

| Szín | Kód | Használat |
|------|-----|-----------|
| **Arany** (elsődleges) | `#C8A96E` | CTA gombok, kiemelések, logó akcentus |
| **Fekete** (alap) | `#1A1A1A` | Háttér, szövegtörzs, fejlécek |
| **Fehér** | `#FAFAFA` | Szöveg sötét háttéren, kártyák |
| **Szürke** | `#888888` | Alcímek, elválasztók, másodlagos szöveg |
| **Sötét arany** | `#A68B5B` | Hover állapotok |

### Betűtípusok

| Használat | Font |
|-----------|------|
| Fejlécek (H1-H3) | **Montserrat Bold** vagy **Inter Bold** |
| Szövegtörzs | **Inter Regular** vagy **Open Sans** |
| Számok, árak | **Inter Bold** (nagyobb méretben) |

### Hangulat

**Prémium, de elérhető. Technológiai, de emberi. Dinamikus.**
- Sötét háttér, arany kiemelések (Apple-vibe)
- Sok whitespace, tiszta elrendezés
- Minimális animáció (scroll reveal, hover effekt)
- Nincs zsúfoltság – inkább kevesebb, de hatásosabb

---

## 4. FŐOLDAL (/)

### Szekciók sorrendben:

#### 4.1 HERO

```
Headline: „Ügynökségi minőség. AI-sebesség. Vállalkozóbarát ár."
Sub-headline: „Social media · Webfejlesztés · Online oktatás – egy kézből."

[CTA 1: „Összerakom a csomagomat" → /studio vagy /digital]
[CTA 2: „Ingyenes konzultáció" → /kapcsolat]
```

Háttér: sötét, animált gradiens vagy egy rövid loop videó (ha van)

#### 4.2 3 PILLÉR (üzletágak)

3 kártya egymás mellett:

| Kártya | Ikon/kép | Headline | Leírás | CTA |
|--------|---------|----------|--------|-----|
| **Studio** | 🎬 | Social Media & Tartalomgyártás | „Forgatunk, vágunk, posztolunk – te csak az eredményt nézed." | [Konfigurátor →] |
| **Digital** | 💻 | Webfejlesztés & AI | „Modern weboldal 2 nap alatt. Ami máshol 2 hét." | [Konfigurátor →] |
| **Learning** | 🎓 | Online Oktatás | „15 napos challenge – építsd fel a saját rendszeredet." | [Megnézem →] |

#### 4.3 HOGYAN MŰKÖDIK (3 lépés)

```
1. „Válaszolj 5 kérdésre" → profil kitöltés
2. „Kapj személyre szabott ajánlatot" → konfigurátor ajánlás
3. „Indulunk 1 héten belül" → onboarding
```

#### 4.4 REFERENCIÁK

| Ügyfél | Egy mondat | Logó/kép |
|--------|-----------|---------|
| DH Prime | „Luxus ingatlan tartalom – organikus jelenlét felépítése a semmiből" | DH logó |
| Akadémia Plusz | „Jelentkezői érdeklődés generálás social médián" | Logó |
| DH Istenhegyi | „Csapat pozicionálás és online jelenlét a budai piacon" | DH logó |

#### 4.5 SZÁMOK

```
3 aktív ügyfél | 50+ legyártott videó | 3 szolgáltatás | 6 fős csapat
```

#### 4.6 CTA SZEKCIÓ

```
„Nem csomagot vásárolsz, hanem rendszert konfigurálsz."
[Összerakom a csomagom →]  [Ingyenes konzultáció →]
```

#### 4.7 FOOTER

- Logó + szlogen
- Linkek: Studio | Digital | Learning | Rólunk | Kapcsolat
- Adatvédelem | ÁSZF
- Social linkek (IG, TikTok, LinkedIn)
- © 2026 Scroll Studio Kft.

---

## 5. STUDIO OLDAL (/studio) – KONFIGURÁTOR

### Ez a legfontosabb oldal. Két belépési mód:

**Mód A: „Ajánljon nekem a rendszer"** → Profil kitöltés (6 kérdés) → Automatikus ajánlás → Módosítás → CTA

**Mód B: „Magam rakom össze"** → Egyenesen a konfigurátor lépésekhez

### Profil kérdések (Mód A):

1. **Mivel foglalkozik?** (dropdown: szépség, egészségügy, ingatlan, vendéglátás, szálláshely, fitness, ügyvéd, oktatás, építőipar, webshop, szolgáltató, személyes márka)
2. **Mi a fő célja?** (lead generálás / brand építés / értékesítés / közösség / toborzás)
3. **Havi büdzsé?** (<250K / 250-400K / 400-600K / 600K+)
4. **Milyen gyorsan kell eredmény?** (1-3 hó / 6-12 hó / nem sürgős)
5. **Van már social média?** (nincs / elavult / van de nem elég / van, skálázni akar)
6. **Cégméret?** (egyéni / 2-10 / 11-50 / 50+) – opcionális

**Ha büdzsé < 250K → Learning-re irányít** (nem a konfigurátorba)

### Konfigurátor lépések (Mód B, vagy Mód A után módosítás):

**LÉPÉS 1: Videó mennyiség** (kötelező)

| Szint | Videó/hó | Ár | Rövid leírás |
|-------|---------|-----|-------------|
| Alap | 8 | 250 000 Ft/hó | Stabil jelenlét, heti 2 videó |
| Standard | 10 | 320 000 Ft/hó | Legjobb ár-érték arány |
| Pro | 12 | 400 000 Ft/hó | Intenzív növekedés |
| Ultra | 15 | 500 000 Ft/hó | Maximális jelenlét |

**LÉPÉS 2: Brand hangvétel** (választó kártyák)

4 kártya: Komoly / Energikus / Laza / Vicces – mindegyikhez 1 mondat leírás + példa iparágak

**LÉPÉS 3: Platformok** (checkbox lista)

- [x] Instagram + TikTok (benne)
- [ ] + Facebook (+30 000 Ft/hó)
- [ ] + YouTube Shorts (+30 000 Ft/hó)
- [ ] + LinkedIn (+30 000 Ft/hó)
- [ ] Platformonként eltérő tartalom (+50 000 Ft/hó)

**LÉPÉS 4: Extrák** (checkbox lista, kategóriánként)

Instagram:
- [ ] Carousel posztok – havi 4 db (+40 000 Ft/hó)
- [ ] Carousel posztok – havi 8 db (+70 000 Ft/hó)
- [ ] IG Story kezelés – heti 3-4 (+50 000 Ft/hó)
- [ ] IG Story kezelés – napi (+80 000 Ft/hó)
- [ ] Carousel + Story kombó (+70 000 Ft/hó)
- [ ] Reels cover design (+15 000 Ft/hó)
- [ ] Highlights rendezés (+10 000 Ft egyszeri)
- [ ] Bio + Linktree optimalizálás (+10 000 Ft egyszeri)

Videó típusok:
- [ ] YouTube long-form – havi 2 db (+80 000 Ft/hó)
- [ ] YouTube long-form – havi 4 db (+140 000 Ft/hó)
- [ ] Podcast videó – havi 2 db (+60 000 Ft/hó)
- [ ] Interjú videó (+40 000 Ft/alkalom)
- [ ] Termékvideó (+35 000 Ft/db)
- [ ] Testimonial videó (+30 000 Ft/db)

Képes tartalom:
- [ ] Fotózás – forgatás mellett (+30 000 Ft/alkalom)
- [ ] Képes posztok – havi 4 db (+25 000 Ft/hó)
- [ ] Képes posztok – havi 8 db (+40 000 Ft/hó)

Szöveges tartalom:
- [ ] Egyedi copywriting (+20 000 Ft/hó)
- [ ] Blog cikk – havi 2 (+40 000 Ft/hó)
- [ ] Blog cikk – havi 4 (+70 000 Ft/hó)
- [ ] Hírlevél szövegírás – havi 2 (+25 000 Ft/hó)

AI tartalom:
- [ ] 25% AI-generált (-5% az alapárból)
- [ ] 50% AI-generált (-10% az alapárból)

Drón / speciális:
- [ ] Drón felvétel (+25 000 Ft/alkalom)
- [ ] Time-lapse (+20 000 Ft/alkalom)

Hirdetés:
- [ ] Meta Ads kezelés (+50 000 Ft/hó)
- [ ] Google Ads kezelés (+50 000 Ft/hó)
- [ ] TikTok Ads kezelés (+50 000 Ft/hó)
- [ ] Meta + Google kombó (+80 000 Ft/hó)
- [ ] Remarketing (+30 000 Ft/hó)

**LÉPÉS 5: Stratégia** (választó)

- ⚡ Gyors megtérülés (3 hó, magasabb díj, PPC ajánlott)
- 🌱 Hosszú távú építkezés (6-12 hó, -10% éves kedvezmény)

### Összesítő panel (jobb oldalt, sticky)

```
┌──────────────────────────┐
│ AZ ÖN CSOMAGJA           │
│                          │
│ Standard (10 videó) 320K │
│ + Facebook        +30K   │
│ + Carousel (4/hó) +40K   │
│ + Meta Ads        +50K   │
│ ──────────────────────── │
│ HAVI ÁR:      440 000 Ft │
│                          │
│ [📞 Kérem az ajánlatot]  │
│ [💬 Ingyenes konzultáció]│
└──────────────────────────┘
```

Az ár **valós időben frissül** ahogy pipálgat.

### CTA (az összesítő alján):

Kattintásra → form: Név + Cégnév + Email + Telefon + üzenet (opcionális)
→ Értesítés Viktornak/Eszternek → 24 órán belül visszahívjuk

---

## 6. DIGITAL OLDAL (/digital) – KONFIGURÁTOR

**Ugyanaz a logika mint a Studio-nál:** Profil kitöltés VAGY „Magam rakom össze"

### Profil kérdések: ugyanaz a 6 kérdés

### Konfigurátor elemek (checkbox lista):

Alap struktúra:
- ( ) Landing page – 1 szekció (100 000 Ft)
- ( ) Standard landing – 5-8 szekció (150 000 – 220 000 Ft)
- ( ) Bemutatkozó oldal – 3-5 oldal (250 000 – 400 000 Ft)
- ( ) Céges oldal – 5-10 oldal (500 000 – 900 000 Ft)
- [ ] + Extra szekció (+15 000 Ft/db)
- [ ] + Extra aloldal (+40 000 Ft/db)

Design:
- [x] Alap dizájn (benne)
- [ ] Egyedi UI/UX dizájn (+30 000 Ft)
- [ ] Prémium dizájn – animációk, parallax (+60 000 Ft)
- [ ] Dark mode (+20 000 Ft)

SEO:
- [ ] Alap SEO (+20 000 Ft)
- [ ] Haladó SEO (+50 000 Ft)
- [ ] Google My Business (+15 000 Ft)
- [ ] Lokális SEO csomag (+40 000 Ft)
- [ ] Google Search Console (+10 000 Ft)

Kapcsolat:
- [ ] Kontakt form – alap (+10 000 Ft)
- [ ] Kontakt form – haladó (+25 000 Ft)
- [ ] WhatsApp gomb (+5 000 Ft)
- [ ] Click-to-call (+5 000 Ft)
- [ ] Élő chat widget (+15 000 Ft)
- [ ] AI chatbot – egyszerű (+120 000 Ft)
- [ ] AI chatbot – haladó (+240 000 Ft)

Foglalás:
- [ ] Online időpontfoglaló – alap (+100 000 Ft)
- [ ] Online időpontfoglaló – haladó, fizetéssel (+180 000 Ft)
- [ ] Étterem asztalfoglalás (+120 000 Ft)
- [ ] Szálláshely foglalás (+200 000 Ft)
- [ ] Channel Manager – Booking/Airbnb (+300 000 – 500 000 Ft)

Tartalom:
- [ ] Blog – alap (+40 000 Ft)
- [ ] Blog – haladó CMS (+80 000 Ft)
- [ ] Hírlevél integráció (+25 000 Ft)

Galéria:
- [ ] Képgaléria – alap (+15 000 Ft)
- [ ] Képgaléria – haladó, szűrős (+35 000 Ft)
- [ ] Előtte-utána slider (+20 000 Ft)
- [ ] Virtuális túra beágyazás (+15 000 Ft)

E-commerce:
- [ ] Webshop – max 20 termék (+300 000 Ft)
- [ ] Webshop – 20-100 termék (+500 000 Ft)
- [ ] Fizetés – SimplePay (+60 000 Ft)
- [ ] Fizetés – Stripe (+50 000 Ft)
- [ ] Számlázás – szamlazz.hu (+80 000 Ft)
- [ ] SZÉP kártya (+40 000 Ft)
- [ ] Ajándékutalvány (+50 000 Ft)

Felhasználói:
- [ ] Bejelentkezés / regisztráció (+60 000 Ft)
- [ ] Zárt tartalom (+80 000 Ft)
- [ ] Ügyfélkapu (+120 000 Ft)
- [ ] Véleményezési rendszer (+40 000 Ft)

Automatizáció:
- [ ] Email automatizáció – welcome (+80 000 Ft)
- [ ] Email automatizáció – teljes nurturing (+150 000 Ft)
- [ ] CRM bevezetés (+100 000 – 200 000 Ft)
- [ ] GA4 beállítás (+15 000 Ft)
- [ ] Meta Pixel (+10 000 Ft)
- [ ] Google Tag Manager (+20 000 Ft)
- [ ] Social media feed (+15 000 Ft)

Jogi / technikai:
- [x] SSL (benne)
- [x] Hosting (benne)
- [x] Mobiloptimalizálás (benne)
- [ ] Domain beállítás (+10 000 Ft)
- [ ] Cookie consent (+10 000 Ft)
- [ ] Adatvédelmi nyilatkozat (+15 000 Ft)
- [ ] ÁSZF (+15 000 Ft)
- [ ] Sebesség optimalizálás (+20 000 Ft)
- [ ] Többnyelvű – +1 nyelv (+60 000 Ft/nyelv)

Havi karbantartás (retainer):
- ( ) Nincs retainer (egyszeri projekt)
- ( ) Alap karbantartás (30 000 Ft/hó)
- ( ) Aktív karbantartás (80 000 Ft/hó)
- ( ) Teljes menedzsment (150 000 – 300 000 Ft/hó)

Hirdetés (retainer):
- [ ] Google Ads (50 000 – 100 000 Ft/hó)
- [ ] Meta Ads (50 000 – 100 000 Ft/hó)
- [ ] SEO retainer (50 000 – 100 000 Ft/hó)

### Összesítő panel: ugyanaz mint a Studio-nál, de egyszeri + havi bontásban:

```
┌──────────────────────────────┐
│ AZ ÖN WEBOLDALA              │
│                              │
│ EGYSZERI:                    │
│ Standard landing     180 000 │
│ + SEO               +20 000 │
│ + Foglalás          +100 000 │
│ + GMB               +15 000 │
│ + Cookie + GDPR     +25 000 │
│ ──────────────────────────── │
│ EGYSZERI ÁR:     340 000 Ft  │
│                              │
│ HAVI:                        │
│ Alap karbantartás  30 000 Ft │
│                              │
│ [📞 Kérem az ajánlatot]      │
└──────────────────────────────┘
```

---

## 7. LEARNING OLDAL (/learning)

**Ez NEM konfigurátor – ez egy klasszikus sales landing page.** (A Learning platform külön domain-en lesz: learning.scrollstudio.hu)

### Szekciók:

1. **Hero:** „15 napos AI Challenge – építsd fel a saját működő AI rendszeredet"
   - CTA: [Jelentkezem – founding ár: 39 900 Ft]
   - Founding számláló: „47 hely maradt a founding árból"

2. **Két challenge vonal:**
   - AI Challenge (Viktor) – „AI a munkádban"
   - Brandépítés Challenge (Eszter) – „Social media brand a semmiből"

3. **Hogyan működik:** Day 1 → Day 5 (badge) → Day 10 (badge) → Day 15 (champion) – vizuális timeline

4. **Kinek szól:** Vállalkozó, irodai dolgozó, marketinges, KKV tulajdonos

5. **Árazás:**
   - Mini Challenge: 6 900 – 9 900 Ft
   - Core (founding): 39 900 Ft
   - Core (normál): 59 900 Ft
   - VIP: 79 900 Ft
   - Bundle (AI + Brand): 99 900 Ft

6. **GYIK:** 5-6 gyakori kérdés (Mennyi idő naponta? Kell-e előismeret? Visszakapom a pénzem? stb.)

7. **CTA:** „Nem kurzust kapsz, hanem rendszert."
   - [Jelentkezem a founding árért]
   - [Várólistára feliratkozom (Brand Challenge)]

---

## 8. RÓLUNK OLDAL (/rolunk)

### Misszió
> „Azért létezünk, hogy a magyar vállalkozások digitális jelenlétét a valós minőségükhöz emeljük — gyorsan, megfizethetően, mesterséges intelligenciával."

### Csapat (6 fő, fotóval)

| Személy | Szerep | 1 mondat |
|---------|--------|---------|
| **Eszter** | Ügyvezető | Brand stratégia és ügyfélkapcsolat |
| **Viktor** | CEO, Sales | Üzletfejlesztés és AI tréner |
| **Zoli** | Videograf | Forgatás és tartalomgyártás |
| **Dani** | AI fejlesztő | Webfejlesztés és automatizáció |
| **Barni** | Web fejlesztő | Weboldalak és platform építés |
| **Nóri** | Vágó & Sales | Videó utómunka és ügyfélszerzés |

### Értékek (röviden)
1. Sebesség intelligenciával
2. Őszinte partnerség
3. Eredmény, nem prezentáció

---

## 9. KAPCSOLAT OLDAL (/kapcsolat)

### Form mezők:
- Név (kötelező)
- Cégnév (opcionális)
- Email (kötelező)
- Telefon (kötelező)
- Mivel foglalkozik? (dropdown – ugyanaz mint a konfigurátor)
- Üzenet (szabad szöveg)
- [Küldés]

### Kontakt adatok:
- Email: (Eszter email)
- Telefon: (Viktor telefon)
- Cím: 1101 Budapest, Üllői út 124. (csak ha akarjátok)
- Social: IG, TikTok, LinkedIn linkek

---

## 10. KOMMUNIKÁCIÓS SZABÁLYOK (szövegíráshoz)

### Amit HASZNÁLUNK:
- Tegezés (a weboldalon tegezünk)
- Rövid, direkt mondatok
- Számok, eredmények (ne általánosság)
- CTA minden szekcióban
- „Nem X-et kapsz, hanem Y-t" struktúra

### Amit SOHA NEM HASZNÁLUNK:
- ~~„Olcsó"~~ → „Vállalkozóbarát ár"
- ~~„Mindent csinálunk"~~ → „3 fókuszált szolgáltatás"
- ~~„Garantáljuk az eredményt"~~ → „Mérhető eredményt hozunk"
- ~~„Online kurzus"~~ → „15 napos kihívás / challenge"
- ~~Technikai zsargon~~ (SEO, CRM, API) → érthetően magyarázzuk vagy kihagyjuk

### Headline stílusok:
- „Ami máshol 2 hét, az nálunk 2 nap."
- „Nem csomagot vásárolsz, hanem rendszert konfigurálsz."
- „Az ügyfeled nem a weboldaladért fizet – azért fizet, amit a weboldal hoz."
- „2 nap alatt kész. Nem sablon."

---

## 11. TECHNIKAI KÖVETELMÉNYEK

| Szempont | Elvárás |
|----------|---------|
| **Responsive** | Mobilon, tableten, desktopon tökéletes |
| **Sebesség** | PageSpeed 90+ (mobil + desktop) |
| **SEO** | Meta title/desc minden oldalon, sitemap.xml, robots.txt |
| **Analytics** | GA4 + Meta Pixel beépítve |
| **Form** | Email értesítés leadekről (Eszter + Viktor) |
| **Cookie** | GDPR sáv (elfogad/elutasít) |
| **Hosting** | Vercel (automatikus deploy) |
| **Konfigurátor** | Valós idejű ár-összesítő, nem kell backend – JS elég |
| **Domain** | scrollstudio.hu VAGY scrollstudio.com (Eszter dönt) |

---

## 12. PRIORITÁS

| Sorrend | Oldal | Mikor kell |
|---------|-------|-----------|
| **1** | Főoldal + Studio konfigurátor + Kapcsolat | **Ápr. 1-ig** (hideghívás indul) |
| **2** | Digital konfigurátor | **Ápr. első hét** |
| **3** | Learning landing | **Ápr. közepéig** (launch előkészítés) |
| **4** | Rólunk | **Ápr. végéig** |

**MVP (minimum ápr. 1-re):** Főoldal + Studio konfigurátor + Kontakt form. A többi jöhet utána.

---

## 13. REFERENCIA FÁJLOK (olvasd el)

Ezeket a fájlokat használd forrásként a szövegekhez és árazáshoz:

| Fájl | Mit találsz benne |
|------|-------------------|
| `STUDIO-ARAZO-KONFIGURATOR.md` | Studio minden eleme + árak + példák |
| `DIGITAL-ARAZO-KONFIGURATOR.md` | Digital minden eleme + árak + példák |
| `KONFIGURATOR-AJANLASI-LOGIKA.md` | Profil kérdések + ajánlási algoritmus + iparág-specifikus szövegek |
| `UZLETI-TERV-SCROLL-STUDIO.md` | Studio stratégia, sales, munkafolyamat |
| `UZLETI-TERV-SCROLL-DIGITAL.md` | Digital stratégia, pipeline, web audit |
| `UZLETI-TERV-SCROLL-LEARNING.md` | Learning challenge struktúra, árazás |
| `SCROLL_STUDIO_TELJES_MUKODES.md` | Brand irányelvek, hangvétel, vizuális szabályok |

---

*Scroll Studio – Weboldal Brief | v1.0 | 2026.03.26.*
