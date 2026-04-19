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
│   ├── zatepleni-fasady-bytovy-dum-poly-stavby.webp   ← hero bg
│   ├── zatepleni-omitka-rodinneho-domu.webp           ← sekce O mně
│   ├── rodinny-dum-pred-zateplenim.webp               ← před/po #1
│   ├── rodinny-dum-po-zatepleni-rekonstrukci.webp     ← před/po #1
│   ├── bytovy-dum-pred-rekonstrukci-fasady.webp       ← před/po #2
│   ├── bytovy-dum-po-rekonstrukci-fasada.webp         ← před/po #2
│   ├── zatepleni-fasady-novostavba.webp               ← galerie
│   ├── fasada-rodinneho-domu-po-zatepleni.webp        ← galerie
│   ├── zatepleni-bytoveho-domu-prubeh-praci.webp      ← galerie
│   ├── novostavba-rodinneho-domu-zatepleni.webp       ← galerie
│   └── zatepleni-polyfunkcniho-objektu.webp           ← galerie
└── Fotky/              # Původní JPG fotky (nezveřejňovat)
```

## Sekce webu (index.html)

| ID sekce | Obsah |
|----------|-------|
| `#uvod` | Hero – titulní obrazovka s fotkou bytového domu |
| `#sluzby` | 4 karty: Zateplení fasád, Fasádní omítky, Sádrokarton, Štuk |
| `#o-mne` | Profil Petra Poláčka + odkaz na NejŘemeslníci.cz |
| `#pred-po` | 2 páry před/po (rodinný dům + bytový dům) |
| `#galerie` | 6 fotek realizací |
| `#kde-pracujeme` | Oblast působnosti – seznam měst + okresy (local SEO) |
| `#recenze` | 4 reálné ověřené recenze z NejŘemeslníci.cz (5,0★), odkaz na zdroj |
| `#kontakt` | Telefon, e-mail, Instagram, Messenger |

## Design

- **Barvy:** Tmavá `#111827` + oranžová `#ea580c`
- **Font:** Inter (Google Fonts)
- **Styl:** Moderní, čistý, bez externích CSS frameworků
- **Responzivní:** Breakpointy na 820px, 700px, 480px

## Kontaktní údaje (Petra Poláčka)

- Telefon: 728 509 805
- E-mail: polacek85@gmail.com
- Instagram: @petan.poly_stavby
- Messenger: Poly stavby

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
2. Zaregistrovat v Google Search Console
3. Nahradit vymyšlené recenze reálnými
4. Případně přidat kontaktní formulář
