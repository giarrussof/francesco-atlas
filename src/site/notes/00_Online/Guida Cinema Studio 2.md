---
{"dg-publish":true,"dg-path":"Guida Cinema Studio 2.md","permalink":"/guida-cinema-studio-2/"}
---


# Guida completa a Cinema Studio 2.0 di Higgsfield  
## Workflow per un breve video (Retro Sci‑Fi Anni '70)

## 1. Panoramica

Cinema Studio 2.0 è uno strumento di AI generativa video che permette di creare brevi sequenze cinematografiche controllando:

- personaggi
- ambienti
- movimenti di camera
- emozioni

Questa guida mostra passo‑passo come creare un breve video con:

- **Personaggio:** astronauta donna in stile retro sci‑fi anni '70  
- **Ambiente:** sala controllo analogica di un'astronave alla deriva  
- **Stile visivo:** monitor CRT verdi, pulsanti analogici, cavi spessi, luce cinematografica, lente anamorfica, grana pellicola 35mm

---

## 2. Accesso e interfaccia

### 2.1 Accesso a Cinema Studio 2.0

1. Vai su https://higgsfield.ai/
2. Crea un account o accedi
3. Dall'interfaccia principale, entra in **Cinema Studio 2.0**

### 2.2 Modalità Principali

- **Image Mode**: creazione e refining del personaggio
- **Video Mode**: creazione di clip video (Single Shot, Multishot Automatico, Multishot Manuale)

---

## 3. Fase 1 – Creazione del personaggio

### 3.1 Prompt di base

Definisci il personaggio principale e il suo ambiente in modo chiaro e coerente.

**Prompt di partenza:**
```text
1970s retro sci-fi movie still. A female astronaut wearing a bulky, 
weathered orange and white spacesuit with a domed glass helmet. She is 
standing in the dimly lit, analog control room of a derelict spaceship. 
CRT monitors glowing green, analog buttons, thick cables. Cinematic 
lighting, anamorphic lens, 35mm film grain, moody atmosphere.
```

**Best practices:**

- Menziona sempre a seconda delle necessità questi elementi:
  - tuta arancione/bianca
  - casco a cupola
  - control room analogica
  - monitor CRT verdi
  - cavi spessi e pulsanti analogici
  - estetica 1970s retro sci‑fi, 35mm grain

### 3.2 Parametri di generazione immagine

Imposta, ad esempio:

- **Aspect Ratio:** 21:9 (cinematografico)
- **Risoluzione:** 2K (bilanciata)
- **Camera:** 8K Digital Camera
- **Lente:** Anamorfica
- **Focale:** 35mm o 50mm

Genera 1–4 immagini, scegli quella con:

- personaggio leggibile
- ambiente retro ben definito
- illuminazione cinematografica coerente

---

## 4. Fase 2 – Angles: Inquadrature multiple del personaggio

### 4.1 Editor "Angles"

A partire dall'immagine scelta:

- Apri l'editor **Angles**
- Ruota la camera intorno all'astronauta (360°)
- Varia tilt (alto/basso) e pan (sinistra/destra)

### 4.2 "Generate from 12 Best Angles"

Utilizza la funzione automatica per ottenere 12 inquadrature:

- frontale, profili, 3/4
- angolazioni dall'alto e dal basso
- tutte con:
  - stessa astronauta
  - stessa sala controllo analogica
  - stesso look anni '70

Queste immagini serviranno per "addestrare" il personaggio in modalità video.

---

## 5. Fase 3 – Creare il personaggio in libreria (Video Mode)

1. Vai in **Video**
2. Clicca su **Add Character and Props**
3. Premi **+** per aggiungere un nuovo personaggio
4. Carica 4–8 inquadrature migliori (da Angles)
5. Dai un nome, es. `@astronaut`
6. Aggiungi una descrizione breve, es.:

   > "female astronaut in bulky orange and white spacesuit, domed glass helmet, 1970s retro analog spaceship control room"

Il nome `@astronaut` verrà usato in tutti i prompt video.

---

## 6. Fase 4 – Modalità di creazione video

### 6.1 Le tre modalità

1. **Single Shot**
   - Una singola scena alla volta
   - Utile per test e clip isolate

1. **Multishot automatico**
   - Sequenza generata dall'AI partendo da un prompt unico
   - Poco controllo sulle singole inquadrature

1. **Multishot manuale (consigliato)**
   - Fino a 6 scene consecutive
   - Controllo pieno su prompt, movimento camera, durata, emozione per ogni scena
   - Output già montato

Per un breve video narrativo, useremo **Multishot manuale**.

---

## 7. Multishot manuale – struttura della sequenza

### 7.1 Setup iniziale

1. In **Video**, scegli **Multishot Manual**
2. Di default avrai 2 scene; puoi aggiungerne fino a 6
3. Per ogni scena imposti:
   - Start frame
   - Prompt
   - Movimento camera
   - Durata
   - Emozione
   - Parametri generali (AR, risoluzione, ecc.)

### 7.2 Parametri consigliati (comuni a tutte le scene)

- **Aspect Ratio:** 21:9
- **Risoluzione:** 2K
- **Content Type:** General
- **Camera / Lens (derivano dallo stile dei prompt):**
  - Cinematic lighting
  - Anamorphic lens
  - 35mm film grain

---

## 8. Prompt di scena 

### 8.1 Scena 1 – Esplorazione della sala controllo

**Obiettivo narrativo:** introdurre il personaggio e lo spazio.

**Prompt esempio:**
```text
@astronaut is walking slowly through the dimly lit analog control room 
of the derelict spaceship. Long shot showing the bulky orange and white 
spacesuit, the domed glass helmet, and rows of green-glowing CRT monitors, 
analog buttons and thick cables. 1970s retro sci-fi aesthetic, cinematic 
lighting, anamorphic lens, 35mm film grain.
```

**Impostazioni tipiche:**

- Start frame: una delle inquadrature long shot da Angles
- Movimento camera: Auto o leggero Dolly In
- Durata: 5 s
- Emozione: Neutral

---

### 8.2 Scena 2 – Scoperta dell'allarme

**Obiettivo narrativo:** il personaggio si accorge che qualcosa non va.

**Prompt esempio:**
```text
@astronaut notices critical warning signals flashing on the CRT monitors. 
Green phosphor displays show alarm messages and glitching data. She realizes 
something is wrong in the derelict spaceship. Same 1970s retro analog control 
room, moody cinematic lighting, 35mm film grain.
```

**Impostazioni tipiche:**

- Start frame: frame finale della Scena 1
- Movimento camera: Auto o Pan verso i monitor
- Durata: 4 s
- Emozione: Fearful (preoccupata/spaventata)

---

### 8.3 Scena 3 – Reazione al pericolo

**Obiettivo narrativo:** l'astronauta reagisce, tenta di intervenire.

**Prompt esempio:**
```text
@astronaut quickly moves to the main analog control panel, 
hands reaching for switches and buttons to handle the emergency. 
The bulky orange spacesuit catches the green CRT glow, thick cables 
hanging in the background. 1970s retro sci-fi mood, anamorphic lens 
flares, 35mm film grain.
```

**Impostazioni tipiche:**

- Start frame: frame finale della Scena 2
- Movimento camera: Dolly In o Auto
- Durata: 6 s
- Emozione: Angry (determinata/risoluta)

---

### 8.4 Scena 4 – Visione della minaccia

**Obiettivo narrativo:** climax percettivo, rivelazione della minaccia esterna.

**Prompt esempio:**
```text
@astronaut is terrified as she stands in the flickering analog control room, 
red emergency lights mixing with the green CRT glow. Through the large viewport 
window she sees a massive alien structure slowly approaching the derelict 
spaceship. Her reflection is visible in the domed glass helmet, surrounded by 
thick cables and vintage consoles. 1970s retro sci-fi movie still, cinematic 
lighting, anamorphic lens, 35mm film grain.
```

**Camera movement (da impostare nei controlli):**

- Tilt Up + Behind the Back  
  (la camera dietro l'astronauta sale e rivela il viewport con la struttura aliena)

**Impostazioni tipiche:**

- Start frame: frame finale della Scena 3
- Durata: 7 s
- Emozione: Fearful (terrore)

---

## 9. Emozioni: Progressione coerente

Esempio di arco emotivo in 4 scene:

1. **Scena 1 – Esplorazione:** Neutral  
2. **Scena 2 – Allarme sui CRT:** Fearful  
3. **Scena 3 – Intervento sui pannelli:** Angry (determinazione)  
4. **Scena 4 – Visione struttura aliena:** Fearful (terrore)

La progressione emotiva contribuisce alla coerenza narrativa del breve video.

---

## 10. Coerenza di ambiente e stile

Per evitare incoerenze:

- Mantieni sempre:
  - "analog control room of a derelict spaceship"
  - "CRT monitors glowing green"
  - "analog buttons, thick cables"
  - "1970s retro sci-fi aesthetic"
  - "cinematic lighting, anamorphic lens, 35mm film grain"
- Non introdurre ambienti diversi (niente deserti, città, ecc.)
- Usa sempre il personaggio definito (`@astronaut`) con tuta arancione/bianca e casco a cupola

---

## 11. Raccordi tra le scene

Per creare transizioni fluide:

1. Usa il **frame finale** di una scena come **start frame** della successiva
2. Mantieni continuità di:
   - postura del personaggio
   - direzione dello sguardo
   - illuminazione generale
3. Sfrutta movimenti di camera coerenti:
   - se una scena termina con un movimento in avanti, la successiva può iniziare da una posizione leggermente più avanti, mantenendo l'azione fluida

Esempio:

- Fine Scena 3: close/medium shot dell'astronauta sui controlli  
- Inizio Scena 4: camera dietro di lei (Behind the Back), poi Tilt Up verso il viewport.

---

## 12. Best Practices sui prompt (solo astronauta)

**Prompt essenziale (debole):**
```text
@astronaut walks in the room
```

**Prompt forte:**
```text
@astronaut is walking slowly through the dimly lit analog control room 
of the derelict spaceship. Wide shot showing the weathered orange and 
white spacesuit, domed glass helmet, and rows of green CRT monitors. 
1970s retro sci-fi aesthetic, cinematic lighting, 35mm film grain.
```

**Prompt bilanciato per azione:**
```text
@astronaut cautiously approaches the main control panel. CRT monitors 
glowing green, analog buttons and thick cables around her. Medium shot, 
1970s retro sci-fi control room, moody cinematic lighting, 35mm film grain.
```

Linee guida:

- Non essere troppo vago
- Non scrivere romanzi: 2–3 frasi chiare bastano
- Richiama sempre gli stessi elementi chiave (CRT, cavi, estetica anni '70)

---

## 13. Generazione, download e montaggio

### 13.1 Generazione

- Dopo aver impostato tutte le scene in Multishot Manuale:
  - clicca **Generate**
  - attendi l'elaborazione
  - controlla il video risultante

### 13.2 Download

- Dalla libreria progetti:
  - seleziona la sequenza
  - scarica in MP4 o MOV (a seconda del flusso di lavoro)

### 13.3 Assemblaggio in Post‑produzione

Importa le clip in un software di editing (DaVinci Resolve, Premiere, ecc.):

- ordina le sequenze in timeline
- controlla i raccordi
- eventualmente aggiungi:
  - musica
  - effetti sonori
  - un leggero color grading aggiuntivo (mantenendo il look 35mm)

---

## 14. Uso didattico per studenti

Ambiti:

- **Media Studies / Film Studies**
  - grammatica cinematografica
  - movimenti di camera
  - raccordi e continuità

- **Visual Communication**
  - coerenza stilistica (retro sci‑fi anni '70)
  - uso della palette cromatica (verde CRT, rossi d'emergenza, ombre bluastre)

- **Storytelling digitale**
  - scrittura di prompt come micro‑sceneggiatura
  - arco emotivo del personaggio in breve durata

---

## [[00_Online/Vademecum Cinema Studio 2\|15. Sintesi operativa (checklist)]]

1. Definisci il personaggio (astronauta retro sci‑fi) con il prompt base
2. Genera l'immagine migliore del personaggio
3. Usa **Angles** per ottenere 12 inquadrature coerenti
4. Crea il personaggio `@astronaut` in Video Mode caricando 4–8 immagini
5. In Multishot Manuale:
   - imposta 4 scene (esplorazione, allarme, reazione, climax)
   - scrivi prompt coerenti (solo ambientazione astronave retro)
   - assegna emozioni e movimenti di camera
6. Genera la sequenza
7. Scarica il video e rifinisci in montaggio

