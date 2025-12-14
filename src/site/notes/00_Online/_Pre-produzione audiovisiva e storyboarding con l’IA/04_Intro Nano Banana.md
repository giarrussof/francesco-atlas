---
{"dg-publish":true,"dg-path":"_Pre-produzione audiovisiva e storyboarding con l’IA/04_Intro Nano Banana.md","permalink":"/pre-produzione-audiovisiva-e-storyboarding-con-l-ia/04-intro-nano-banana/"}
---


# Usare Nano Banana (Gemini 2.5‑flash‑image) per Storyboard – Dispensa introduttiva

Queste dispense guidano passo‑passo nell'uso di **Nano Banana (Gemini 2.5‑flash‑image)** per la realizzazione di storyboard, integrando tecniche di prompting, trattamento, mood board e workflow narrativo. Il materiale è pensato per studenti universitari (livello intermedio) che vogliono usare l'AI come strumento di pre‑produzione visuale e di ricerca.

---

## 1. Obiettivi del modulo

Al termine del modulo, lo/la studente/ssa sarà in grado di:

- Comprendere cosa è **Nano Banana (Gemini 2.5‑flash‑image)** e come funziona in relazione allo storyboard.
- Usare **prompt strutturati** per generare storyboard coerenti (singolo frame e sequenza).
- Integrare **trattamento**, **mood board** e **storyboard** in un flusso di lavoro unico.
- Lavorare in modo **iterativo** con editing conversazionale (non solo rigenerazione casuale).
- Gestire la **consistenza dei personaggi** lungo più frame.

---

## 2. Risorse fondamentali

### 2.1. Guida ufficiale Google al prompting di Gemini 2.5 Flash Image

- **Titolo:** How to prompt Gemini 2.5 Flash Image Generation for the best results  
- **Link:** [https://developers.googleblog.com/en/how-to-prompt-gemini-2-5-flash-image-generation-for-the-best-results/](https://developers.googleblog.com/en/how-to-prompt-gemini-2-5-flash-image-generation-for-the-best-results/)

Perché è centrale:

- Spiega i principi guida del prompting (descrivere scene, non solo parole chiave).
- Offre esempi di prompt per **pannelli singoli** in stile fumetto / storyboard.
- Insiste su descrizione di:
  - foreground, background;
  - tipo di luce;
  - stile visivo;
  - composizione.

### 2.2. Documentazione API per l'image generation

- **Titolo:** Image generation with Gemini (aka Nano Banana & Nano Banana Pro)  
- **Link:** [https://ai.google.dev/gemini-api/docs/image-generation](https://ai.google.dev/gemini-api/docs/image-generation)

Perché leggerla anche se non programmi:

- Chiarisce come il modello "vede" input testuali e visivi.
- Mostra come passare **più immagini di riferimento** (fondamentale per consistenza personaggi/scene).
- Aiuta a pensare al prompting come costruzione di un "contenuto multimodale".

### 2.3. Video tutorial ufficiale Google Developers

- **Titolo:** Learn to Build with Gemini Nano‑Banana (Gemini 2.5 Flash Image)  
- **Link:** [https://www.youtube.com/watch?v=UTdfxFyOQTI](https://www.youtube.com/watch?v=UTdfxFyOQTI)

Perché guardarlo:

- Dimostrazione pratica ufficiale: accesso via AI Studio, image creation, editing conversazionale.
- Mostra uso di più immagini per mantenere coerenza.
- Best practices di prompting applicate.

### 2.4. Blog e guide avanzate

**Fotor – 40+ Nano Banana Pro Prompts**  
[https://www.fotor.com/blog/nano-banana-model-prompts/](https://www.fotor.com/blog/nano-banana-model-prompts/)

- Sezione "Detailed Storyboard" con prompt pronti.
- Consigli pratici su iterative refinement.

**Dev Community – Nano-Banana Pro: Prompting Guide & Strategies**  
[https://dev.to/googleai/nano-banana-pro-prompting-guide-strategies-1h9n](https://dev.to/googleai/nano-banana-pro-prompting-guide-strategies-1h9n)

- Character Consistency & "Identity Locking".
- One‑Shot Storyboarding & Concept Art.

**Replicate – How to prompt Nano Banana Pro**  
[https://replicate.com/blog/how-to-prompt-nano-banana-pro](https://replicate.com/blog/how-to-prompt-nano-banana-pro)

- Guida sintetica e pratica.

**Blog Google ufficiale – 7 tips to get the most out of Nano Banana Pro**  
[https://blog.google/products/gemini/prompting-tips-nano-banana-pro/](https://blog.google/products/gemini/prompting-tips-nano-banana-pro/)

### 2.5. Risorse specifiche su storyboard e character consistency

**Emerge – How to Storyboard Product Launches with Consistent AI Characters**  
[https://emerge.fibre2fashion.com/blogs/10815/how-to-storyboard-a-product-launch-with-consistent-characters-across-10-images-in-n](https://emerge.fibre2fashion.com/blogs/10815/how-to-storyboard-a-product-launch-with-consistent-characters-across-10-images-in-n)

- Workflow step‑by‑step per storyboard con personaggi consistenti.

**Apiyi – Nano Banana Pro Storyboard Generation Complete Guide**  
[https://help.apiyi.com/nano-banana-pro-storyboard-generation-guide-en.html](https://help.apiyi.com/nano-banana-pro-storyboard-generation-guide-en.html)

**Skywork – Anime Character Consistency: Nano Banana 2 Complete Guide**  
[https://skywork.ai/blog/nano-banana-2-anime-character-guide/](https://skywork.ai/blog/nano-banana-2-anime-character-guide/)

- Tecniche per mantenere identità visiva lungo più frame.

**Nanobananaz – How to Create Consistent Characters with Nano Banana**  
[https://nanobananaz.com/consistent-characters-with-nano-banana/](https://nanobananaz.com/consistent-characters-with-nano-banana/)

**YouTube – I Created a Full AI Storyboard Using Nano Banana x Kling AI**  
[https://www.youtube.com/watch?v=SgMZO1sq4j8](https://www.youtube.com/watch?v=SgMZO1sq4j8)

- Workflow completo end-to-end.

**YouTube – Google's FREE Gemini 2.0 is INSANE: Consistent Characters, Storyboards**  
[https://www.youtube.com/watch?v=iKUdeKYnt6Y](https://www.youtube.com/watch?v=iKUdeKYnt6Y)

**YouTube – Storyboarding Images from Script Using Gemini**  
[https://www.youtube.com/watch?v=wujAT1GJxX8](https://www.youtube.com/watch?v=wujAT1GJxX8)

---

## 3. Concetti base: modello, storyboard, prompting

### 3.1. Cos'è Nano Banana (Gemini 2.5‑flash‑image)

- Modello di generazione di immagini della famiglia **Gemini 2.5**.
- Pensato per: immagini ad alta qualità, **editing conversazionale**, uso di più input visivi.
- Punti di forza per storyboard:
  - consistenza più robusta tra più immagini;
  - capacità di seguire istruzioni di tipo "regia" (camera, luce, composizione);
  - integrazione naturale in flussi di lavoro testuali (script, trattamenti, shot list).

### 3.2. Cos'è uno storyboard (in questo corso)

Useremo una definizione operativa:

> **Storyboard** = sequenza di immagini (frame) che rappresentano visivamente i singoli shot di una scena o di un intero corto, con indicazioni su inquadratura, azione, luce, dialogo, durata.

Elementi chiave di ogni frame:

- Tipo di inquadratura (wide, medium, close‑up, POV, ecc.).
- Posizione della camera.
- Azione dei personaggi.
- Elementi di ambiente (sfondo, oggetti).
- Mood/luci.
- (Facoltativo) breve didascalia e note tecniche.

### 3.3. Differenza tra mood board e storyboard

**Mood board:**  
Collage visivo che definisce l'estetica, l'atmosfera, i colori, lo stile. Non è sequenziale, non racconta la storia frame per frame.

**Storyboard:**  
Sequenza ordinata di frame che mostra la progressione narrativa shot per shot.

Per approfondire:

- Miro – Storyboard vs. Mood board: [https://miro.com/storyboard/storyboard-vs-moodboard/](https://miro.com/storyboard/storyboard-vs-moodboard/)
- Impress Video – Difference between Storyboard and Mood Board: [https://www.impressvideo.co.uk/vlog/difference-between-storyboard-and-mood-board/](https://www.impressvideo.co.uk/vlog/difference-between-storyboard-and-mood-board/)

---

## 4. Principi di prompting per storyboard

### 4.1. Formula "golden structure"

Struttura minima per un buon prompt di singolo frame:

> **[Stile] + [Soggetto] + [Azione] + [Ambiente] + [Luce] + [Mood]**

Esempio astratto:

> "pencil storyboard sketch, young nurse walks alone down a dimly lit hospital corridor at night, long empty hallway in the background, cold fluorescent lights from above, melancholic and tense mood"

### 4.2. Due livelli di prompt

Nel corso useremo due livelli:

1. **Prompt per singolo frame**  
   - Estremamente dettagliato su inquadratura e azione.
2. **Prompt per sequenza multi‑frame**  
   - Descrive un'intera mini‑storia (4–8 riquadri) in un'unica richiesta.

### 4.3. Principio fondamentale: "Describe the scene, don't just list keywords"

Come insegnato nella guida Google ufficiale:

- **Cattivo prompt:** "hospital, nurse, night, scared"
- **Buon prompt:** "A young nurse walks nervously down a dimly lit hospital corridor at night, holding a medical chart against her chest. The hallway is empty with closed doors on both sides and fluorescent lights casting cold shadows. The mood is tense and melancholic."

### 4.4. Character consistency: il "DNA" del personaggio

Per mantenere lo stesso personaggio in più frame:

- Crea una **character sheet** iniziale (Image 1) con viste multiple (frontale, 3/4, profilo).
- In ogni prompt successivo, cita sempre: "Use the same character as in Image 1, maintaining identical facial features, hairstyle, and body proportions."
- Specifica cosa deve rimanere identico E cosa deve cambiare.

### 4.5. Editing conversazionale > rigenerazione

Invece di rigenerare da zero se un frame non è perfetto:

- Usa comandi di editing mirato: "Keep everything the same but make the lighting more dramatic, with stronger shadows."
- Il modello mantiene la "memoria visiva" del frame precedente.
- Questo minimizza il "drift" (deriva) dei tratti del personaggio.

---

## 5. Struttura delle dispense

Queste dispense sono organizzate in:

1. 01-intro-nano-banana (questo file) – introduzione, risorse, concetti base.
2. [[00_Online/_Pre-produzione audiovisiva e storyboarding con l’IA/05_Template Prompt\|05_Template Prompt]] – template riusabili in italiano per diversi tipi di storyboard.
3. [[00_Online/_Pre-produzione audiovisiva e storyboarding con l’IA/06_Workflow Storyboard\|06_Workflow Storyboard]] – flusso di lavoro integrato Trattamento → Mood Board → Storyboard.
4. [[00_Online/_Pre-produzione audiovisiva e storyboarding con l’IA/07_Case Study_100s\|07_Case Study_100s]] – case study completo di cortometraggio da 100 secondi con tutti i prompt.
5. [[00_Online/_Pre-produzione audiovisiva e storyboarding con l’IA/08_Esercizi didattici\|08_Esercizi didattici]] – esercizi pratici per studenti con obiettivi di apprendimento.

---

## 6. Come usare queste dispense

**Per studenti:**

- Leggi nell'ordine i file 01 → 02 → 03 → 04.
- Guarda i video e leggi le risorse (link).
- Usa i template del file 02 per i tuoi progetti.
- Segui il case study del file 04 per capire il workflow completo.
- Fai gli esercizi del file 05.

**Per docenti:**

- Usa i template come base per lezioni ed esercitazioni.
- Il case study può diventare un progetto di gruppo o individuale.
- Gli esercizi sono scalabili (da 1-2 ore a progetti più lunghi).
- Puoi modificare e adattare tutto il materiale.

---

## 7. Prerequisiti tecnici

### 7.1. Accesso a Nano Banana

- **Google AI Studio** (gratuito, interfaccia web): [https://aistudio.google.com/](https://aistudio.google.com/)
- **Gemini Advanced** (a pagamento, integrato in Google Workspace).
- **Via API** (per chi programma): usa Gemini API con modello `gemini-2.5-flash-image`.

### 7.2. Strumenti complementari consigliati

**Per mood board:**
- Milanote: [https://milanote.com/](https://milanote.com/)
- Miro: [https://miro.com/](https://miro.com/)
- Canva: [https://www.canva.com/](https://www.canva.com/)

**Per assemblaggio storyboard:**
- PowerPoint / Keynote / Google Slides
- Boords: [https://boords.com/](https://boords.com/)
- Adobe Photoshop / Illustrator

**Per organizzazione materiali:**
- Obsidian: [https://obsidian.md/](https://obsidian.md/)
- Notion: [https://www.notion.so/](https://www.notion.so/)

---

## 8. Valutazione e output attesi

Al termine del modulo, ogni studente/ssa produrrà:

1. **Trattamento** (1-2 pagine) per un corto di 60-120 secondi.
2. **Mood board** (1-2 pagine digitali) con sezioni tematiche.
3. **Storyboard completo** (6-12 frame) generato con Nano Banana.
4. **Documento di riflessione** (1 pagina) su:
   - cosa ha funzionato nel prompting;
   - quali difficoltà sono emerse;
   - come l'AI ha influenzato il processo creativo.

---

## 9. Letture e approfondimenti opzionali

**Struttura narrativa per short film:**
- Write Movies – How to Structure a Short Film: [https://writemovies.com/how-to-structure-a-short-film/](https://writemovies.com/how-to-structure-a-short-film/)
- Cloudghostwriting – Story Structure of a Short Film: [https://www.cloudghostwriting.com/blog/how-to-write-the-story-structure-of-a-short-film/](https://www.cloudghostwriting.com/blog/how-to-write-the-story-structure-of-a-short-film/)

**Storyboard best practices:**
- StudioBinder – How to Storyboard a Short Film: [https://www.studiobinder.com/blog/how-to-storyboard-a-short-film/](https://www.studiobinder.com/blog/how-to-storyboard-a-short-film/)
- Boords – How to Storyboard (2025 Guide): [https://boords.com/how-to-storyboard](https://boords.com/how-to-storyboard)
- Meegle – Storyboarding Best Practices: [https://www.meegle.com/en_us/topics/storyboarding/storyboarding-best-practices](https://www.meegle.com/en_us/topics/storyboarding/storyboarding-best-practices)

**Mood board e pre-produzione:**
- StudioBinder – How to Make a Film Mood Board: [https://www.studiobinder.com/blog/how-to-make-a-film-mood-board/](https://www.studiobinder.com/blog/how-to-make-a-film-mood-board/)
- Videomaker – Role of Mood Board in Pre-Production: [https://www.videomaker.com/how-to/planning/organization/the-role-of-the-mood-board-in-pre-production/](https://www.videomaker.com/how-to/planning/organization/the-role-of-the-mood-board-in-pre-production/)

**Esempi di storyboard professionali:**
- StudioBinder – 46 Best Movie Storyboard Examples: [https://www.studiobinder.com/blog/storyboard-examples-film/](https://www.studiobinder.com/blog/storyboard-examples-film/)
- Boords – 28 Best Storyboard Examples: [https://boords.com/storyboard-examples](https://boords.com/storyboard-examples)

---
## 10 Risorse aggiuntive

#### Link utili
- **Accesso gratuito**: [aistudio.google.com](https://aistudio.google.com)
- **Documentazione ufficiale**: [ai.google.dev/gemini-api/docs/image-generation](https://ai.google.dev/gemini-api/docs/image-generation)
- **Github**:  [Casi d'uso Nano Banana](https://github.com/PicoTrex/Awesome-Nano-Banana-images/blob/main/README_en.md#example-91-train-station-movie-poster-by-ai_kei75)
- **Community Educatori**: Forum e gruppi Facebook "AI per la Didattica"

---
**Nota finale:** Tutti i link sono stati verificati alla data di dicembre 2025.
