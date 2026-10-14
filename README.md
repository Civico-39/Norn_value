# Un bacino normale

Una lontra scivola giù dalla funzione di ripartizione della normale, Φ(x),
corre verso lo schermo e ti lascia un bacino sul vetro.

## Come pubblicarla su GitHub Pages

1. Crea un repository (anche privato, se il tuo piano lo permette) e carica `index.html`.
2. Vai su **Settings → Pages**, scegli il branch `main` e la cartella `/ (root)`.
3. Dopo un minuto la pagina è su `https://<tuo-utente>.github.io/<nome-repo>/`.

Serve internet: la grafica 3D (three.js) e il carattere arrivano da CDN.

## Cosa si cambia facilmente (tutto dentro `index.html`)

| Cosa | Dove |
|---|---|
| La scritta del bacio (`Smack!`) | costante `SCRITTA` all'inizio dello script |
| Il titolo della scheda | tag `<title>` |
| I colori della lontra | oggetto `PELO` nella sezione "Lontra" |
| I colori della pagina, chiaro e scuro | variabili `--bg`, `--kiss`, `--accent`… in cima allo stile |
| L'altezza della curva | costante `HC` (la larghezza si adatta da sola allo schermo, in `scalaPer`) |
| I tempi di ogni momento | campo `d` di ogni fase nella sezione "Regia" |

Con "Riduci movimento" attivo nel sistema, la lontra compare già davanti allo schermo con il bacio sul vetro.
