---
{"dg-publish":true,"dg-path":"Guida_Higgsfield_Modulo2.md","permalink":"/guida-higgsfield-modulo2/"}
---


# Guida completa al workflow cinematografico AI con Higgsfield

## Dal personaggio al film: Soul Cast, Soul Cinema e Cinema Studio 2.5

*(Proseguimento della Guida a Cinema Studio 2.0)*

---

## Panoramica del workflow completo

Nella prima parte di questa guida abbiamo esplorato Cinema Studio 2.0 per creare un breve video in stile retro sci-fi anni '70, lavorando all'interno di un unico ambiente (Image Mode e Video Mode). In questa seconda parte estendiamo il workflow all'intero ecosistema Higgsfield, che si articola in tre strumenti integrati:

- **Soul Cast**: Creazione di personaggi AI personalizzati con controllo su ogni dettaglio fisico e caratteriale

- **Soul Cinema**: Generazione di ambientazioni cinematografiche (location)

- **Cinema Studio 2.0 / 2.5**: Composizione (personaggio + ambientazione), animazione video e montaggio multi-shot

La logica di produzione segue il paradigma **"Cast → Shoot → Direct"**: si costruisce il cast, si fotografano le scene, si dirige il video. L'obiettivo di questa guida è mostrare come creare un cortometraggio AI.

---

## Fase 1 – Soul Cast: creazione del personaggio AI

### 1. Accesso e organizzazione del progetto

Vai su https://higgsfield.ai/ e dalla barra laterale seleziona **Soul Cast**. L'interfaccia consente di navigare tra diverse tipologie di asset: Image, Video, Audio e Cast.

Prima operazione consigliata: crea un **nuovo progetto** con un nome riconoscibile (es. il titolo del tuo film). Questo mantiene ordinato l'intero workflow fin dall'inizio.

### 2 Parametri di costruzione del personaggio

La creazione avviene attraverso una serie di pannelli progressivi. Ogni scelta influenza l'estetica e la coerenza narrativa del personaggio.

**Genre (Genere cinematografico)**
Seleziona il genere in cui si colloca il progetto: Fantasy, Sci-Fi, Romance, Detective, ecc. Questa scelta non vincola la trama, ma orienta l'estetica del personaggio. Esempio: scegliere "Detective" non significa, ad esempio, fare un film poliziesco, ma ottenere un aspetto sospeso e lugubre.

**Budget in millions**
Simula l'aspetto produttivo: un budget alto genera un look premium e rifinito, un budget basso orienta verso un'estetica da cinema indipendente.

**Era (Epoca)**
Definisce l'ambientazione temporale e influenza costumi, acconciature e aspetto generale.

**Archetype (Archetipo)**
Tipologia caratteriale del personaggio. Opzioni disponibili: Innocent, Everyman, Hero, Caregiver, Explorer, Rebel, Lover, Creator.

**Identity (Identità)**
Genere del personaggio: maschile o femminile.

**Physical Appearance (Aspetto fisico)**
Pannello dettagliato che comprende: tipo di pelle (caucasica, asiatica, ecc.), età, corporatura, altezza, colore degli occhi, tipo di capelli (texture, colore, lunghezza), barba.

**Details (Dettagli)**
Elementi personalizzati aggiuntivi: Confirm (cicatrici di conferma), Facial scar, Freckles, Tattoos, Eye patch. La voce "Custom" consente di inserire preferenze personalizzate.

**Outfit**
L'abbigliamento del personaggio (Casual, Formal, ecc.).

### 3 Generazione e scheda personaggio

Completata la configurazione, premi **"Generate"**. Il sistema produce il personaggio con una **Character Sheet** che mostra diverse angolazioni e i parametri riassuntivi.

Esempio di Character Parameters risultanti:

- Age: 55
- Race: White
- Genre: Detective
- Gender: Male
- Outfit: Casual
- Archetype: Everyman

### 4 Opzioni post-generazione

Dopo la generazione, hai a disposizione:

- **Save as Element**: Salva il personaggio come "element" richiamabile in Cinema Studio con il simbolo @. Operazione caldamente raccomandata e indispensabile per il workflow.

- **Get Exclusive Rights** (pulsante giallo): Acquista i diritti esclusivi per uso commerciale del personaggio generato.

- **Download**: Scarica la Character Sheet per uso esterno (es. generare varianti in altri strumenti).

- **Edit**: Modifica i parametri del personaggio dopo la generazione.

- **Use in Image**: Utilizza il personaggio nella generazione di immagini (selezionando Element, Single Image o Character Sheet).

- **Use in Cinema**: Porta il personaggio direttamente in Cinema Studio.

### 5 Best practice: creare più personaggi

Per un progetto completo, crea più personaggi con nomi propri (es. "Daniel Kerns", "Elena Voss"). Ogni nome verrà utilizzato per richiamare il personaggio in Cinema Studio tramite la chiocciola (@). 

### 6 Distinzione fondamentale: Element vs Soul Character

Esistono due formati di salvataggio del personaggio con funzioni diverse:

| Formato | Dove si usa | Come si crea |
|---|---|---|
| **Element** | Cinema Studio (immagine e video) | Pulsante "Save as Element" dalla Character Sheet |
| **Soul Character** | Soul Cinema | Upload di ~20 immagini del personaggio da diverse angolazioni |

Per creare un Soul Character (necessario se vuoi il personaggio già dentro Soul Cinema), scarica la Character Sheet e inseriscila in uno strumento esterno come **Nano Banana**. Usa un prompt del tipo: *"create detailed character sheet, only one angle for each image, no character sheet mode"*. Nano banana genererà le diverse angolature che poi caricherai come Soul Character in Higgsfield.

---

## Fase 2 – Soul Cinema: generazione delle ambientazioni

### 1 La logica della separazione scena-personaggio

Principio chiave del workflow: in questa fase si generano **solo le ambientazioni** (location), senza il personaggio. Il soggetto verrà inserito successivamente in Cinema Studio. Questa separazione garantisce maggiore controllo su entrambi gli elementi.

### 2 Interfaccia di Soul Cinema

L'interfaccia è essenziale: un campo di testo per la descrizione dell'immagine desiderata e, opzionalmente, lo slot per associare un Soul Character. Per le sole ambientazioni, lascia vuoto lo slot del personaggio.

### 3 Prompt per le ambientazioni

I prompt devono descrivere l'ambiente con precisione, evocando il mood desiderato. Un suggerimento pratico: usa **ChatGPT/Claude/Gemini** per generare i prompt, fornendo il contesto del film e specificando che stai scrivendo per Soul Cinema.

Esempio di approccio:

- Descrivi a ChatGPT la scena che vuoi (es. "piccola cucina disordinata con un certo mood malinconico")
- Chiedigli di scriverti un prompt ottimizzato per Soul Cinema
- Copia e incolla il risultato nell'interfaccia

Soul Cinema restituirà immagini con forte componente cinematografica: grana, contrasto e composizione di livello professionale.

### 4 Iterazione e selezione delle ambientazioni

Anche con soli 4 risultati per generazione, la qualità è molto alta. Genera ambientazioni per ogni scena del tuo film:

- **Stanza da letto** (scena risveglio/meditazione)
- **Cucina** (scena della solitudine)
- **Salotto** (scena finale davanti alla TV)

Seleziona per ogni ambientazione l'immagine che meglio si adatta alla tua visione registica.

### 5 Color Transfer: coerenza cromatica tra le scene

All'interno di Soul Cinema è disponibile il pannello **Color Transfer**. Questa funzione campiona la palette cromatica da un'immagine precedentemente generata e la applica a una nuova generazione.

Utilizzo pratico: genera la prima ambientazione che definisce il mood cromatico del film, poi usa Color Transfer su tutte le successive per mantenere coerenza visiva nell'intero progetto.

---

## Fase 3 – Cinema Studio 2.0 Image: composizione personaggio + ambientazione

### 1 Obiettivo

Collocare il personaggio (creato in Soul Cast) all'interno delle ambientazioni (create in Soul Cinema), ottenendo frame cinematografici completi che serviranno come base per la fase video.

### 2 Richiamare il personaggio con @

In Cinema Studio, digita il simbolo **@** nel campo di input e apparirà la lista degli Element salvati. Seleziona il tuo personaggio (es. "@Daniel Kerns").

Nota: questo è possibile solo se hai precedentemente salvato il personaggio come Element (vedi sezione precedente).

### 3 Assegnare il mood emotivo

Accanto all'Element del personaggio c'è un pulsante dedicato al **mood emozionale**. Opzioni disponibili:

- Angry
- Joyful
- Trust
- Fear
- Surprise
- Sadness

La scelta del mood influenza espressione facciale e postura del personaggio. Per coerenza narrativa, mantieni lo stesso mood su tutte le scene (es. "Sadness" per un film introspettivo e malinconico).

### 4 Prompt d'azione

I prompt devono essere semplici e descrivere l'azione del personaggio nella scena. Il sistema sa già dove collocarlo (grazie all'ambientazione) e chi è (grazie all'Element): basta descrivere cosa fa.

Prompt esempio:

```
@Daniel Kerns is sitting on the couch watching the television
that is in the foreground, sadness atmosphere
```

Best practice: se il sistema non interpreta correttamente un elemento della scena (es. confonde la TV con un altro oggetto), specifica la posizione spaziale dell'elemento nel prompt (es. "the television that is in the foreground").

### 5 Parametri cinematografici

Come già visto nella prima parte della guida precedente, Cinema Studio offre parametri tecnici professionali:

- **Tipologia di camera**: Ogni modello ha le sue caratteristiche estetiche.

- **Lenti**: Anamorfiche o standard.

- **Lunghezza focale**: Per un film introspettivo e quotidiano, il **50mm** è ideale: equivale alla visione naturale dell'occhio umano.

**- Apertura**: f/1.4 per forte effetto bokeh, f/4 per mantenere più elementi a fuoco.

### 6 Output in 4K e iterazione

Imposta **sempre** l'output in **4K**, soprattutto quando le immagini saranno usate nella fase video. Un output a risoluzione inferiore produrrà risultati inconsistenti nel passaggio a video.

Ogni generazione costa solo **16 crediti**, ma quando si combinano personaggio e ambientazione le variabili aumentano: preparati a iterare più volte rispetto alla fase delle sole ambientazioni.

---

## Fase 4 – Cinema Studio 2.5: l'ecosistema integrato

### 1 La novità

Cinema Studio 2.5 è un aggiornamento che integra tutte le fasi precedenti in un unico ambiente. Non è più necessario spostarsi tra Soul Cast, Soul Cinema e Cinema Studio: tutto avviene dentro la stessa interfaccia.

Per accedere: all'interno di Cinema Studio Image, troverai la possibilità di switchare tra **Cinema 2.0** e **Cinema Studio 2.5**.

### 2 Scenation

La funzione chiave di Cinema Studio 2.5 si chiama **Scenation**. Al suo interno troverai:

- **Build Your Cast**: Crea il personaggio direttamente in Cinema Studio 2.5, con le stesse opzioni viste in Soul Cast. Le voci disponibili sono identiche.

- **Locations**: Genera ambientazioni direttamente, utilizzando il modello **Soul Location**. Scrivi la descrizione dell'ambiente desiderato e il sistema genera le immagini di riferimento.

### 3 Salvare una location come element

Una volta generata un'ambientazione soddisfacente, seleziona **"Save as Location"**. Questo la trasforma in un Element richiamabile con @ all'interno della composizione, esattamente come il personaggio.

### 4 Composizione integrata

Nella composizione di Cinema Studio 2.5, digitando @ avrai a disposizione sia la **Location** salvata sia il **personaggio**. Il vantaggio è evidente: velocità, logicità e nessun passaggio tra strumenti diversi.

### 5 Confronto operativo: workflow tradizionale vs Cinema Studio 2.5

| Passaggio | Workflow tradizionale | Cinema Studio 2.5 |
|---|---|---|
| Creazione personaggio | Soul Cast → Save as Element | Build Your Cast (interno) |
| Creazione ambientazione | Soul Cinema → Download | Locations + Soul Location (interno) |
| Composizione | Cinema Studio Image + @ | @ con Location + Character (interno) |
| Passaggio al video | Cinema Studio Video | Cinema Studio Video (stesso ambiente) |

---

## Fase 5 – Cinema Studio Video: animazione e montaggio Multi-Shot

### 21.1 Dal frame statico alla clip animata

Prendi le immagini finali (personaggio + ambientazione) prodotte nelle fasi precedenti e portale nella sezione **Video** di Cinema Studio. Come già visto nella prima parte, la modalità consigliata è il **Multishot Manuale**.

### 21.2 Setup del Multishot Manuale per il film completo

Come nella prima guida, in Multishot Manuale puoi creare fino a 6 scene consecutive. Per ogni scena imposti:

- Start frame
- Prompt
- Movimento camera
- Durata
- Emozione
- Element del personaggio (@)

### 3 Configurazione per scena

Per ogni scena del multi-shot:

- **Prompt d'azione**: Ogni scena ha il suo prompt specifico. Mantieni i prompt semplici e focalizzati sull'azione, come per le immagini.

- **Personaggio (Element)**: Inserisci il tuo personaggio con @ in ogni scena. Mantieni lo stesso mood emozionale per coerenza narrativa.

- **Durata**: Definisci la durata di ogni inquadratura. Esempio dal workflow di riferimento: 3 secondi per la scena 1, 3 secondi per la scena 2, 6 secondi per la scena 3.

- **Audio**: Higgsfield include la generazione audio integrata, che produce risultati di buona qualità.

- **General (Preset)**: Identifica il mood, la tipologia e lo stile visivo del video.

- **Batch Size**: Numero di varianti generate per ogni scena. Si consiglia di generarne sempre tanti, perché le variabili nella fase video sono maggiori.

- **Movimenti di camera**: Per un film introspettivo e statico, imposta "Auto" per ottenere movimenti minimi. Per film d'azione, specifica movimenti più dinamici.

- **Speed Ramp**: Controlla le variazioni di velocità nella clip. Per un ritmo uniforme e introspettivo, lascia "Auto" o "Lineare".

- **Start Frame**: Definisci l'immagine da cui parte la generazione video. Questo garantisce che il primo fotogramma corrisponda esattamente alla composizione voluta.

### 4 Costi e crediti

96 crediti per 4 generazioni parallele. Higgsfield risulta economico rispetto ad altre piattaforme, ma la fase video richiede più iterazione. Genera sempre più varianti e seleziona i migliori risultati.

### 5 Gestione degli artefatti

Piccoli artefatti (deformazioni di elementi secondari, comportamenti innaturali di oggetti) possono comparire. Due strategie:

1. **Iterare** ulteriormente per ottenere generazioni pulite
2. **Tagliare** la clip qualche frame prima dell'artefatto in fase di montaggio

---

## Storyboard e pre-produzione AI

### 1 L'importanza dello storyboard

Prima di avviare qualsiasi generazione, prepara uno **storyboard** che definisca:

- Quante scene compongono il film
- Cosa accade in ciascuna scena
- Quale emozione domina ogni scena
- Quale tipo di inquadratura e movimento di camera utilizzi

Questo evita sprechi di crediti e garantisce coerenza narrativa. Nel workflow di riferimento, il film è stato pensato prima come sequenza narrativa:

1. Personaggio medita sul letto (mood triste, risveglio)
2. Si alza e va in cucina
3. Apre il frigo e lo trova vuoto (conferma la solitudine)
4. Si sposta in salotto e guarda la TV (chiusura malinconica)

### 2 Riferimenti visivi

Cerca riferimenti cinematografici reali prima di scrivere i prompt. Film, fotografie, mood board: tutto ciò che può guidare le tue scelte di luce, colore e composizione.

---

## Coerenza visiva e narrativa: checklist

Per mantenere coerenza lungo l'intero progetto:

- **Personaggio**: Usa sempre lo stesso Element (@nome) in tutte le scene; non cambiare i parametri dopo la creazione
- **Mood emotivo**: Mantieni lo stesso mood su tutte le scene se il film ha un tono uniforme (es. Sadness per un film malinconico), oppure progetta un arco emotivo coerente come nella prima guida
- **Palette cromatica**: Usa il Color Transfer di Soul Cinema per uniformare i colori tra tutte le ambientazioni
- **Output**: Tutte le immagini destinate al video devono essere in 4K
- **Prompt**: Richiama sempre gli elementi visivi chiave del tuo film in ogni prompt 

---

## Uso didattico per studenti (estensione)

In aggiunta agli ambiti didattici già indicati nella prima guida, questo workflow esteso consente di esplorare:

**Pre-produzione cinematografica AI**
Il concetto di casting, location scouting e storyboard tradotti in ambiente digitale. Gli studenti sperimentano le stesse decisioni di un regista (scelta degli archetipi, definizione del look, selezione delle ambientazioni) senza le barriere logistiche ed economiche di una produzione reale.

**Character Design e coerenza identitaria**
La costruzione di un personaggio attraverso parametri (età, archetipo, corporatura, outfit) insegna a pensare un personaggio in modo sistematico, come farebbe un character designer o uno sceneggiatore.

**Fotografia cinematografica applicata**
La scelta di lunghezze focali (50mm vs 35mm), aperture (f/1.4 vs f/4) e lenti (anamorfiche vs standard) in Cinema Studio traduce concetti teorici di fotografia in scelte operative immediate, con risultato visibile.

**Color Grading e coerenza cromatica**
Il Color Transfer di Soul Cinema introduce gli studenti al concetto di palette cromatica coerente e di color grading come strumento narrativo.

**Workflow iterativo e pensiero critico**
Il processo di generazione-selezione-iterazione sviluppa capacità di analisi critica dell'immagine: lo studente deve valutare composizione, coerenza e qualità ad ogni iterazione.

---

## Sintesi operativa (checklist completa del workflow)

1. **Soul Cast**: Definisci i parametri del personaggio (genere, budget, era, archetipo, identità, aspetto fisico, dettagli, outfit)
2. **Soul Cast**: Premi Generate e ottieni la Character Sheet
3. **Soul Cast**: Salva il personaggio come **Element** (fondamentale)
4. *(Opzionale)* Scarica la Character Sheet e genera 20 angolature in Nanobanana per creare un **Soul Character**
5. **Soul Cinema**: Genera le ambientazioni per ogni scena del film, usando prompt descrittivi (anche generati via ChatGPT)
6. **Soul Cinema**: Usa **Color Transfer** per uniformare la palette cromatica tra tutte le ambientazioni
7. **Cinema Studio Image** (2.0 o 2.5): Inserisci il personaggio (@nome) nelle ambientazioni con prompt d'azione semplici
8. **Cinema Studio Image**: Assegna il **mood emotivo** e i **parametri cinematografici** (camera, lente, focale, apertura)
9. **Cinema Studio Image**: Imposta output in **4K** e itera fino a ottenere il frame desiderato
10. **Cinema Studio Video**: Porta le immagini finali in Multishot Manuale
11. **Cinema Studio Video**: Per ogni scena: inserisci personaggio, scrivi prompt, imposta durata, camera, mood, start frame
12. **Cinema Studio Video**: Genera con batch size elevato, seleziona le migliori varianti
13. **Post-produzione**: Assembla le clip in un software di editing (DaVinci Resolve, Premiere, ecc.), aggiungi musica, effetti sonori e color grading finale


