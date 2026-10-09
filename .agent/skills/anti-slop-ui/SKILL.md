---
name: anti-slop-ui
description: Istruzioni vincolanti per design web moderno, UX raffinata, performance ed eliminazione dei pattern IA generici (AI slop).
---

# Regole di Design & Frontend Craftmanship

Quando progetti o implementi interfacce web, devi seguire rigorosamente questi canoni:

### 1. Niente "AI Slop" & Palette Generiche
- VIETATO l'uso del classico gradiente viola/indaco/rosa o delle card scure generiche con bordo semitrasparente se non espressamente richiesto.
- Usa una palette deliberata: 1 colore d'accento deciso, 1 neutro caldo o freddo per i testi/sfondi, e stati di hover/focus coerenti.
- Spaziature armoniche basate su griglia 4px/8px (usa `gap-2`, `gap-4`, `gap-6`, `p-6` in modo matematico e coerente).
- Tipografia: Definisci una gerarchia severa (massimo 2 font, 1 per titoli e 1 per body). Usa `clamp()` o scale `text-sm`, `text-base`, `text-2xl`, `text-4xl` con line-height bilanciata.

### 2. Mobile-First & Responsive Moderno
- Scrivi CSS/Tailwind pensando prima allo smartphone e poi al desktop (`sm:`, `md:`, `lg:`).
- Usa le unità di misura viewport moderne: `dvh` anziché `vh` per evitare problemi con la barra degli indirizzi sui browser mobili.
- Zero overflow orizzontale: nessun elemento deve mai rompere la larghezza dello schermo su viewport 360px.
- Usa CSS Grid e Flexbox moderni; prediligi container queries (`@container`) quando progetti componenti riutilizzabili.

### 3. Componentistica & UI Patterns
- Se usi React/Next/Vite, preferisci componenti headless o accessibili stile **shadcn/ui**, **Radix UI** o **Tailwind UI**.
- Ogni pulsante o elemento interattivo DEVE avere:
  - Stato di `:hover` visibile ma discreto (transizioni da 150-200ms).
  - Stato di `:active` (leggera pressione o feedback tattile).
  - Stato di `:focus-visible` chiaro per navigazione da tastiera.
  - Cursore appropriato (`cursor-pointer`).

### 4. Performance & Core Web Vitals
- Ottimizzazione immagini: usa sempre tag moderni con `loading="lazy"`, dimensioni esplicite (`width`/`height` o `aspect-ratio`) per prevenire Layout Shift (CLS).
- Evita bundle JS pesanti per animazioni semplici: usa transizioni CSS native o micro-librerie leggere.
- Icone: Usa set SVG moderni e coerenti (Lucide Icons, Heroicons).