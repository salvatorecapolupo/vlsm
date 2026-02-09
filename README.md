# 🧮 VLSM Calculator

Questo software è uno strumento web *client-side* progettato per la pianificazione di reti IP utilizzando la tecnica **VLSM** (Variable Length Subnet Mask). A differenza dei calcolatori standard, questo tool integra un motore di rendering matematico (KaTeX) che mostra in tempo reale le formule utilizzate per calcolare l'allocazione degli host e il CIDR.

### 🚀 Live Demo

Puoi vedere l'applicazione in funzione qui:
👉 **[https://salvatorecapolupo.github.io/vlsm/](https://salvatorecapolupo.github.io/vlsm/)**

---

### ✅ Pregi

* **Approccio Didattico (LaTeX):** Non si limita a dare il risultato, ma spiega il *perché*. Mostra i passaggi matematici () per ogni sottorete, rendendolo ideale per studenti e docenti.
* **Algoritmo di Ottimizzazione:** Applica automaticamente la regola d'oro del VLSM, riordinando le richieste dalla più grande alla più piccola per evitare la frammentazione dello spazio di indirizzamento.
* **Zero Dipendenze Server:** L'intera logica è scritta in JavaScript puro. Funziona offline (una volta caricata la libreria KaTeX) e non richiede backend.
* **Interfaccia Reattiva:** Permette di aggiungere o rimuovere dinamicamente le sottoreti e ricalcola l'intera topologia istantaneamente.

### ⚠️ Limiti

* **Solo IPv4:** Il software gestisce esclusivamente indirizzi IPv4 a 32 bit; non supporta l'indirizzamento IPv6.
* **Assenza di Persistenza:** Non utilizzando un database o il *local storage*, i dati inseriti vanno persi se si aggiorna la pagina.
* **Validazione Base:** Il controllo sugli input verifica la sintassi dell'IP, ma non impedisce l'uso di indirizzi riservati (es. classi D/E o loopback) se inseriti come rete principale.
