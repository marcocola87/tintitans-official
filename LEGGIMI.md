# tintitans-official

**Le pagine pubbliche di TinTitans**, servite da GitHub Pages a
`https://marcocola87.github.io/tintitans-official/`.

Il repository del gioco è privato. Questo è pubblico perché Google Play pretende
che certe pagine siano **raggiungibili da chiunque**, anche da chi non ha
installato niente.

## Cosa c'è

| file | indirizzo | a che serve |
|---|---|---|
| `index.html` | `/` | l'informativa sulla privacy, italiano e inglese |
| `elimina-account.html` | `/elimina-account.html` | come cancellare il proprio account |

Tutti e due gli indirizzi sono **incollati nel Play Console** — il primo in
«Norme sulla privacy», il secondo in «Sicurezza dei dati». Cambiare i nomi dei
file vuol dire aggiornarli anche là.

## Perché si chiamava `tintitans-privacy`

Perché è nato per l'informativa e basta. Il 16 settembre 2026, mentre si
compilava la scheda dello store, è stato rinominato in **`tintitans-official`**:
il nome vecchio sarebbe stato stretto il giorno in cui qui dentro ci fosse
qualcosa che privacy non è.

**E i vecchi indirizzi delle pagine NON rimandano al nuovo.** Verificato subito
dopo il rinomina: `marcocola87.github.io/tintitans-privacy/` risponde picche.

E' una distinzione che vale la pena sapere, perché è facile crederci al
contrario: GitHub mantiene i rinvii per gli indirizzi del **repository**
(`github.com/utente/nome`), **ma non per GitHub Pages**. Rinominare un
repository serve le pagine da un indirizzo nuovo e basta — quello vecchio muore.

Per questo è stato fatto **prima della pubblicazione**, quando i due indirizzi
erano scritti in un posto solo: il Play Console. Farlo dopo avrebbe voluto dire
due pagine morte in mano a chi cerca l'informativa.

## Come si modifica

Si modifica il file, si committa, si manda:

```
git add -A
git commit -m "…"
git push
```

GitHub Pages ricostruisce da sé in un minuto o due. Lo stato si guarda con:

```
gh api repos/marcocola87/tintitans-official/pages/builds/latest
```

## Regole per chi scrive qui dentro

**Niente dipendenze.** Nessun Jekyll, nessun tema, nessun foglio di stile
esterno: un file che si apre com'è, si legge sul telefono, e funziona in tema
chiaro e scuro. Un'informativa che non si carica è un'informativa che non esiste.

**Tutto in due lingue**, italiano e inglese, come il gioco.

**L'indirizzo email è `tintitans-privacy@marcocola.com`**, e resta quello: è
scritto nelle pagine e nel Play Console, e non ha niente a che vedere col nome
del repository.

## Quando va aggiornata l'informativa

Ogni volta che il gioco comincia a raccogliere qualcosa che prima non
raccoglieva. In particolare:

- **quando arriverà lo sblocco a pagamento**, perché si aggiungono i dati
  dell'acquisto (che gestisce Google, ma vanno dichiarati);
- **quando arriverà l'uno contro uno**, perché due telefoni si scambieranno
  comandi in tempo reale;
- **se un giorno entrasse un qualunque strumento di analisi**, che oggi non c'è.

E ogni volta si cambia la data di entrata in vigore, in cima.

## Quel che potrebbe arrivare qui

Il ragionamento sta in `documenti/23-il-sito-parcheggio-idee.md`, nel repository
del gioco. In breve: la **classifica mondiale guardabile dal browser** — i dati
si leggono già in pubblico — e, il giorno che ne varrà la pena, il **replay del
record che si rigioca nel browser**, visto che Godot esporta anche per il web.

Non prima della pubblicazione: un sito per un gioco che non si può scaricare è
una vetrina davanti a un negozio chiuso.
