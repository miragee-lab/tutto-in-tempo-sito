# Revisione grafica del sito

Revisione dell’8 ottobre 2026. Ambito: grafica e fruibilità delle pagine esistenti.

## Direzione

Presentazione di un’app per l’organizzazione quotidiana, con il registro caldo ed editoriale già presente nel sito. Logo, nome, percorsi, categorie, testi funzionali e contenuto delle dodici sezioni della privacy sono conservati. Le modifiche riguardano caratteri, spazi, gerarchie, anteprima del prodotto e stati delle interazioni.

Taste: `DESIGN_VARIANCE: 6`, `MOTION_INTENSITY: 3`, `VISUAL_DENSITY: 4`. L’obiettivo è una pagina leggibile e calma, con una sola breve entrata del prodotto e feedback sui comandi, senza movimento continuo o scorrimento controllato da JavaScript.

## Sistema applicato

- Fondo chiaro `#fbf9f4`, testo verde scuro `#172c29`, accento `#a34529`; colori secondari derivati dai toni del marchio. Il tema scuro usa gli stessi ruoli semantici.
- Titoli Lora; testi e comandi DM Sans. Lora continua la voce editoriale dei titoli Georgia preesistenti, invece di introdurre una nuova identità tipografica. Tracking minimo `-0.035em`, interlinea dei titoli `1.14`.
- Corpo principale 16 px; contenuto delle categorie 14–15 px; note 12–14 px. La privacy usa corpo 16 px con misura massima di 72ch.
- Gruppi delle categorie senza riquadri individuali. La sezione delle funzioni distingue l’avviso principale dalle due funzioni di supporto.
- Controlli a pillola; riquadri e avvisi a 16 px; la cornice del telefono ha una curvatura separata che rappresenta il dispositivo.
- Feedback dei pulsanti 140–160 ms con `cubic-bezier(.23,1,.32,1)`. Hover di movimento limitato ai puntatori precisi. Nessuna animazione sugli spostamenti del focus o sull’indice privacy. Preferenza di movimento ridotto rispettata.
- Altezza minima dei collegamenti principali 44 px; indice della privacy collassabile sotto 768 px; i collegamenti originali alle sezioni restano invariati.

## Evidenza e scelte contestuali

Il contenuto della schermata del telefono proviene dalla beta reale, acquisita in un browser di prova separato. La didascalia e il testo alternativo dichiarano i dati di esempio. Non è una UI fittizia costruita per il sito, né una promessa di disponibilità sul Play Store.

Il controllo statico Impeccable segnala i titoli serif in corsivo e alcuni spazi prima dei divisori. Il corsivo è conservato intenzionalmente come parte della voce preesistente, non scelto come stile predefinito per un nuovo marchio. Gli spazi reali sono verificati nel browser: le righe dei passi hanno 28 px sotto il contenuto e le FAQ 21 px. I falsi positivi del controllo statico su `padding-block` non richiedono duplicare dichiarazioni CSS.

Le regole delle skill sono applicate nel contesto di un’evoluzione del sito esistente: nessuna migrazione di framework, nessuna nuova affermazione commerciale, nessun cambio del logo. La foto del prodotto è una schermata reale; non richiede una rappresentazione generata. Un nuovo stile completo richiederebbe un brief distinto.

## Controlli

Home e privacy controllate a 320, 390, 768, 1024 e 1440 px, più il tema scuro su telefono e desktop. Verificati collegamenti interni, FAQ via mouse e tastiera, indice mobile, caricamento dei caratteri, assenza di overflow, movimento ridotto e accesso al contenuto via tastiera. Il testo delle dodici sezioni della privacy è confrontato con la versione precedente.

I rapporti di contrasto di testo primario, secondario e accento superano 4,5:1 sui tre fondi previsti in entrambi i temi. I rapporti e le catture di prova sono conservati in `qa/`, esclusa da Git.

Lighthouse eseguito sul server locale con Chrome headless: home 96/100 prestazioni e 100/100 accessibilità, buone pratiche e SEO; privacy 100/100 accessibilità, buone pratiche e SEO. Sono misure di laboratorio, non dati di navigazione raccolti dagli utenti. Il controllo delle prestazioni è simulato su dispositivo mobile.
