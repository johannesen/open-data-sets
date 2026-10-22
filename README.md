# OpenDataSets – Danske Åbne Datasæt & Lister

Dette repository indeholder **udelukkende færdigbehandlede, statiske datalister** i universelle tekst- og dataformater (`.csv`, `.json`, `.txt`).

> **Kilderepository & transformationsværktøjer:** [OpenData](https://git.p20.dev/christian/OpenData.git)  
> **Seneste synkronisering:** `2026-10-22 18:06:25 UTC`  
> **Samlet antal filer:** `186` lister (46.2 MB)

---

## 📂 Mappestruktur & Filformater

Hvert datasæt er organiseret i sin oprindelige emnemappe med dedikerede undermapper til hvert filformat:

```text
OpenDataSets/
├── README.md                 # Denne centrale dokumentation
├── dataset_manifest.json     # Integritets- og versionsmanifest (SHA-256)
├── cor_ordlister/            # Bøjningsformer, Wordle, Scrabble, længder m.m.
│   ├── wordle/
│   │   ├── csv/              # Wordle 5-bogstavers ord i CSV
│   │   ├── json/             # Wordle 5-bogstavers ord i JSON
│   │   └── txt/              # Wordle 5-bogstavers ord i ren tekstlinie-format
│   └── laengder/
│       ├── csv/
│       ├── json/
│       └── txt/
├── cor_ekstra/               # Grammatik, ordklasser, kuriositeter, stavefejl
│   ├── grammatik/
│   ├── kuriositeter/
│   ├── ordklasser/
│   └── stavefejl/
├── danske_aabne_datakilder/  # Register over 60+ åbne danske datakilder
├── dst_alkohol_tobak/        # Historiske tidsserier for salg af alkohol og tobak
└── dst_navne/                # Danmarks Statistiks mest populære navne (1985-2025)
```

---

## 📊 Oversigt over Datasæt

### 🔹 `cor_ekstra`
Ekstra sproglige udtræk fra COR & søgehjælpsdata – herunder grammatiske særtræk, ordklassekategorier, stavefejlsrettelser og ordspilskuriositeter.

- [**`cor_ekstra/grammatik`**](cor_ekstra/grammatik/) — Formater: `csv` (5), `json` (5), `txt` (3) (13 filer i alt)
- [**`cor_ekstra/kuriositeter`**](cor_ekstra/kuriositeter/) — Formater: `csv` (8), `json` (8), `txt` (5) (21 filer i alt)
- [**`cor_ekstra/ordklasser`**](cor_ekstra/ordklasser/) — Formater: `csv` (11), `json` (11), `txt` (10) (32 filer i alt)
- [**`cor_ekstra/stavefejl`**](cor_ekstra/stavefejl/) — Formater: `csv` (1), `json` (1) (2 filer i alt)

### 🔹 `cor_ordlister`
Danske ordlister baseret på Det Centrale Ordregister (COR) – velegnet til spil (Scrabble, Wordle), ordbøger og tekstanalyse.

- [**`cor_ordlister/grundformer`**](cor_ordlister/grundformer/) — Formater: `csv` (1), `json` (1), `txt` (1) (3 filer i alt)
- [**`cor_ordlister/laengder`**](cor_ordlister/laengder/) — Formater: `csv` (33), `json` (33), `txt` (33) (99 filer i alt)
- [**`cor_ordlister/palindromer`**](cor_ordlister/palindromer/) — Formater: `csv` (1), `json` (1), `txt` (1) (3 filer i alt)
- [**`cor_ordlister/scrabble`**](cor_ordlister/scrabble/) — Formater: `csv` (1), `json` (1), `txt` (1) (3 filer i alt)
- [**`cor_ordlister/wordle`**](cor_ordlister/wordle/) — Formater: `csv` (1), `json` (1), `txt` (1) (3 filer i alt)

### 🔹 `danske_aabne_datakilder`
Katalogiseret oversigt over åbne danske API'er og dataportaler med adresser, kategorier, licenser og adgangskrav.

- [**`danske_aabne_datakilder`**](danske_aabne_datakilder/) — Formater: `csv` (1), `json` (1) (2 filer i alt)

### 🔹 `dst_alkohol_tobak`
100+ års historiske data (1921–2025) over salg og forbrug af alkohol, cigaretter og tobak i Danmark fra Danmarks Statistik.

- [**`dst_alkohol_tobak`**](dst_alkohol_tobak/) — Formater: `csv` (2), `json` (2) (4 filer i alt)

### 🔹 `dst_navne`
Top 50-lister over nyfødtes navne i Danmark fra 1985 frem til seneste opgørelse (Danmarks Statistik).

- [**`dst_navne`**](dst_navne/) — Formater: `csv` (1) (1 filer i alt)

---

## 🔄 Integritet & Opdatering

Alle filers SHA-256 hash og størrelse registreres i [`dataset_manifest.json`](dataset_manifest.json).
Ved enhver synkronisering fra hoved-repositoriet verificeres filernes integritet og versionshistorik.

## 📜 Licenser & Kildeangivelse

- **COR (cor_ordlister, cor_ekstra):** Creative Commons CC0 1.0 Universal (Det Centrale Ordregister / Dansk Sprognævn).
- **Danmarks Statistik (dst_alkohol_tobak, dst_navne):** CC BY 4.0 (Danmarks Statistik).
- **Danske Åbne Datakilder:** CC0 1.0 Universal.

Se [OpenData](https://git.p20.dev/christian/OpenData.git) for rådata-scripts og opdateringsprocesser.