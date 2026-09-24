# Clean Code & Professional Engineering Standards

## 1. Architettura & Pulizia del Codice
- **Modularità e Separazione delle Responsabilità**: Separa rigorosamente la logica di business, le chiamate API/database e la presentazione visiva.
- **Tipizzazione Rigorosa**: In linguaggi tipizzati (TypeScript, Python con Type Hints, Rust, Go), dichiara sempre interfacce e tipi precisi per prop, stati e risposte API. Mai ricorrere a `any` o dizionari generici non tipizzati.
- **Dry & Manutenibilità**: Evita duplicazioni di logica estraendo funzioni pure e helper riutilizzabili.

## 2. Robustezza & Gestione Errori
- **Validazione degli Input**: Valida sempre i dati in ingresso provenienti da form o endpoint (usando librerie come Zod o Pydantic).
- **Gestione Errori Esplicita**: Evita blocchi `try/catch` generici o silenti. Ogni errore deve restituire un messaggio chiaro per l'utente o un log dettagliato per il debug.
- **Stati Asincroni**: Gestisci sempre tutti i 3 stati delle operazioni asincrone: caricamento (loading/skeleton), successo (dati renderizzati) ed errore (fallback visivo).

## 3. Sicurezza
- Non inserire mai stringhe di connessione, token o chiavi API nel codice. Richiedi l'uso di variabili d'ambiente (`.env`).
- Sanitizza sempre gli input per prevenire attacchi XSS, injection SQL o accessi non autorizzati.

## 4. Modalità di Consegna del Codice
- Consegna codice completo e pronto per l'esecuzione. Non omettere sezioni con commenti del tipo `// qui inserisci la logica`.
- Includi sempre le istruzioni minime per l'installazione delle dipendenze e l'avvio del file/modulo.
