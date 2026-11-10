# 🧩 Quizzettini - Daily Quiz Italiano

Benvenuti su **Quizzettini**, una dashboard minimale e moderna creata per raccogliere i migliori **Daily Quiz** e party game in lingua italiana (e internazionali).

L'obiettivo di questa pagina è offrire un punto di accesso rapido, organizzato e tracciabile ai quiz giornalieri.

## 🚀 Caratteristiche Principali

- 🎨 **Interfaccia Moderna & Adattiva:** Design curato con tema scuro predefinito (*Dark Mode*) e supporto automatico al tema chiaro (*Light Mode*) in base alle preferenze del sistema.
- 🕒 **Orologio in Tempo Reale:** Navbar con data e ora locale sempre aggiornata.
- 📊 **Barra di Progresso & "Sorprendimi":** Monitora in tempo reale quanti quiz giornalieri hai completato oggi (con percentuale) oppure clicca su **Sorprendimi** per far scegliere casualmente un quiz non ancora completato.
- 🔍 **Ricerca Rapida & Filtri per Categoria:** Filtra istantaneamente i quiz per nome tramite la barra di ricerca o naviga per categoria (*Tutti*, *Parole & Enigmi*, *Geografia*, *Cultura & Media*, *Party & Illimitati*).
- ✅ **Sistema di Tracciamento Completati:** Segna manualmente i quiz vinti/completati tramite il pulsante dedicato con la spunta verde accanto ad ogni gioco:
    - Il quiz viene sbarrato e il contatore di progresso si aggiorna.
    - Puoi annullare lo stato in qualsiasi momento cliccando nuovamente sulla spunta.
    - Lo stato si resetta automaticamente **24 ore dopo il completamento**.
- 📱 **Totalmente Responsive & Accessibile:** Ottimizzato per PC, Tablet e Smartphone (fino a 360px senza overflow) con supporto alla navigazione da tastiera e riduzione del movimento (`prefers-reduced-motion`).

## 🕹️ Quiz Inclusi

La lista include 27 giochi suddivisi in quattro categorie:
*   **Parole & Enigmi:** Frase Fortunata, Parola Chiave, Catena Daily, Wordle, Quordle, Fuochino, Best Guess, Perceptle, Dialed Color², Dialed Shape.
*   **Geografia:** Angle, Guess The Angle, Travel, Globle, Flagle, TimeGuessr.
*   **Cultura & Media:** Songless, Minecraftle, Daily Red, CronoNews, Food Guesser, Gamedle.
*   **Party & Illimitati:** Guess The Age, Higher Or Lower, Linkedin Or Interpol, Jeopardy, Card Against Humanity (con menu rapido per *Pretend You're CLRTD* versione LagXCVII e lista *Mazzi*).

## 🛠️ Tecnologie Utilizzate

Questo progetto è una web app **Vanilla** leggera e senza dipendenze esterne di runtime:
- **HTML5**
- **CSS3** (Design Tokens, Flexbox, animazioni native)
- **JavaScript (ES6+)**

## 📦 Installazione Locale

Se vuoi scaricare il progetto sul tuo computer:
1. Clona il repository:
   ```bash
   git clone https://github.com/CiccioLagXCVIII/DailyQuizItaliano.git
   ```
2. Apri il file `index.html` direttamente nel tuo browser.

## 📝 Note Tecniche Sullo Stato Completato
Il sistema di tracciamento non salva dati su server: tutto viene memorizzato localmente nel browser tramite `localStorage` (`played_<nome_quiz>`).  
I party game multi-sessione puri (*Jeopardy* e *Card Against Humanity*) sono esclusi dal pulsante di completamento giornaliero e dal calcolo della barra di progresso.

---

Creato con ❤️ da [CiccioLagXCVIII](https://github.com/CiccioLagXCVIII)
