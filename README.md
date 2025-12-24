# Meta Ads Library Scraper 2025


- **🛡️ Advanced Anti-Detection** - Modern fingerprinting evasion and stealth techniques
- **🔍 GraphQL Interception** - Captures comprehensive ad data directly from API calls
- **🎭 Human Behavior Simulation** - Realistic mouse movements, scrolling, and delays
- **🌐 Proxy Support** - Built-in Apify proxy integration with residential IPs
- **📊 Comprehensive Data** - Ad creatives, targeting, performance metrics, and more

## 🆕 Novità 2025

- ✅ Bypass avanzato dei sistemi anti-bot di Facebook
- ✅ Intercettazione richieste GraphQL interne
- ✅ Simulazione comportamento umano realistico
- ✅ Supporto per tutti i tipi di ads (non solo politici)
- ✅ Rotazione User-Agent e fingerprint evasion
- ✅ Metodo HAR per estrazione legale al 100%

## 🛠️ Installazione Rapida

### 1. Setup Automatico
```bash
# Clona o scarica i file del progetto
cd V2Scraping

# Esegui setup automatico
python setup.py
```

### 2. Setup Manuale
```bash
# Installa dipendenze Python
pip install -r requirements.txt

# Installa browser Playwright
playwright install chromium
```

## 🚀 Quick Start

### Using Apify Console
1. **Import this Actor** to your Apify account
2. **Configure input parameters** (see Input Configuration below)
3. **Run the Actor** and monitor progress
4. **Download results** from the dataset

### Local Development
```bash
# 1. Install dependencies
npm install

# 2. Set up environment
cp .env.example .env
# Edit .env with your configuration

# 3. Run locally
npm start
```

## 📊 Output Data

The Actor saves comprehensive ad data to the Apify dataset with the following structure:

```json
{
  "adId": "123456789",
  "pageId": "987654321",
  "pageName": "Brand Name",
  "adContent": "Ad text content...",
  "startDate": "2025-01-01",
  "endDate": "2025-01-31",
  "spend": "1000-5000",
  "impressions": "10K-50K",
  "reach": "8K-40K",
  "demographics": {...},
  "platforms": ["Facebook", "Instagram"],
  "adCreative": {
    "images": [...],
    "videos": [...],
    "link_url": "..."
  },
  "targetingInfo": {...},
  "currency": "EUR",
  "isActive": true,
  "scrapedAt": "2025-01-15T10:30:00Z",
  "source": "graphql_interception"
}
```

### Struttura Dati CSV

| Campo | Descrizione |
|-------|-------------|
| `timestamp` | Data/ora estrazione |
| `ad_id` | ID univoco dell'ad |
| `page_name` | Nome della pagina |
| `page_id` | ID della pagina |
| `ad_text` | Testo dell'annuncio |
| `image_url` | URL immagine |
| `video_url` | URL video |
| `cta_text` | Testo call-to-action |
| `start_date` | Data inizio campagna |
| `end_date` | Data fine campagna |
| `impressions` | Numero impressioni |
| `spend` | Spesa pubblicitaria |
| `demographics` | Dati demografici |
| `platforms` | Piattaforme di pubblicazione |

## 🔧 Configurazione Avanzata

### File di Configurazione

Copia `config.env.example` in `.env` e modifica:

```env
# Impostazioni generali
HEADLESS=false
MAX_RESULTS=100
DELAY_MIN=1
DELAY_MAX=3

# Proxy (opzionale)
USE_PROXY=false
PROXY_LIST=proxy1:port,proxy2:port

# Anti-detection
SIMULATE_HUMAN=true
RANDOM_DELAYS=true
MOUSE_MOVEMENTS=true

# Output
OUTPUT_FORMAT=csv,json
OUTPUT_DIR=./results
```

### Personalizzazione Scraper

```python
# Esempio di utilizzo programmatico
from facebook_ad_library_scraper_2025 import FacebookAdLibraryScraper

async def custom_scraping():
    scraper = FacebookAdLibraryScraper(
        headless=True,
        use_proxy=False
    )
    
    await scraper.search_ads(
        search_term="your_brand",
        max_results=200
    )
    
    scraper.save_results("custom_output")
```

## 🛡️ Tecniche Anti-Detection

### Scraper Automatico
- **Playwright Stealth** - Evasione fingerprinting avanzata
- **User-Agent Rotation** - Rotazione automatica browser
- **Viewport Randomization** - Dimensioni schermo casuali
- **Human Behavior Simulation** - Movimenti mouse e scroll realistici
- **Request Timing** - Delay casuali tra richieste
- **GraphQL Interception** - Cattura dati API interne

### Metodo HAR
- **100% Legale** - Usa traffico web registrato manualmente
- **Zero Detection** - Nessun rischio di ban
- **Accesso Completo** - Tutti i tipi di ads disponibili
- **Dati Strutturati** - JSON dalle API interne Facebook

## 📈 Confronto Metodi

| Caratteristica | Scraper Automatico | Estrattore HAR |
|----------------|-------------------|----------------|
| **Legalità** | ⚠️ Zona grigia | ✅ 100% Legale |
| **Velocità** | 🚀 Veloce | 🐌 Manuale |
| **Rilevamento** | ⚠️ Possibile | ✅ Zero rischio |
| **Scalabilità** | ✅ Alta | ⚠️ Limitata |
| **Facilità** | ✅ Automatico | ⚠️ Richiede setup |
| **Dati** | ✅ Buona qualità | ✅ Qualità massima |
| **Manutenzione** | ⚠️ Aggiornamenti | ✅ Stabile |

## 🎯 Casi d'Uso

### Ricerca Competitiva
```bash
# Analizza ads dei competitor
python facebook_ad_library_scraper_2025.py
# Cerca: "competitor_name"
```

### Analisi Settore
```bash
# Estrai ads per categoria
python facebook_ad_library_scraper_2025.py
# Cerca: "fitness", "fashion", "tech"
```

### Monitoraggio Brand
```bash
# Monitora menzioni del tuo brand
python facebook_ad_library_scraper_2025.py
# Cerca: "your_brand_name"
```

### Ricerca Creativa
```bash
# Trova ispirazione per creatività
# Usa metodo HAR per sessioni lunghe
python facebook_har_extractor_2025.py session.har
```

## 🔍 Troubleshooting

### Problemi Comuni

**1. Scraper non trova ads:**
```bash
# Prova modalità non-headless per debug
python facebook_ad_library_scraper_2025.py
# Seleziona: headless = n
```

**2. Errori di installazione:**
```bash
# Reinstalla dipendenze
pip uninstall playwright playwright-stealth
pip install -r requirements.txt
playwright install chromium
```

**3. File HAR vuoto:**
- Assicurati di aver attivato "Preserve log" in DevTools
- Naviga attivamente nell'Ad Library durante la registrazione
- Registra per almeno 5-10 minuti

**4. Rilevamento anti-bot:**
- Usa il metodo HAR invece dello scraper automatico
- Riduci la velocità di scraping
- Usa proxy diversi

### Log e Debug

```bash
# Abilita logging dettagliato
export LOG_LEVEL=DEBUG
python facebook_ad_library_scraper_2025.py
```

## ⚖️ Note Legali

### ⚠️ IMPORTANTE - Leggere Attentamente

1. **Rispetta i Terms of Service** di Facebook
2. **Non abusare** del servizio (limita le richieste)
3. **Usa responsabilmente** i dati estratti
4. **Considera l'API ufficiale** quando possibile
5. **Il metodo HAR è raccomandato** per uso commerciale


## 🔄 Aggiornamenti

### v2.0 (2025)
- ✅ Tecniche anti-detection aggiornate
- ✅ Supporto GraphQL intercettazione
- ✅ Metodo HAR integrato
- ✅ Simulazione comportamento umano
- ✅ Setup automatico

### Roadmap
- 🔄 Supporto API ufficiale Facebook
- 🔄 Dashboard web per visualizzazione dati
- 🔄 Integrazione database
- 🔄 Analisi sentiment automatica
- 🔄 Export PowerBI/Tableau

---NiksHacks
