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

- **Web:** https://poly-stavby.vercel.app ✅ live
- **Doména:** poly-stavby.cz (zakoupena, čeká se na připojení k Vercel)
- **GitHub:** https://github.com/Vognarek-profil/Poly-stavby
- **Hosting:** Vercel (auto-deploy z main větve)
- **Google Search Console:** zatím nezaregistrováno – čeká se na připojení domény

## Struktura souborů

```
Poly stavby/
├── index.html          # Celý web (single-page)
├── favicon.svg         # SVG favicon (domeček, tmavý + oranžový)
├── robots.txt          # Povoluje vše, odkazuje na sitemap
├── sitemap.xml         # Jedna URL: https://poly-stavby.cz/
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
| `#uvod` | Hero – titulní obrazovka s fotkou bytového domu |
| `#sluzby` | 4 karty: Zateplení fasád, Fasádní omítky, Sádrokarton, Štuk |
| `#o-mne` | Profil Petra Poláčka + odkaz na NejŘemeslníci.cz |
| `#pred-po` | 2 páry před/po (rodinný dům + bytový dům) |
| `#proces` | 5 kroků komplexní rekonstrukce (holé zdivo → ocel → vlna → SDK → hotovo) |
| `#galerie` | 12 fotek realizací – fasády, rekonstrukce, interiéry |
| `#video` | Video z realizace (placeholder – čeká na optimalizované video) |
| `#kde-pracujeme` | Oblast působnosti – seznam měst + okresy (local SEO) |
| `#recenze` | 4 reálné ověřené recenze z NejŘemeslníci.cz (5,0★), odkaz na zdroj |
| `#kontakt` | Telefon, e-mail, Instagram, Facebook + dlaždice se sídlem a IČO |

## Design

- **Barvy:** Tmavá `#111827` + oranžová `#ea580c`
- **Font:** Inter (Google Fonts)
- **Styl:** Moderní, čistý, bez externích CSS frameworků
- **Responzivní:** Breakpointy na 820px, 700px, 480px

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
- [x] JSON-LD schema (HomeAndConstructionBusiness) – plná `PostalAddress`, `GeoCoordinates`, IČO, `foundingDate`, `serviceArea` 50 km, 22 `areaServed`, `hasOfferCatalog`
- [x] Geo meta tagy (`geo.region`, `geo.position`, `ICBM`)
- [x] robots.txt + sitemap.xml
- [x] Favicon
- [x] Preload hero image
- [x] WebP obrázky s SEO názvy a alt tagy
- [x] loading="lazy" + width/height na obrázcích
- [x] Sekce "Kde pracujeme" se seznamem měst (local SEO + user intent)
- [x] Adresa + IČO v kontaktu i patičce
- [x] Reálné ověřené recenze z NejŘemeslníci.cz + `AggregateRating` + `Review` entity ve schema (5,0★, 4 recenze)
- [ ] Google Search Console – po připojení domény
- [ ] Upřesnit pracovní dobu → doplnit `openingHours` do schema

## Další plánované kroky

1. Připojit doménu poly-stavby.cz k Vercel (DNS záznamy u registrátora)
2. Zaregistrovat v Google Search Console po připojení domény
3. Založit Google Business Profile (pro "blízko mě" a mapy – klíčové pro local SEO)
4. Upřesnit pracovní dobu Petra a doplnit `openingHours` do JSON-LD schema
5. Průběžně doplňovat nové ověřené recenze z NejŘemeslníci
6. **Optimalizovat video** (`YouCut_20260421_175048497.mp4`, 114 MB) → spustit `optimize_video.ps1`, nahradit placeholder v sekci `#video`
7. Případně přidat kontaktní formulář

## Optimalizace videa – doporučení

Původní video má 114 MB – to je pro web nepoužitelné (i modernímu uživateli by se načítalo desítky vteřin). Cíl: **pod 8 MB**.

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

**Postup:**
1. `winget install -e --id Gyan.FFmpeg` (instalace ffmpeg)
2. Otevřít nové PowerShell okno (kvůli PATH)
3. V rootu projektu: `.\optimize_video.ps1`
4. V `index.html` v sekci `#video` odkomentovat `<video>` blok a smazat `.video-placeholder` div
