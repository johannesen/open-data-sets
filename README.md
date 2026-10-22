# OpenDataSets – Danske Åbne Datasæt & Lister / Danish Open Datasets

[🇩🇰 Dansk](#dansk) | [🇬🇧 English](#english)

---

<a name="dansk"></a>
## 🇩🇰 Dansk

Dette repository indeholder **udelukkende færdigbehandlede, statiske datalister** i universelle dataformater (`.csv`, `.json`, `.txt`).

> **Kilderepository & bygge-scripts:** [OpenData](https://git.p20.dev/christian/OpenData.git)  
> **Seneste synkronisering:** `2026-10-22 18:20:21 UTC`  
> **Samlet antal lister:** `186` filer (46.2 MB)

### 📂 Mappestruktur & Filformater

Hvert datasæt følger kildens mappehierarki med dedikerede undermapper til hver filtype (`csv/`, `json/`, `txt/`):

```text
OpenDataSets/
├── README.md                 # Denne centrale tosprogede dokumentation
├── dataset_manifest.json     # Integritets- og versionsmanifest (SHA-256 for alle filer)
├── cor_ordlister/            # Bøjningsformer, Wordle, Scrabble, længder m.m.
│   ├── wordle/
│   │   ├── csv/              # CSV-format
│   │   ├── json/             # JSON-format
│   │   └── txt/              # Rent linje-tekstformat (UTF-8)
│   └── laengder/
│       ├── csv/
│       ├── json/
│       └── txt/
├── cor_ekstra/               # Grammatik, ordklasser, kuriositeter, stavefejl
│   ├── grammatik/ (csv/, json/, txt/)
│   ├── kuriositeter/ (csv/, json/, txt/)
│   ├── ordklasser/ (csv/, json/, txt/)
│   └── stavefejl/ (csv/, json/)
├── danske_aabne_datakilder/  # Register over 60+ åbne danske datakilder (csv/, json/)
├── dst_alkohol_tobak/        # Tidsserier for alkohol & tobak 1921–2025 (csv/, json/)
└── dst_navne/                # Nyfødtes navne top 50 1985–2025 (csv/)
```

### 📊 Oversigt over Datasæt

#### 🔹 `cor_ekstra`
Ekstra sproglige udtræk fra COR & søgehjælpsdata – herunder grammatiske særtræk, ordklassekategorier, stavefejlsrettelser og ordspilskuriositeter.

- [**`cor_ekstra/grammatik`**](cor_ekstra/grammatik/) — Formater: `csv` (5), `json` (5), `txt` (3) (13 filer i alt)
- [**`cor_ekstra/kuriositeter`**](cor_ekstra/kuriositeter/) — Formater: `csv` (8), `json` (8), `txt` (5) (21 filer i alt)
- [**`cor_ekstra/ordklasser`**](cor_ekstra/ordklasser/) — Formater: `csv` (11), `json` (11), `txt` (10) (32 filer i alt)
- [**`cor_ekstra/stavefejl`**](cor_ekstra/stavefejl/) — Formater: `csv` (1), `json` (1) (2 filer i alt)

#### 🔹 `cor_ordlister`
Danske ordlister baseret på Det Centrale Ordregister (COR) – velegnet til spil (Scrabble, Wordle), ordbøger og tekstanalyse.

- [**`cor_ordlister/grundformer`**](cor_ordlister/grundformer/) — Formater: `csv` (1), `json` (1), `txt` (1) (3 filer i alt)
- [**`cor_ordlister/laengder`**](cor_ordlister/laengder/) — Formater: `csv` (33), `json` (33), `txt` (33) (99 filer i alt)
- [**`cor_ordlister/palindromer`**](cor_ordlister/palindromer/) — Formater: `csv` (1), `json` (1), `txt` (1) (3 filer i alt)
- [**`cor_ordlister/scrabble`**](cor_ordlister/scrabble/) — Formater: `csv` (1), `json` (1), `txt` (1) (3 filer i alt)
- [**`cor_ordlister/wordle`**](cor_ordlister/wordle/) — Formater: `csv` (1), `json` (1), `txt` (1) (3 filer i alt)

#### 🔹 `danske_aabne_datakilder`
Katalogiseret oversigt over 60+ åbne danske API'er og dataportaler med adresser, kategorier, licenser og adgangskrav.

- [**`danske_aabne_datakilder`**](danske_aabne_datakilder/) — Formater: `csv` (1), `json` (1) (2 filer i alt)

#### 🔹 `dst_alkohol_tobak`
100+ års historiske data (1921–2025) over salg og forbrug af alkohol, cigaretter og tobak i Danmark fra Danmarks Statistik.

- [**`dst_alkohol_tobak`**](dst_alkohol_tobak/) — Formater: `csv` (2), `json` (2) (4 filer i alt)

#### 🔹 `dst_navne`
Top 50-lister over nyfødtes navne i Danmark fra 1985 frem til seneste opgørelse (Danmarks Statistik).

- [**`dst_navne`**](dst_navne/) — Formater: `csv` (1) (1 filer i alt)

### 🔄 Integritet & Opdatering

Alle filers SHA-256 hash og størrelse registreres i [`dataset_manifest.json`](dataset_manifest.json).
Ved enhver synkronisering fra kilderepositoriet verificeres filernes integritet og versionshistorik automatisk.

### 📜 Licenser & Kildeangivelse

- **COR (cor_ordlister, cor_ekstra):** Creative Commons CC0 1.0 Universal (Det Centrale Ordregister / Dansk Sprognævn).
- **Danmarks Statistik (dst_alkohol_tobak, dst_navne):** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.da) (Danmarks Statistik).
- **Danske Åbne Datakilder:** [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/).

For transformerscripts, rådata-downloaders og pipeline-koder henvises til [OpenData](https://git.p20.dev/christian/OpenData.git).

---

<a name="english"></a>
## 🇬🇧 English

This repository contains **exclusively static, processed data lists** in open universal formats (`.csv`, `.json`, `.txt`).

> **Source repository & pipelines:** [OpenData](https://git.p20.dev/christian/OpenData.git)  
> **Last synchronized:** `2026-10-22 18:20:21 UTC`  
> **Total datasets:** `186` files (46.2 MB)

### 📂 Directory Structure & Formats

All datasets retain the logical domain taxonomy of the source repository, organized into dedicated subdirectories per file extension (`csv/`, `json/`, `txt/`):

```text
OpenDataSets/
├── README.md                 # Bilingual root documentation
├── dataset_manifest.json     # Integrity manifest with SHA-256 hashes
├── cor_ordlister/            # Word lists, inflections, lengths, Scrabble, Wordle
│   ├── wordle/
│   │   ├── csv/
│   │   ├── json/
│   │   └── txt/
├── cor_ekstra/               # Grammatical anomalies, curiosities, 10 POS categories, typos
├── danske_aabne_datakilder/  # Directory of 60+ Danish open data sources and APIs
├── dst_alkohol_tobak/        # Historical sales & consumption series 1921–2025
└── dst_navne/                # Top 50 newborn baby names 1985–2025
```

### 📊 Dataset Catalog

#### 🔹 `cor_ekstra`
Linguistic subsets and curio lists from COR & search assistance data – grammar anomalies, 10 parts of speech, typos with corrections, and word puzzles.

- [**`cor_ekstra/grammatik`**](cor_ekstra/grammatik/) — Formats: `csv` (5), `json` (5), `txt` (3) (13 files total)
- [**`cor_ekstra/kuriositeter`**](cor_ekstra/kuriositeter/) — Formats: `csv` (8), `json` (8), `txt` (5) (21 files total)
- [**`cor_ekstra/ordklasser`**](cor_ekstra/ordklasser/) — Formats: `csv` (11), `json` (11), `txt` (10) (32 files total)
- [**`cor_ekstra/stavefejl`**](cor_ekstra/stavefejl/) — Formats: `csv` (1), `json` (1) (2 files total)

#### 🔹 `cor_ordlister`
Danish word lists derived from The Central Word Register (COR) – ideal for games (Scrabble, Wordle), spell-checkers, and NLP.

- [**`cor_ordlister/grundformer`**](cor_ordlister/grundformer/) — Formats: `csv` (1), `json` (1), `txt` (1) (3 files total)
- [**`cor_ordlister/laengder`**](cor_ordlister/laengder/) — Formats: `csv` (33), `json` (33), `txt` (33) (99 files total)
- [**`cor_ordlister/palindromer`**](cor_ordlister/palindromer/) — Formats: `csv` (1), `json` (1), `txt` (1) (3 files total)
- [**`cor_ordlister/scrabble`**](cor_ordlister/scrabble/) — Formats: `csv` (1), `json` (1), `txt` (1) (3 files total)
- [**`cor_ordlister/wordle`**](cor_ordlister/wordle/) — Formats: `csv` (1), `json` (1), `txt` (1) (3 files total)

#### 🔹 `danske_aabne_datakilder`
Verified directory of 60+ Danish open data sources and APIs with endpoints, domains, licenses, and access requirements.

- [**`danske_aabne_datakilder`**](danske_aabne_datakilder/) — Formats: `csv` (1), `json` (1) (2 files total)

#### 🔹 `dst_alkohol_tobak`
100+ years of historical data (1921–2025) on sales and consumption of alcohol, cigarettes, and tobacco in Denmark (Statistics Denmark).

- [**`dst_alkohol_tobak`**](dst_alkohol_tobak/) — Formats: `csv` (2), `json` (2) (4 files total)

#### 🔹 `dst_navne`
Top 50 baby names for newborns in Denmark from 1985 to latest official releases (Statistics Denmark).

- [**`dst_navne`**](dst_navne/) — Formats: `csv` (1) (1 files total)

### 🔄 Data Integrity

Each release computes SHA-256 checksums stored in [`dataset_manifest.json`](dataset_manifest.json) to guarantee immutability and verifiable pedigree.

### 📜 Licenses & Attribution

- **COR (cor_ordlister, cor_ekstra):** Creative Commons CC0 1.0 Universal (Det Centrale Ordregister / Danish Language Council).
- **Statistics Denmark (dst_alkohol_tobak, dst_navne):** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) (Danmarks Statistik).
- **Danish Open Data Catalog:** [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/).

For raw data downloaders, build scripts, and MCP server integrations, visit [OpenData](https://git.p20.dev/christian/OpenData.git).