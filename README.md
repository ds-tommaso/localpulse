# LocalPulse 🌿

> **Digitalizzare la tradizione per abbattere lo spreco alimentare.**  
> Progetto di **Angelica Goffredo**

![HTML](https://img.shields.io/badge/HTML5-single--file-e07b39?style=flat-square&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-Liquid%20Glass-2d6a4f?style=flat-square&logo=css3&logoColor=white)
![JS](https://img.shields.io/badge/JavaScript-Vanilla%20ES6-f4c896?style=flat-square&logo=javascript&logoColor=black)
![License](https://img.shields.io/badge/Licenza-MIT-b7e4c7?style=flat-square)

---

## Indice

- [Il progetto](#il-progetto)
- [Contesto e dati](#contesto-e-dati)
- [Innovazione tecnologica](#innovazione-tecnologica)
- [Posizionamento competitivo](#posizionamento-competitivo)
- [Business plan](#business-plan)
- [Funzionalità della webapp](#funzionalità-della-webapp)
- [Tecnologie](#tecnologie)
- [Struttura del progetto](#struttura-del-progetto)
- [Come iniziare](#come-iniziare)
- [Pagine della webapp](#pagine-della-webapp)
- [Design system](#design-system)
- [Roadmap](#roadmap)
- [Impatto atteso](#impatto-atteso)
- [Autrice](#autrice)

---

## Il progetto

**LocalPulse** è un ecosistema digitale "Phygital" che trasforma i mercati rionali italiani in piattaforme connesse, senza snaturarne l'identità.

L'idea nasce da un'osservazione concreta: i mercati di quartiere sono un patrimonio culturale e gastronomico italiano, ma soffrono un gap tecnologico crescente che favorisce la Grande Distribuzione Organizzata a scapito della qualità e della prossimità locale. LocalPulse colma questo divario con strumenti digitali accessibili a tutti — venditori inclusi, anche senza competenze tecniche.

La **mission** è creare un nuovo modello di business sostenibile che riduca lo spreco alimentare, aumenti i margini dei venditori e rilanci le micro-economie di quartiere.

---

## Contesto e dati

I tre problemi strutturali che LocalPulse affronta:

| Problema | Dato |
|----------|------|
| 🗑️ **Spreco alimentare** | Il **15%** dei prodotti freschi nei mercati rionali non viene venduto e finisce al macero |
| 📱 **Cambiamento generazionale** | Il **70%** degli under-40 preferisce l'acquisto via app per comodità e velocità |
| 🏘️ **Crisi della prossimità** | Necessità urgente di rilanciare le micro-economie di quartiere in modo sostenibile |

---

## Innovazione tecnologica

LocalPulse si distingue per tre pilastri tecnologici integrati:

### 🧠 AI Dynamic Pricing
Un algoritmo cloud regola i prezzi in tempo reale in base all'orario di chiusura del mercato, incentivando l'acquisto dei prodotti prima che vadano sprecati. Il prezzo scende progressivamente nelle ultime ore, trasformando l'invenduto in opportunità.

### ☁️ Vendor Cloud Portal
I venditori caricano l'inventario tramite **messaggi vocali o foto**, senza dover digitare nulla. Il sistema interpreta e aggiorna automaticamente la disponibilità sul portale. Pensato per chi non ha familiarità con la tecnologia.

### 📍 Geo-Push Marketing
Notifiche push basate su **geofencing**: i clienti nelle vicinanze del mercato ricevono avvisi di offerte lampo "last minute" negli ultimi minuti prima della chiusura. Massima efficacia, zero spreco.

---

## Posizionamento competitivo

Integrazione con la filiera corta e gestione tempo reale dell'invenduto (scala 0–100):

| Piattaforma | Score | Caratteristica |
|-------------|-------|----------------|
| **LocalPulse** (noi) | **95%** | Piena digitalizzazione banchi — filiera corta integrata |
| Too Good To Go | 60% | Solo "Magic Box" generiche senza profilo produttore |
| Glovo / Deliveroo | 45% | Solo logistica di consegna, nessun legame col territorio |
| Esselunga a Casa | 25% | Modello GDO centralizzato, contrario alla prossimità |

> LocalPulse è l'unico sistema che non vende solo "avanzi", ma l'**intera qualità del mercato fresco**.

---

## Business plan

### Investimento iniziale (Seed)

| Voce | Importo |
|------|---------|
| Sviluppo MVP (AI + Cloud) | € 25.000 |
| Kit Digitalizzazione Banchi | € 10.000 |
| Marketing locale & Onboarding | € 10.000 |
| **Totale Seed Investment** | **€ 45.000** |

### Flussi di ricavo

- **Commissione** — 8% su ogni vendita gestita tramite app
- **Modello Premium** — abbonamento mensile per i venditori che vogliono dati di vendita avanzati e insight predittivi
- **Partnership istituzionali** — accordi con i Comuni per la riduzione dei costi di smaltimento rifiuti alimentari

### Obiettivo

> **Break-even point entro 15 mesi** dal lancio operativo.

---

## Funzionalità della webapp

### Per gli acquirenti
- 🔍 **Esplora mercati** — ricerca per prodotto, quartiere, categoria con filtri interattivi
- 🎠 **Carousel parallasse** — vetrina visiva dei mercati più vicini con foto reali
- 🔔 **Notifiche anti-spreco** — avvisi geo-push per offerte last-minute
- 📦 **Pre-ordini** — prenota la cassetta settimanale e scegli il giorno di ritiro
- 🌱 **Tracker impatto** — monitora kg salvati dallo spreco e CO₂ evitata personalmente
- ❤️ **Preferiti** — salva banchi e mercati di fiducia

### Per i venditori
- 🧑‍🌾 **Profilo banco** — storia, metodi, certificazioni visibili alla community
- 📊 **Dashboard vendite** — analisi su ordini, prodotti più venduti, fasce orarie
- 📦 **Gestione scorte** — aggiornamento disponibilità via voce o foto (Vendor Cloud Portal)
- 📣 **Promozioni lampo** — crea offerte anti-spreco last-minute con un tap
- 📅 **Calendario presenze** — comunica orari e assenze al mercato

---

## Tecnologie

Questa versione è un **prototipo frontend a singolo file HTML**, senza dipendenze da installare.

```
HTML5 + CSS3 + JavaScript Vanilla ES6
```

| Tecnologia | Utilizzo |
|------------|----------|
| `backdrop-filter` CSS | Effetto Liquid Glass su card, navbar e drawer mobile |
| CSS Custom Properties | Sistema di design token con variabili globali |
| CSS Animations + `@keyframes` | Blob animati, fade-up, pulse del logo, barre progress |
| JavaScript ES6 (Vanilla) | Router SPA, carousel parallasse, toast, hamburger menu |
| Google Fonts API | Cormorant Garamond (display) + DM Sans (corpo) |
| Unsplash (CDN) | Immagini reali dei mercati nel carousel |

**Nessun framework. Nessun bundle. Nessuna dipendenza npm.** Apri il file e funziona.

---

## Struttura del progetto

```
local-pulse/
│
├── index.html                  # ← Webapp completa, single-file
│
├── README.md                   # Questo file
```

> **Nota:** Il file `local-pulse.html` è autosufficiente. La cartella `assets/` contiene la versione scomposta in componenti separati, utile per evolvere il progetto verso un framework o un build system.

### Architettura SPA

Ogni "pagina" è un `<div id="p-{nome}">` con classe `.page`. Il router JavaScript gestisce la navigazione attivando/disattivando le sezioni senza ricaricare la pagina.

```javascript
function go(id) {
  document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
  document.getElementById('p-' + id).classList.add('active');
  window.scrollTo({ top: 0, behavior: 'instant' });
}
```

---

## Come iniziare

### Prerequisiti

Nessuno. Basta un browser moderno (Chrome 76+, Firefox 70+, Safari 14+, Edge 79+).

### Avvio immediato

```bash
# Clona il repository
git clone https://github.com/angelicagoffredo/local-pulse.git
cd local-pulse

# macOS
open local-pulse.html

# Linux
xdg-open local-pulse.html

# Windows
start local-pulse.html
```

Oppure **trascina `local-pulse.html` direttamente nel browser**.

### Sviluppo con live reload

```bash
# Node.js
npx serve .

# Python
python -m http.server 8080
```

---

## Pagine della webapp

| Pagina | ID SPA | Contenuto principale |
|--------|--------|----------------------|
| 🏠 **Home** | `p-home` | Hero, statistiche chiave, 3 pilastri tech, grafico competitivo, business plan seed, CTA venditori |
| 🗺️ **Esplora** | `p-esplora` | Carousel parallasse 5 mercati, ricerca, filtri categoria, 6 schede mercato |
| 🔐 **Login** | `p-login` | Accesso email + Google OAuth |
| 📝 **Registrazione** | `p-register` | Selezione ruolo acquirente/venditore, form completo |
| 👤 **Account** | `p-account` | Profilo, ordini recenti, tracker impatto ambientale con progress bar |
| 📬 **Contatti** | `p-contatti` | Info team, form di contatto, sezione FAQ |

---

## Design system

### Filosofia: Liquid Glass

Il design si ispira all'estetica **Liquid Glass** — superfici traslucide con profondità e riflessi, che restituiscono leggerezza senza perdere struttura. Ogni elemento sembra poggiare su vetro smerigliato davanti ai blob di colore animati in background.

```css
/* Formula base dell'effetto glass */
.glass {
  background: rgba(255, 255, 255, 0.20);
  backdrop-filter: blur(18px) saturate(180%);
  -webkit-backdrop-filter: blur(18px) saturate(180%);
  border: 1px solid rgba(255, 255, 255, 0.48);
  box-shadow: 0 8px 32px rgba(31, 38, 135, 0.08),
              inset 0 1px 0 rgba(255, 255, 255, 0.60);
}
```

### Palette colori

| Variabile | Hex | Utilizzo |
|-----------|-----|----------|
| `--g` | `#2d6a4f` | Verde primario — CTA, accenti, brand |
| `--g-dk` | `#1f4f38` | Verde scuro — hover stati |
| `--w` | `#e07b39` | Arancio caldo — secondario, highlights, tag warm |
| `--bg` | `#f2ede4` | Avorio — sfondo generale |
| `--txt` | `#1a1a18` | Quasi-nero — testo principale |
| `--txt2` | `#4a4a42` | Grigio caldo — testo secondario |
| `--muted` | `#888876` | Grigio-verde — placeholder, note, metadati |

### Tipografia

| Font | Pesi | Utilizzo |
|------|------|----------|
| `Cormorant Garamond` | 300, 400, 600 + italic | Titoli, hero, numeri statistiche, display |
| `DM Sans` | 300, 400, 500 | Corpo, UI, label, bottoni, navigazione |

### Componenti chiave

| Classe | Descrizione |
|--------|-------------|
| `.glass` | Surface traslucida base |
| `.gc` | Glass card con hover elevazione |
| `.btn-p` | Bottone primario verde |
| `.btn-gh` | Bottone ghost trasparente |
| `.btn-bl` | Bottone full-width per form |
| `.chip` | Filtro/tag selezionabile |
| `.feat-c` | Feature card con icona |
| `.mkt-c` | Scheda mercato con thumbnail |
| `.auth-c` | Contenitore form di autenticazione |
| `.comp-fill` | Barra animata grafico competitivo |

---

## Roadmap

### v1.0 — Prototipo UI (attuale ✅)
- [x] Single-file HTML con CSS iniettato
- [x] 6 pagine con router SPA vanilla
- [x] Design Liquid Glass completo e responsive
- [x] Carousel parallasse con 5 mercati reali
- [x] Hamburger menu per mobile
- [x] Grafico competitivo animato (AI Dynamic Pricing, TGTG, Glovo, Esselunga)
- [x] Business plan integrato con barre proporzionali
- [x] Tracker impatto ambientale con progress bar

### v1.1 — Backend
- [ ] API REST (Node.js / FastAPI)
- [ ] Database mercati e prodotti (PostgreSQL)
- [ ] Autenticazione JWT + OAuth Google
- [ ] Upload inventario via voce/foto (Vendor Cloud Portal)

### v1.2 — Features core
- [ ] Geolocalizzazione e mappa interattiva (Leaflet.js)
- [ ] Sistema notifiche push geofencing (anti-spreco)
- [ ] Pre-ordini, carrello, pagamenti (Stripe)
- [ ] Dashboard venditori con grafici reali

### v2.0 — App mobile
- [ ] Progressive Web App (PWA) con service worker
- [ ] Notifiche push native
- [ ] Modalità offline per la consultazione dei mercati
- [ ] App nativa iOS/Android (React Native o Flutter)

### v2.1 — AI & Sostenibilità
- [ ] AI Dynamic Pricing in produzione
- [ ] Calcolo automatico impronta carbonica per ordine
- [ ] Certificazioni biologico/km zero verificate on-chain
- [ ] Report impatto mensile aggregato per Comune
- [ ] Partnership istituzionali con programmi anti-spreco comunali

---

## Impatto atteso

### 🌍 Ambientale
- Riduzione stimata del **15→ <5%** di prodotti freschi sprecati nei mercati aderenti
- Diminuzione emissioni legate alla logistica grazie al modello km zero
- Tracker personale che rende tangibile l'impatto delle scelte d'acquisto

### 💼 Economico
- Aumento del fatturato dei venditori grazie alla visibilità digitale e ai pre-ordini
- Riduzione delle perdite da invenduto tramite AI Dynamic Pricing e offerte last-minute
- Commissione dell'**8% sulle vendite** come modello sostenibile per la piattaforma
- Risparmio sui costi di smaltimento rifiuti per i Comuni (potenziale partnership)

### 🤝 Sociale
- Rilancio del tessuto commerciale e culturale di quartiere
- Accesso facilitato a prodotti freschi di qualità, anche per famiglie a budget ridotto
- Riduzione del gap tecnologico per i venditori tradizionali over-50
- Creazione di comunità locali intorno al consumo consapevole e alla filiera corta

---

## Autrice

**Angelica Goffredo**

Progetto sviluppato sul tema: *LocalPulse — Digitalizzare la tradizione per abbattere lo spreco alimentare.*

Obiettivo: dimostrare come la tecnologia possa essere uno strumento concreto per valorizzare la tradizione locale, ridurre l'impatto ambientale e creare un nuovo modello di business sostenibile per i mercati rionali italiani.

---

<div align="center">

**LocalPulse** — *Digitalizzare la tradizione per abbattere lo spreco alimentare* 🌿  
*Progetto di Angelica Goffredo*

</div>