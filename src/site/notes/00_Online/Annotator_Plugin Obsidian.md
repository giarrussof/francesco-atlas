---
{"dg-publish":true,"dg-path":"Annotator_Plugin Obsidian.md","permalink":"/annotator-plugin-obsidian/"}
---


## Guida dettagliata al plugin annotator
Il plugin Annotator è uno strumento potente per Obsidian che ti consente di leggere, evidenziare e annotare file in formato EPUB e PDF direttamente all'interno del tuo vault. La grande comodità è che tutte le tue evidenziazioni e annotazioni vengono salvate nel formato Markdown, garantendoti che tutti i contenuti siano in un unico posto, massimizzando la portabilità e la flessibilità.

### Fase 1: Installazione e preparazione dei file
Questa fase ti illustra i passaggi iniziali per rendere operativo Annotator nel tuo ambiente Obsidian.

#### 1.1 Installazione del plugin
Per iniziare a usare Annotator, devi prima installarlo dalla libreria dei plugin della community:

1. Apri le **Impostazioni** (l'icona dell'ingranaggio).
2. Vai su **Plugin di terze parti**.
3. Clicca su **Sfoglia**.
4. Cerca `Annotator`.
5. Clicca su **Installa** e subito dopo su **Abilita**.

#### 1.2 Preparazione e importazione dei documenti
Affinché Annotator possa funzionare, i file EPUB o PDF che desideri annotare devono essere copiati all'interno del tuo vault di Obsidian.

1. Crea una cartella dedicata per i tuoi libri (ad esempio, `ePub` o `PDF`) all'interno del tuo vault per mantenere tutto organizzato.
2. Copia i file EPUB o PDF in questa cartella.
3. **Suggerimento importante:** Ti consiglio di rinominare i file con nomi brevi e chiari per evitare problemi durante la copiatura del percorso e per comodità quando dovrai scrivere il codice di collegamento. PEr esempio, [[Nome anno\|Nome anno]]

> **Nota sulla visibilità dei file:** Se non vedi i file EPUB nell'Esplora Risorse di Obsidian, vai su **Impostazioni > File e collegamenti** e assicurati che l'opzione **Rileva tutte le estensioni di file** sia attiva. Questa impostazione permette a Obsidian di visualizzare anche formati che normalmente non supporta direttamente, come gli EPUB.

### Fase 2: Configurazione delle opzioni (settings)
Prima di configurare la singola nota di lettura, personalizziamo il comportamento generale di Annotator.

1. Vai in **Impostazioni** e clicca sul plugin **Annotator**.
2. **Percorso predefinito (Custom default Path):** Se tutti i tuoi libri sono nella stessa cartella (es. `ePub`), puoi impostare qui questo percorso predefinito. Questo ti farà risparmiare tempo, perché non dovrai specificare il percorso completo del file ogni volta.
3. **Visualizzazione:** Puoi scegliere come visualizzare il libro:
    - **Pagine:** Il libro appare diviso in pagine fisse.
    - **Scroll:** Il libro viene mostrato come una singola pagina scorrevole, simile a una pagina web.
4. **Impostazioni di salvataggio (Prefix/Postfix/Colore):** Queste opzioni definiscono come il testo evidenziato viene salvato nella nota Markdown.
    - Di default, Annotator può includere un testo prima (**Prefix**) e dopo (**Postfix**) l'evidenziazione, oltre a mostrare il colore.
    - Se desideri un codice Markdown più pulito, ti suggerisco di disattivare le opzioni Prefix e Postfix.
    - Se disattivi Prefix e Postfix, puoi anche disattivare l'opzione per mostrare il colore (il classico giallo), altrimenti ha più senso lasciarla attiva se usi Prefix/Postfix per distinguere chiaramente il testo evidenziato nel codice. Se non le usi, il codice apparirà più pulito e meno complesso.

### Fase 3: Creazione della nota di lettura
Per aprire il documento EPUB o PDF e iniziare a annotare, devi creare una nota Markdown che funga da "contenitore" per il file.

#### 3.1 Collegamento del file al plugin
Devi inserire una proprietà specifica all'interno della nota per indicare ad Annotator quale file aprire:
**Opzione 1: Utilizzo del Front Matter (Consigliato)**
Il metodo standard e più pulito è usare il Front Matter (le proprietà in YAML) all'inizio della nota:

1. Apri la tua nuova nota Markdown (ad esempio, `Lettura - Titolo Libro`).
2. In cima alla nota, inserisci i tre trattini:
    
    ```
    ---
    annotation-target: nome_del_file.epub
    ---
    ```
    
1. Sostituisci `nome_del_file.epub` con il nome esatto del tuo documento, inclusa l'estensione (`.epub` o `.pdf`). Se non hai impostato un percorso predefinito, devi includere il percorso della cartella (es. `ePub/nome_del_file.pdf`).

> **Formato del file:** Se in rari casi Annotator non riesce a identificare il tipo di file, puoi forzarlo aggiungendo una seconda proprietà: `annotation-target-type: pdf` (o `epub`).

#### 3.2 Avvio della lettura
Dopo aver inserito la proprietà di collegamento:

1. Chiudi e riapri la nota, oppure, se necessario, utilizza il riquadro comandi (`Ctrl/Cmd + P`) e cerca il comando "Annotate".
2. In alternativa, fai clic sui tre puntini (`...`) nell'angolo in alto a destra della nota e seleziona **Annotate**.

Il tuo documento si aprirà direttamente all'interno della nota.

### Fase 4: Evidenziazioni e annotazioni
Una volta che il testo in EPUB/PDF è aperto, puoi iniziare il processo di lettura attiva:

1. **Evidenziare:** Seleziona il testo desiderato con il cursore del mouse. Ti appariranno due opzioni:
    - **Annota:** Ti permette di salvare l'evidenziazione e aggiungere immediatamente un tuo pensiero, un commento, o un riassunto con le tue parole. Puoi usare la formattazione Markdown e aggiungere tag all'interno dell'annotazione.
    - **Evidenzia:** Salva la selezione direttamente, rimandando l'aggiunta di commenti a un secondo momento.
2. **Visualizzazione Side-bar:** Sulla destra, Annotator mostra un pannello dove sono elencate tutte le evidenziazioni e annotazioni relative al documento attivo. Queste possono essere ricercate e si aggiornano quando scorri la pagina.
3. **Note di Pagina (Page Notes):** Puoi usare questa funzione per scrivere note o commenti che si riferiscono a una pagina intera del libro.

### Fase 5: Gestione e riutilizzo delle annotazioni
Il grande vantaggio di Annotator risiede nel modo in cui salva i tuoi appunti, rendendoli subito riutilizzabili e cercabili.
#### 5.1 Il formato Markdown delle evidenziazioni
Le tue evidenziazioni sono scritte direttamente all'interno del file Markdown della nota di lettura.

1. Per visualizzare il codice sottostante, vai sui tre puntini (`...`) e clicca su **Open as Markdown**.
2. Vedrai che il codice generato è dettagliato, contenente ID univoci, date e link, necessari al plugin per identificare e richiamare il blocco di testo.

#### 5.2 Modalità Lettura e link rapidi
Passando alla **Modalità Lettura** (`Ctrl/Cmd + E`), Obsidian nasconde tutto il codice del plugin, mostrandoti solo il testo evidenziato.

- Il testo salvato include anche dei **link cliccabili** che, una volta selezionati, ti riportano direttamente alla porzione di testo evidenziata all'interno del libro.

#### 5.3 Riutilizzo delle annotazioni
Puoi facilmente estrarre e incorporare le tue evidenziazioni in qualsiasi altra nota del vault, sfruttando la funzione di incorporamento (embed) di Obsidian:

1. **Incorporamento tramite ID di blocco:** Utilizza la sintassi di incorporamento di Obsidian, facendo riferimento al blocco specifico (che ha un ID univoco).
    - Sintassi: `![[Nome Nota Libro#^blocco_ID]]`.
2. **Trascinamento (Drag and Drop):** Mentre il testo è aperto, tieni premuto il tasto **Shift**, seleziona l'evidenziazione dalla nota Markdown e trascinala in un'altra nota. Verrà inserita come un link.
3. **Sincronizzazione dinamica:** Poiché stai incorporando o linkando un blocco di testo, qualsiasi modifica tu faccia all'annotazione nella nota originale si rifletterà automaticamente in tutte le note in cui l'hai incorporata.

---

## Utilità e funzioni del plugin Annotator

L'utilizzo di Annotator offre diversi benefici cruciali per il tuo Sistema di Gestione della Conoscenza (PKM) in Obsidian:

### 1. Centralizzazione del workflow di lettura

- **Lettura unificata:** Ti permette di evitare l'uso di software esterni specifici per EPUB o PDF, mantenendo l'intero processo di lettura e annotazione all'interno di Obsidian.
- **Gestione dei PDF:** Sebbene Obsidian abbia un lettore PDF nativo (che permette, ad esempio, di copiare il testo come citazione completa di link al blocco), Annotator estende questa funzionalità, offrendo un'interfaccia focalizzata specificamente sull'evidenziazione e l'annotazione.
- **Indipendenza dal formato:** Poiché le annotazioni sono in Markdown, esse non sono vincolate al file originale (PDF/EPUB) e possono essere utilizzate ovunque, garantendo la flessibilità del formato Markdown.

### 2. Ricerca e collegamento avanzato
- **Ricerca Facilitata:** Il testo delle evidenziazioni è integrato nella nota Markdown e viene quindi indicizzato. Questo significa che puoi cercare facilmente il contenuto evidenziato utilizzando la potente funzione di ricerca globale di Obsidian (che può filtrare per tag, per contenuto e persino usare espressioni regolari come `regex`).
- **Creazione della rete:** Sfruttando le capacità di _linking_ di Obsidian (parentesi quadre doppie) e la capacità di incorporare le evidenziazioni (embed) in altre note, puoi integrare i concetti dai tuoi libri con il resto del tuo grafo di conoscenza, collegando ad esempio le idee principali (MoC).

### 3. Alternative nel panorama dei plugin
Sebbene Annotator sia eccellente per EPUB e PDF, esistono altre opzioni per formati specifici:

- **PDF++:** Un'alternativa molto avanzata per i PDF, che consente evidenziazioni con diversi colori e la possibilità di copiare link e callout direttamente dall'area selezionata.
- **Kindle Highlights:** Se la tua lettura avviene su Kindle, questo plugin è l'ideale per importare automaticamente tutte le evidenziazioni in una nota Markdown di Obsidian.
- **EPUB Importer:** Questo plugin tenta di convertire ogni capitolo di un EPUB in una nota Markdown separata, sebbene a volte possa presentare problemi di formattazione o note vuote.