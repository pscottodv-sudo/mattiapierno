# mattiapierno.it

Portfolio di Mattia Pierno, regista e filmmaker. Sito statico per GitHub Pages, con pannello per modificarlo.

## Struttura

```
index.html      ← il sito (legge tutto da content.json)
content.json    ← testi, film, crediti, impostazioni della pellicola
foto/           ← fotogrammi a piena qualità
img/g, img/t    ← copie leggere per la pellicola 3D e per il pannello
admin/          ← pannello (mattiapierno.it/admin/)
```

## Messa online (una volta sola)

1. Crea un repository su GitHub (es. `mattiapierno/sito`) e carica tutti questi file nella radice.
2. Settings → Pages → Source: `Deploy from a branch`, branch `main`, cartella `/ (root)`.
3. Settings → Pages → Custom domain: `mattiapierno.it`. Poi, dal pannello del dominio, punta i record DNS a GitHub Pages
   (A `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153` e CNAME `www` → `<utente>.github.io`).
4. Facoltativo: crea un modulo su formspree.io e incolla il suo indirizzo in Pannello → Contatti.
   Finché è vuoto, il modulo dei contatti apre l'app email di chi scrive con il messaggio già pronto.

## Pannello

Vai su `mattiapierno.it/admin/`, scrivi il repository (es. `mattiapierno/sito`) e incolla un token GitHub:
github.com/settings/personal-access-tokens/new → Only select repositories → il repository del sito →
Repository permissions → Contents: Read and write.

Dal pannello si aggiungono film (link Vimeo, YouTube o del player Adobe, durata, crediti, fotogrammi),
si scelgono i film che escono dalla pellicola e come si muove, si cambiano testi, collaborazioni e contatti.
"Anteprima" mostra il sito con le modifiche prima di pubblicarle; "Pubblica" salva tutto in un solo commit.
