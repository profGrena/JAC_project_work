1. Documento di Visione e Ambito (Project Charter / Vision Document)
Questo documento definisce l'identità del progetto e allinea tutti gli stakeholder sulla direzione da prendere.
Anagrafica del Progetto:
Nome del progetto (e codice identificativo se presente).
Keywords (parole chiave che descrivono il core business/tecnologia).
Breve descrizione (l'ormai famoso "elevator pitch").
Identità Strategica:
Mission: Cosa fa l'applicazione oggi e quale problema immediato risolve.
Vision: Dove si vuole arrivare nel lungo periodo; l'impatto desiderato sul mercato.
Analisi di Mercato e Contesto:
Target (User Personas): Profilazione degli utenti finali (età, bisogni, competenze tecnologiche).
Competitors: Analisi dei concorrenti diretti e indiretti (punti di forza e di debolezza).
Mappa degli Stakeholder:
Matrice degli stakeholder (committenti, utenti, team di sviluppo, project manager) con relativi ruoli e responsabilità (es. Matrice RACI).
2. Documento dei Requisiti (Specifiche Tecniche e Funzionali - SRS)
Il cuore operativo del progetto. Definisce nel dettaglio cosa l'applicazione deve fare.
Requisiti Funzionali:
Elenco dettagliato delle funzionalità (es. "L'utente deve poter resettare la password").
Requisiti Non Funzionali:
Prestazioni: Tempi di caricamento massimi, gestione del carico di utenti in contemporanea.
Sicurezza: Standard di crittografia, conformità GDPR, gestione delle sessioni.
Usabilità e Accessibilità: Linee guida (es. WCAG) e compatibilità con i vari browser (Responsive Design).
Modellazione dei Casi d'Uso (Use Case Diagram & Details):
Diagramma dei Casi d'Uso (UML): Rappresentazione visiva degli Attori (utenti/sistemi esterni) e delle loro interazioni con il sistema.
Schede di Dettaglio dei Casi d'Uso: Per ogni caso d'uso critico, compilare una scheda contenente:
ID e Nome del Caso d'Uso
Attori coinvolti
Pre-condizioni (cosa deve essere vero prima che l'azione inizi)
Flusso Principale (Scenario nominale): I passaggi passo-passo della corretta esecuzione.
Flussi Alternativi / Eccezioni: Cosa succede se qualcosa va storto (es. errore di login).
Post-condizioni (lo stato del sistema al termine).
3. Documento di Architettura e Design (SAD - Software Architecture Document)
Definisce come l'applicazione verrà costruita a livello tecnico.
Architettura di Sistema:
Scelta del pattern architetturale (es. MVC, Microservizi, Serverless).
Tecnologie utilizzate (Frontend, Backend, Database, Cloud Provider).
Modellazione dei Dati:
Diagramma ER (Entità-Relazione) o schema del database (NoSQL/Relazionale).
Dizionario dei dati.
Specifiche delle API:
Documentazione degli endpoint (es. tramite standard OpenAPI/Swagger) con formati di Request e Response (JSON).
4. Strategia di Versioning e Gestione del Codice
Le regole del gioco per il team di sviluppo per evitare caos nel codice.
Repository branching strategy: Scelta del modello di ramificazione (es. GitFlow, GitHub Flow, Trunk-based development).
Definizione dei branch principali (main, develop, feature/*, hotfix/*).
Policy di Versioning: Adozione del Semantic Versioning (SemVer: MAJOR.MINOR.PATCH).
Linee guida per le Pull Request (PR): Regole per la code review prima del merge.
5. Piano di Progetto e Tempistiche (Project Management & Scheduling)
Questa sezione definisce la roadmap temporale, l'allocazione delle risorse e la sequenza logica delle attività di sviluppo.
WBS (Work Breakdown Structure): * Scomposizione del progetto in blocchi di lavoro macro (es. Design, Sviluppo Backend, Sviluppo Frontend, Testing, Deployment) e micro-attività.
Diagramma di Gantt:
Asse Temporale: Calendario dettagliato del progetto (giorni/settimane/mesi).
Barre di Attività: Durata stimata per ogni singola attività della WBS.
Dipendenze: Collegamenti logici tra i task (es. "Lo sviluppo frontend della pagina di login non può iniziare finché non sono pronte le API di autenticazione").
Milestone (Pietre miliari): Punti di controllo chiave del progetto (es. Approvazione dei mockup UI/UX, Rilascio versione Alpha, Go-Live).
Allocazione delle Risorse:
Indicazione di quale membro del team (o team) è assegnato a ciascuna barra del Gantt per evitare sovraccarichi.
Evita i colli di bottiglia: Ti mostra subito se i designer, i programmatori backend e frontend stanno lavorando in sinergia o se qualcuno è bloccato in attesa del lavoro altrui.
Gestione del Critical Path (Percorso Critico): Ti permette di identificare quelle attività che, se subiscono un ritardo anche minimo, fanno slittare la data di consegna finale dell'intera applicazione web.
 
6. Piano di Testing e Qualità (QA Document)
Come si garantisce che l'applicazione funzioni correttamente prima del rilascio.
Strategia di Test: Definizione dei livelli di test (Unit Test, Integration Test, End-to-End Test, Penetration Test).
Criteri di Accettazione: Standard minimi che il software deve superare per essere considerato pronto per la produzione.
7. Manualistica (User & Dev Docs)
La documentazione per chi userà il software e per chi dovrà mantenerlo nel tempo.
Manuale Utente (User Guide):
Guida al primo accesso (Onboarding).
Tutorial passo-passo per le funzionalità principali con screenshot e FAQ.
Manuale dello Sviluppatore (Developer Guide):
Guida al setup dell'ambiente: Istruzioni per clonare la repository, installare le dipendenze e avviare l'app in locale (es. comandi Docker, script npm).
Linee guida di stile (Style Guide): Regole di formatting del codice (es. Linter utilizzati).
Procedure di Deployment: Come rilasciare l'applicazione in staging e in produzione (pipeline CI/CD).
8. Documentazione di Chiusura e Manutenzione
Piano di Manutenzione e SLA: Gestione dei bug post-rilascio e tempi di risposta garantiti.
Log dei Cambiamenti (Changelog): Registro pubblico o interno delle modifiche apportate in ogni versione rilasciata.