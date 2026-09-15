# tintitans-privacy

**L'informativa sulla privacy di TinTitans, pubblicata su GitHub Pages.**

Questo repository esiste per una ragione sola: Google Play pretende che
l'informativa stia a un **indirizzo pubblico raggiungibile da chiunque**, anche
da chi non ha installato il gioco. Il repository del gioco è privato, quindi
serviva un posto pubblico separato.

## Come si pubblica

1. Crea il repository su GitHub: **pubblico**, nome `tintitans-privacy`
2. Dalla cartella di questo file:

   ```
   git init
   git add -A
   git commit -m "L'informativa sulla privacy"
   git branch -M main
   git remote add origin https://github.com/marcocola87/tintitans-privacy.git
   git push -u origin main
   ```

3. Su GitHub: **Settings → Pages → Source: Deploy from a branch → main / (root)**

Dopo qualche minuto la pagina è a:

```
https://marcocola87.github.io/tintitans-privacy/
```

È quello l'indirizzo da incollare nel Play Console, in **Norme sulla privacy**.

## Prima di pubblicare: due cose da sostituire

Nel file `index.html` ci sono due segnaposto, uno per lingua:

```
[INDIRIZZO EMAIL DI CONTATTO]
[CONTACT EMAIL ADDRESS]
```

**Vanno sostituiti con un indirizzo email vero**, perché è lì che arriveranno le
richieste di cancellazione — ed è un obbligo, non una cortesia.

Conviene che sia un indirizzo **dedicato** e non quello personale di tutti i
giorni: finisce su una pagina pubblica, quindi verrà raccolto dai robot che
cercano indirizzi. Qualcosa come `tintitans@…` va benissimo.

Lo stesso indirizzo serve anche nel Play Console come **email di assistenza**.

## Perché è una pagina HTML e basta

Niente Jekyll, niente tema, niente dipendenze: un file che si apre com'è, si
legge sul telefono, e funziona in tema chiaro e scuro. Un'informativa privacy che
non si carica è un'informativa che non esiste.

## Quando va aggiornata

Ogni volta che il gioco comincia a raccogliere qualcosa che prima non
raccoglieva. In particolare:

- **quando arriverà lo sblocco a pagamento**, perché si aggiungono i dati
  dell'acquisto (che gestisce Google, ma vanno dichiarati);
- **quando arriverà l'uno contro uno**, perché due telefoni si scambieranno
  comandi in tempo reale;
- **se un giorno entrasse un qualunque strumento di analisi**, che oggi non c'è.

E ogni volta si cambia la data di entrata in vigore, in cima.
