# UI/UX & Frontend Engineering Guidelines

## 1. Palette Cromatica & Contrasti
- Evita colori primari saturi al 100% (niente #0000FF o #FF0000 puri).
- Adotta temi scuri moderni a contrasto multilivello (sfondo: `#09090b` / `zinc-950`, card/superfici: `#18181b` / `zinc-900`, bordi: `#27272a` / `zinc-800`).
- Dettagli di accento: usa tinte sfumate (emerald, cyan, violet o ambra) con leggeri bagliori radiali di sfondo (radial glow/ambient light).

## 2. Tipografia & Gerarchia Visiva
- Titoli d'impatto con spaziatura stretta (`tracking-tight`) e font sans-serif geometrici (es. Inter, Geist, Mona Sans).
- Testo corpo ad alta leggibilità con colore smorzato rispetto al titolo (`zinc-400` / `leading-relaxed`).
- Etichette tecniche o badge in monospace compatto (`font-mono text-xs uppercase tracking-wider`).

## 3. Componenti & Micro-Interazioni
- Bordi ultra-sottili semi-trasparenti (`border border-white/10` o `border-zinc-800`) per dare profondità moderna senza appesantire.
- Transizioni fluide su ogni interazione (`transition-all duration-200 ease-out`).
- Hover states curati: sollevamento impercettibile (`hover:-translate-y-0.5`) e aumento lieve di luminosità del bordo (`hover:border-zinc-700`).
- Feedback di caricamento: niente layout che "saltano", impiega sempre scheletri di caricamento (skeleton shimmer) o indicatori compatti.

## 4. Layout & Spaziature
- Griglie responsive strutturate con gap generosi (`gap-6` o `gap-8`).
- Sezioni ampie con padding verticale abbondante (`py-16` o `py-24`) per dare respiro al design.
