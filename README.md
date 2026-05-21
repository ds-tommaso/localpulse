# 🌿 Local Pulse

> **Mercati rionali italiani, digitalizzati con cura.**
> Zero sprechi. Filiera trasparente. Comunità locale.

---

## Indice

- [Il progetto](#il-progetto)
- [Obiettivi](#obiettivi)
- [Funzionalità](#funzionalità)
- [Tecnologie](#tecnologie)
- [Struttura del progetto](#struttura-del-progetto)
- [Come iniziare](#come-iniziare)
- [Pagine della webapp](#pagine-della-webapp)
- [Design System](#design-system)
- [Roadmap](#roadmap)
- [Impatto atteso](#impatto-atteso)
- [Autore](#autore)

---

## Il progetto

**Local Pulse** nasce dalla volontà di supportare i **mercati rionali italiani** digitalizzandone i processi per renderli competitivi nel contesto attuale, combattendo al contempo lo spreco alimentare.

L'obiettivo è dimostrare come la tecnologia possa essere uno strumento concreto per valorizzare la tradizione locale, riducendo l'impatto ambientale e creando un nuovo modello di business sostenibile.

I mercati di quartiere sono un patrimonio culturale italiano: offrono prodotti freschi, km zero, e un legame diretto tra produttore e consumatore. Eppure rischiano di scomparire per mancanza di strumenti digitali adeguati. Local Pulse colma questo gap.

---

## Obiettivi

| Obiettivo | Descrizione |
|-----------|-------------|
| 🌱 **Anti-spreco** | Ridurre il cibo invenduto a fine giornata attraverso notifiche e offerte last-minute |
| 🗺️ **Visibilità** | Portare i mercati online con profili, orari e disponibilità in tempo reale |
| 🧑‍🌾 **Sostenere i venditori** | Offrire dashboard analitiche semplici anche a chi non ha competenze tech |
| 🤝 **Comunità** | Connettere acquirenti locali con produttori del territorio |
| 📊 **Impatto misurabile** | Tracciare kg salvati, CO₂ evitata, acquisti locali per ogni utente |

---

## Funzionalità

### Per gli acquirenti
- 🔍 **Esplora mercati** — ricerca per prodotto, quartiere, categoria
- 🔔 **Notifiche anti-spreco** — avvisi quando i prodotti di fine giornata vanno in offerta
- 📦 **Pre-ordini** — prenota la tua cassetta settimanale e scegli il giorno di ritiro
- 🌱 **Tracker impatto** — monitora kg salvati dallo spreco e CO₂ evitata
- ❤️ **Preferiti** — salva i tuoi banchi e mercati di fiducia

### Per i venditori
- 🧑‍🌾 **Profilo banco** — storia, metodi di coltivazione, certificazioni visibili a tutti
- 📊 **Dashboard vendite** — analisi semplici su ordini, prodotti più venduti, fasce orarie
- 📦 **Gestione scorte** — aggiorna disponibilità in tempo reale, segnala prodotti in esaurimento
- 📣 **Promozioni** — crea offerte last-minute con un tap
- 📅 **Calendario presenze** — comunica orari e eventuali assenze al mercato

---

## Tecnologie

Questa versione è un **prototipo frontend** a singolo file HTML, senza dipendenze esterne da installare.

```
HTML5 + CSS3 + JavaScript Vanilla
```

| Tecnologia | Utilizzo |
|------------|----------|
| `backdrop-filter` CSS | Effetto Liquid Glass su card e navbar |
| CSS Custom Properties | Sistema di design token coerente |
| CSS Animations | Blob animati in background, transizioni UI |
| Google Fonts | Cormorant Garamond (display) + DM Sans (corpo) |
| JavaScript ES6 | Navigazione SPA client-side, toast, interazioni |

**Nessun framework, nessun bundle, nessuna dipendenza.** Apri il file e funziona.

---

## Struttura del progetto

```
local-pulse/
│
├── README.md                 # Questo file
│
├── docs/
    ├──  index.html           # Prototipo Webapp (single-file)

```

### Architettura SPA

La webapp è strutturata come **Single Page Application** client-side. Ogni "pagina" è un `<div>` con id univoco; la funzione `showPage(id)` gestisce la navigazione mostrando/nascondendo le sezioni.

```javascript
function showPage(id) {
  document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
  document.getElementById('page-' + id).classList.add('active');
  window.scrollTo(0, 0);
}
```

---

## Come iniziare

### Prerequisiti

Nessuno. Solo un browser moderno (Chrome 76+, Firefox 70+, Safari 14+, Edge 79+).

### Avvio

```bash
# Clona il repository
git clone https://github.com/tuousername/local-pulse.git

# Entra nella directory
cd local-pulse

# Apri nel browser (macOS)
open local-pulse.html

# Apri nel browser (Linux)
xdg-open local-pulse.html

# Apri nel browser (Windows)
start local-pulse.html
```

Oppure semplicemente **trascina `local-pulse.html` nel browser**.

### Sviluppo locale con live reload

```bash
# Con Node.js installato
npx serve .

# Con Python installato
python -m http.server 8080
```

---

## Pagine della webapp

| Pagina | Route (id) | Descrizione |
|--------|-----------|-------------|
| 🏠 Home | `home` | Hero, statistiche, features, CTA venditori |
| 🗺️ Esplora | `esplora` | Ricerca mercati, filtri per categoria, schede prodotto |
| 🔐 Login | `login` | Accesso email o Google |
| 📝 Registrazione | `register` | Selezione ruolo (acquirente / venditore) |
| 👤 Account | `account` | Profilo, ordini recenti, tracker impatto ambientale |
| 📬 Contatti | `contatti` | Info team, form di contatto, FAQ |

---

## Design System

### Filosofia: Liquid Glass

Il design si ispira all'estetica **Liquid Glass** — superfici traslucide con profondità, ispirate alle interfacce modern di Apple e al design material di nuova generazione.

```css
/* Formula base dell'effetto glass */
.glass {
  background: rgba(255, 255, 255, 0.18);
  backdrop-filter: blur(18px) saturate(180%);
  border: 1px solid rgba(255, 255, 255, 0.45);
  box-shadow: 0 8px 32px rgba(31, 38, 135, 0.10),
              inset 0 1px 0 rgba(255, 255, 255, 0.6);
}
```

### Palette colori

| Variabile | Hex | Utilizzo |
|-----------|-----|----------|
| `--accent-green` | `#2d6a4f` | Primario, CTA, accenti |
| `--accent-warm` | `#e07b39` | Secondario, highlights |
| `--accent-light` | `#b7e4c7` | Sfondi leggeri |
| `--bg-page` | `#f2ede4` | Sfondo generale |
| `--text-primary` | `#1a1a18` | Testo principale |
| `--text-secondary` | `#4a4a42` | Testo secondario |
| `--text-muted` | `#888876` | Testo terziario, placeholder |

### Tipografia

| Font | Peso | Utilizzo |
|------|------|----------|
| `Cormorant Garamond` | 300, 400, 600 | Titoli, display, numeri grandi |
| `DM Sans` | 300, 400, 500 | Corpo, UI, etichette |

### Componenti principali

- **`.glass`** — card standard con effetto traslucido
- **`.glass-dark`** — variante scura per contrasto
- **`.btn-primary`** — CTA verde principale
- **`.btn-ghost`** — azione secondaria trasparente
- **`.filter-chip`** — filtro tag selezionabile
- **`.market-card`** — scheda mercato con hover elevazione
- **`.auth-card`** — contenitore form autenticazione

---

## Roadmap

### v1.0 — Prototipo (attuale)
- [x] Interfaccia HTML/CSS/JS single-file
- [x] 6 pagine con navigazione SPA
- [x] Design Liquid Glass completo
- [x] Componenti UI: card mercati, form, account

### v1.1 — Backend integration
- [ ] API REST (Node.js / FastAPI)
- [ ] Database mercati e prodotti (PostgreSQL)
- [ ] Autenticazione JWT + OAuth (Google)
- [ ] Gestione sessioni utente

### v1.2 — Features core
- [ ] Geolocalizzazione e mappa interattiva (Leaflet.js)
- [ ] Sistema notifiche push (anti-spreco)
- [ ] Pre-ordini e carrello
- [ ] Dashboard venditori con grafici

### v2.0 — App mobile
- [ ] Progressive Web App (PWA)
- [ ] Notifiche push native
- [ ] Modalità offline
- [ ] App iOS/Android (React Native o Flutter)

### v2.1 — Sostenibilità avanzata
- [ ] Calcolo automatico impronta carbonica
- [ ] Certificazioni biologico/km zero verificate
- [ ] Report impatto mensile per comune
- [ ] Integrazione con programmi comunale anti-spreco

---

## Impatto atteso

Local Pulse si propone di generare impatto misurabile su tre livelli:

### 🌍 Ambientale
- Riduzione stimata del **35–40% dello spreco alimentare** nei mercati aderenti
- Diminuzione delle emissioni legate al trasporto grazie al km zero digitale
- Consapevolezza del consumatore attraverso il tracker impatto personale

### 💼 Economico
- Aumento del fatturato dei venditori grazie alla visibilità online
- Riduzione delle perdite da invenduto tramite le offerte last-minute
- Nuovo modello di business: abbonamenti cassette settimanali

### 🤝 Sociale
- Rafforzamento del tessuto commerciale di quartiere
- Accesso facilitato a prodotti freschi per famiglie a reddito variabile (offerte anti-spreco)
- Creazione di comunità locali attorno al concetto di consumo consapevole

---

## Autore

Progetto ideato e sviluppato nell'ambito di un percorso di ricerca sul tema della **digitalizzazione sostenibile del commercio locale tradizionale**.

**Tema:** *Local Pulse — Supportare i mercati rionali italiani attraverso la tecnologia*

---

<div align="center">

**Local Pulse** — *Mercati di quartiere, digitalizzati con cura* 🌿

</div>
