# Poly stavby – CLAUDE.md

> Aktualizuj tento soubor po každé větší změně v projektu.

## O projektu

Web živnostníka **Petra Poláčka (Poly stavby)** – zateplení fasád, fasádní omítky, sádrokartonářské práce a vnitřní omítky (štuk) na Jižní Moravě.

## Firemní údaje

- **Jméno:** Petr Poláček (OSVČ)
- **IČO:** 87808641
- **OSVČ od:** 27. 4. 2011 (→ 15 let zkušeností v r. 2026)
- **Sídlo:** Moutnice 122, 664 55 Moutnice, okres Brno-venkov, Jihomoravský kraj
- **GPS:** 49.0403 N, 16.7283 E
- **Oblast působnosti:** Moutnice + okruh 50 km (Brno, Brno-venkov, Vyškov, Hodonín, Břeclav, Blansko)
- **NACE:** 43120 (elektroinstalace), 433 (dokončovací stavební práce)

## Stav projektu

- **Web:** https://www.poly-stavby.cz ✅ live (kanonická adresa je **s www**)
- **Doména:** poly-stavby.cz připojena k Vercel; ve Vercelu je primární `www.poly-stavby.cz`, apex `poly-stavby.cz` se na ni přesměrovává (307)
- **poly-stavby.vercel.app:** přesměrováno 301 na www přes `vercel.json` (aby nevznikala duplicita v Googlu)
- **GitHub:** https://github.com/Vognarek-profil/Poly-stavby
- **Hosting:** Vercel (auto-deploy z main větve)
- **Poslední aktualizace:** 2026-08-30 – sjednocení domény na www, sekce FAQ + FAQPage schema
- **Google Search Console:** ověřovací meta tag je v `<head>`. **Property musí být pro `www.poly-stavby.cz`** (nebo Domain property `poly-stavby.cz`, která pokryje obě varianty). Property jen pro apex bez www ukazuje samá přesměrování a nula indexovaných stránek.

## Struktura souborů

```
Poly stavby/
├── index.html          # Celý web (single-page)
├── favicon.svg         # SVG favicon (domeček, tmavý + oranžový)
├── robots.txt          # Povoluje vše, odkazuje na sitemap
├── sitemap.xml         # Jedna URL: https://www.poly-stavby.cz/
├── vercel.json         # 301 redirect z poly-stavby.vercel.app na www.poly-stavby.cz
├── .gitignore
├── fotky-web/          # Optimalizované WebP obrázky (SEO názvy)
│   ├── uvodni-zatepleni-bytoveho-domu-poly-stavby.webp ← hero bg (nová úvodní)
│   ├── zatepleni-omitka-rodinneho-domu.webp            ← sekce O mně
│   ├── rodinny-dum-pred-zateplenim.webp                ← před/po #1
│   ├── rodinny-dum-po-zatepleni-rekonstrukci.webp      ← před/po #1
│   ├── bytovy-dum-pred-rekonstrukci-fasady.webp        ← před/po #2
│   ├── bytovy-dum-po-rekonstrukci-fasada.webp          ← před/po #2
│   ├── rekonstrukce-chaty-puvodni-stav-hole-cihly.webp ← proces #1
│   ├── rekonstrukce-interieru-ocelova-konstrukce-pricek.webp ← proces #2
│   ├── zatepleni-podkrovi-mineralni-vlna.webp          ← proces #3
│   ├── sadrokartonove-pricky-rekonstrukce-interieru.webp ← proces #4
│   ├── podkrovi-se-stresnim-oknem-rekonstrukce.webp    ← proces #5
│   ├── zatepleni-fasady-bytovy-dum-poly-stavby.webp    ← galerie
│   ├── rodinny-dum-po-zatepleni-kremova-fasada.webp    ← galerie
│   ├── rodinny-dum-po-zatepleni-zelena-bila-fasada.webp ← galerie
│   ├── zatepleni-fasady-novostavba.webp                ← galerie
│   ├── detail-fasady-po-zatepleni-rodinny-dum.webp     ← galerie
│   ├── fasada-rodinneho-domu-po-zatepleni.webp         ← galerie
│   ├── zatepleni-bytoveho-domu-prubeh-praci.webp       ← galerie
│   ├── rodinny-dum-zatepleni-fasady-leseni.webp        ← galerie
│   ├── zatepleni-fasady-rekonstrukce-radovy-dum.webp   ← galerie
│   ├── novostavba-rodinneho-domu-zatepleni.webp        ← galerie
│   ├── zatepleni-polyfunkcniho-objektu.webp            ← galerie
│   ├── sadrokartonove-steny-schodiste-rekonstrukce.webp ← galerie
│   ├── podkrovi-po-sadrokartonu-pred-malovanim.webp    ← (rezerva)
│   ├── sadrokartonove-podkrovi-stresni-okno.webp       ← (rezerva)
│   ├── rodinny-dum-pred-a-po-zatepleni-fasady.webp     ← (rezerva – koláž)
│   ├── zatepleni-radoveho-domu-prubeh.webp             ← (rezerva – koláž)
│   ├── zatepleni-podkrovi-parozabrana-folie.webp       ← (rezerva)
│   ├── rekonstrukce-podkrovi-puvodni-drevene-tramy.webp ← (rezerva)
│   └── rekonstrukce-podkrovi-prubeh-praci.webp         ← (rezerva)
├── fotky-web/video/    # Optimalizované video (zatím prázdné, viz optimize_video.ps1)
├── Fotky/              # Původní JPG fotky (nezveřejňovat, v .gitignore)
├── fotky nove/         # Nové JPG + video (nezveřejňovat, v .gitignore)
├── convert_to_webp.py  # Lokální skript pro konverzi JPG→WebP (gitignore)
└── optimize_video.ps1  # Lokální skript pro konverzi videa přes ffmpeg (gitignore)
```

## Sekce webu (index.html)

| ID sekce | Obsah |
|----------|-------|
| `#uvod` | Hero – zateplený bytový dům (šedá fasáda, Cupra), badge „15 let zkušeností", 3 stat boxy |
| `#sluzby` | 4 karty: Zateplení fasád, Fasádní omítky, Sádrokarton, Štuk |
| `#o-mne` | Profil Petra Poláčka + odkaz na NejŘemeslníci.cz |
| `#pred-po` | 2 páry před/po (rodinný dům + bytový dům) |
| `#proces` | 5 kroků komplexní rekonstrukce (holé zdivo → ocel → vlna → SDK → hotovo) |
| `#galerie` | 12 fotek realizací – fasády, rekonstrukce, interiéry |
| `#video` | Video z realizace (placeholder – čeká na optimalizované video) |
| `#kde-pracujeme` | Oblast působnosti – seznam měst + okresy (local SEO) |
| `#faq` | 11 častých otázek ve 3 kategoriích (zateplení / sádrokarton / průběh a záruky) + pruh 4 fází spolupráce. `<details>`/`<summary>`, bez JS. Zdroj textů: `poly-stavby_faq.md` (gitignore) – při přepisu převedeno do 1. os. j. č. |
| `#recenze` | 4 reálné ověřené recenze z NejŘemeslníci.cz (5,0★), odkaz na zdroj |
| `#kontakt` | Telefon, e-mail, Instagram, Facebook + dlaždice se sídlem a IČO |

## Tón webu

Web mluví za **jednoho člověka: 1. osoba jednotného čísla** („nabízím", „pracuji", „přijedu", „doporučuji"). Petr je OSVČ, ne firma s týmem.
Množné číslo je na webu správně jen v **citacích recenzí** – tam mluví zákazník. Nové texty (i podklady dodané v MD) proto vždy převeď do jednotného čísla.

## Design

- **Barvy:** Tmavá `#111827` + oranžová `#ea580c`
- **Font:** Inter (Google Fonts)
- **Styl:** Moderní, čistý, bez externích CSS frameworků
- **Responzivní:** Breakpointy na 820 px (mobilní nav + 2 sloupce galerie + 3 sloupce proces) a 480 px (1 sloupec galerie, 2 sloupce proces)

## Kontaktní údaje (Petra Poláčka)

- Telefon: 728 509 805
- E-mail: polacek85@gmail.com
- Instagram: [@petan.poly_stavby](https://www.instagram.com/petan.poly_stavby)
- Facebook: [facebook.com/Polystavby](https://www.facebook.com/Polystavby)
- NejŘemeslníci: [profil 486432](https://www.nejremeslnici.cz/profil/486432-petr-polacek)
- Sídlo: Moutnice 122, 664 55 Moutnice
- IČO: 87808641

## SEO stav

- [x] Title, meta description, keywords
- [x] Canonical URL
- [x] Open Graph (Facebook, LinkedIn)
- [x] Twitter Card
- [x] Kanonická doména sjednocena na `https://www.poly-stavby.cz/` (canonical, og:url, og:image, twitter:image, schema, sitemap, robots)
- [x] JSON-LD schema (FAQPage) – 11 otázek, generováno přímo z textu viditelného v sekci `#faq`
- [x] JSON-LD schema (HomeAndConstructionBusiness) – plná `PostalAddress`, `GeoCoordinates`, IČO, `foundingDate`, `serviceArea` 50 km, 22 `areaServed`, `hasOfferCatalog`
- [x] Geo meta tagy (`geo.region`, `geo.position`, `ICBM`)
- [x] robots.txt + sitemap.xml
- [x] Favicon
- [x] Preload hero image
- [x] WebP obrázky s SEO názvy a alt tagy (31 fotek ve `fotky-web/`, všechny `<img>` mají popisný český alt)
- [x] loading="lazy" + width/height na obrázcích
- [x] Sekce "Kde pracujeme" se seznamem měst (local SEO + user intent)
- [x] Adresa + IČO v kontaktu i patičce
- [x] Reálné ověřené recenze z NejŘemeslníci.cz + `AggregateRating` + `Review` entity ve schema (5,0★, 4 recenze)
- [ ] Google Search Console – ověřit property pro www, odeslat sitemapu, „Prověřit URL" → Požádat o indexování
- [ ] Upřesnit pracovní dobu → doplnit `openingHours` do schema

## Další plánované kroky

1. V Search Console mít property pro **www.poly-stavby.cz** (ideálně Domain property `poly-stavby.cz` přes DNS TXT – pokryje www i apex)
2. Odeslat `https://www.poly-stavby.cz/sitemap.xml` a přes „Prověřit URL" požádat o indexování
3. Založit Google Business Profile (pro "blízko mě" a mapy – klíčové pro local SEO)
4. Upřesnit pracovní dobu Petra a doplnit `openingHours` do JSON-LD schema
5. Průběžně doplňovat nové ověřené recenze z NejŘemeslníci
6. **Dořešit video** pro sekci `#video`:
   - Původní 114 MB → nepoužitelné pro web (cíl pod ~8 MB)
   - Petr zkouší variantu mobilního exportu (po zkrácení na 30–40 s)
   - Alternativa: `optimize_video.ps1` (vyžaduje ffmpeg) nebo YouTube embed
   - Po dodání odkomentovat `<video>` blok v `index.html` a smazat `.video-placeholder`
7. Případně přidat kontaktní formulář

## Optimalizace videa – doporučení

Cíl: **pod 8 MB** (v krajním případě do 15 MB). 50 MB+ je pro mobilní uživatele nepoužitelné.

**Nejdůležitější:** délka. 84sekundové video = minimálně 10–15 MB při rozumné kvalitě. Na webu stejně 98 % návštěvníků odchází z videa do 15 s – **ideální délka pro web ukázku je 20–40 s**. Nejdřív sestříhat, pak komprimovat.

**Doporučený formát pro web:**
- **MP4 (H.264)** – univerzální, běží všude (Safari, iOS, starší Android)
- **WebM (VP9)** – ~25–40 % menší při stejné kvalitě, moderní prohlížeče (Chrome, Firefox, Edge)
- Obojí v jednom `<video>` tagu přes `<source>` – prohlížeč si vybere podporovaný.

**Parametry:**
- Rozlišení **1280×720** (720p) – pro ukázku z realizace plně dostačuje
- Bitrate ~1,5 Mbps (CRF 28 pro H.264, CRF 34 pro VP9)
- **Bez zvuku** (`-an` v ffmpeg) – ušetří ~10–20 % a stejně poběží muted autoplay
- `faststart` pro MP4 (rychlejší start přehrávání)
- Poster obrázek jako `.webp` – vidí se před načtením, nic nestahuje navíc

**Postup (ffmpeg):**
1. `winget install -e --id Gyan.FFmpeg` (instalace ffmpeg)
2. Otevřít nové PowerShell okno (kvůli PATH)
3. V rootu projektu: `.\optimize_video.ps1`
4. V `index.html` v sekci `#video` odkomentovat `<video>` blok a smazat `.video-placeholder` div

**Alternativa – YouTube embed:**
Pokud nechceš řešit ffmpeg, nahraj video na YouTube (třeba jako Unlisted) a sekci `#video` přepiš na `<iframe>` embed. Plusy: 0 MB v repu, neomezená délka. Minusy: YouTube logo a doporučená videa na konci.

## Changelog

- **2026-08-30** – Sjednocení tónu webu na 1. os. j. č.: FAQ (20 míst) + „Naše realizace" → „Moje realizace" v nadpisu `#pred-po` a v hero tlačítku; `FAQPage` schema přegenerováno, aby doslova sedělo s viditelným textem
- **2026-08-30** – Sjednocení kanonické domény na `www` (8 URL v HTML + sitemap + robots), `vercel.json` s 301 z `poly-stavby.vercel.app`, nová sekce `#faq` (11 otázek, 4 fáze spolupráce) + `FAQPage` JSON-LD, odkaz FAQ v navigaci, aktualizovaný `lastmod` v sitemapě

- **2026-04-24** – 19 nových WebP fotek, nová hero, sekce `#proces` (5 kroků rekonstrukce podkroví), sekce `#video` (placeholder), galerie 6→12, nav rozšířen o „Rekonstrukce", mobilní breakpoint 700→820 px (commit `0a83d21`)
- **2026-04-15** – Google Search Console verification meta tag (commit `26d606c`)
- **2026-04-15** – Local business schema, sekce „Kde pracuji", ověřené recenze z NejŘemeslníci (commit `810174e`)
- **2026-04-15** – Počáteční verze webu (commit `5f572b5`)
