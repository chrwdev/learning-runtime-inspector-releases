# Learning Runtime Inspector — installazione

**Learning Runtime Inspector (LRI)** è un'applicazione desktop per lanciare e ispezionare learning
object SCORM in locale, senza un LMS.

Gli installer sono pubblicati nel repository
[learning-runtime-inspector-releases](https://github.com/chrwdev/learning-runtime-inspector-releases);
il codice sorgente è in un repository separato.

> NOTE: questo file è anche il README del repository degli installer: il workflow di release lo
> copia lì a ogni versione. Va modificato solo nel repository del codice (`docs/INSTALLAZIONE.md`).

## Scaricare

Apri l'[ultima versione](https://github.com/chrwdev/learning-runtime-inspector-releases/releases)
e scarica il file per il tuo sistema:

| Sistema                       | File                               |
| ----------------------------- | ---------------------------------- |
| macOS (Apple Silicon e Intel) | `LRI-<versione>-mac-universal.dmg` |
| Windows 10/11 (64 bit)        | `LRI-<versione>-win-x64.exe`       |

Gli installer non sono ancora firmati: al primo avvio macOS e Windows mostrano un avviso. È
previsto, e qui sotto c'è come superarlo.

## macOS

1. Apri il `.dmg` e trascina **Learning Runtime Inspector** nella cartella **Applicazioni**.
2. Avvia l'app. Al primo avvio macOS avvisa che non può verificare lo sviluppatore.
3. Apri **Impostazioni di Sistema → Privacy e sicurezza**, scorri fino al messaggio su
   "Learning Runtime Inspector" e clicca **Apri comunque**, poi conferma.
   - Su macOS 14 o precedenti basta anche: tasto destro sull'app → **Apri** → **Apri**.

L'operazione va fatta una sola volta per versione.

In alternativa, da Terminale:

```bash
xattr -dr com.apple.quarantine "/Applications/Learning Runtime Inspector.app"
```

## Windows

1. Avvia `LRI-<versione>-win-x64.exe`.
2. Se compare **"Windows ha protetto il PC"** (SmartScreen), clicca **Ulteriori informazioni →
   Esegui comunque**.
3. Segui l'installazione: non servono permessi di amministratore e puoi scegliere la cartella.

Per disinstallare: **Impostazioni → App → App installate → Learning Runtime Inspector**.

## Aggiornamenti

Per ora gli aggiornamenti sono manuali: scarica e installa la nuova versione sopra la precedente.
In una prossima versione l'app avviserà quando ne è disponibile una nuova (e su Windows si
aggiornerà da sola).

## Segnalare un problema

1. Menu **Help → Open Logs Folder** e allega il file `main.log` alla segnalazione.
2. Indica la versione di LRI (la trovi nel menu **Help**), il sistema operativo e, se possibile,
   il pacchetto SCORM usato o uno che riproduce il problema.
3. Invia la segnalazione al responsabile del progetto, oppure apri una issue nel repository del
   codice se vi hai accesso.
