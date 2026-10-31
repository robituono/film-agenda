# Film Agenda

Curated Selection by Robi Tuono: le uscite della settimana (a casa e nelle sale italiane), scelte e commentate.

Sito statico pubblicato con GitHub Pages: `https://robituono.github.io/film-agenda/`

## Com'è fatto

| File | Cosa contiene |
| --- | --- |
| `index.html` | La pagina: mese, settimane, schede film, anno. Non va toccata per aggiornare i film |
| `dati.json` | Tutti i film. Si genera dal foglio Google "Film Streaming – archivio" |
| `locandine/` | Una locandina per film, `<id>.jpg` |
| `tuono-osd.woff2` | Il carattere dei menu (Tuono OSD), ridisegnato da un menu VCR: solo maiuscole |
| `robots.txt` | Chiede ai motori di ricerca di non indicizzare il sito |

## Come si aggiorna

L'aggiornamento lo fa Claude: ricerca dei film, foglio, `dati.json` e locandine, poi un commit su questo repository. GitHub Pages pubblica da solo in circa un minuto.

Per correggere un testo a mano: modifica la cella nel foglio, poi chiedi a Claude di rigenerare `dati.json`.

Nelle note, titoli di film e nomi di persone vanno in grassetto da soli. Se uno sfugge, nel foglio scrivilo tra asterischi: `*Tokyo Sonata*`.

## Caratteri

- Tuono OSD: disegnato per questo sito (menu, titoli, dati).
- Kode Mono (Google Fonts, licenza OFL): testi lunghi.

## Crediti

Dati e locandine da TMDB. Questo prodotto usa l'API di TMDB ma non è approvato né certificato da TMDB. Disponibilità in streaming da JustWatch.
