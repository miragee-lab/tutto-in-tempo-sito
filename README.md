# TuttoInTempo — sito pubblico

Sito di presentazione e privacy policy della beta locale di TuttoInTempo.

- Sito: https://miragee-lab.github.io/tutto-in-tempo-sito/
- Privacy: https://miragee-lab.github.io/tutto-in-tempo-sito/privacy.html
- Repository: https://github.com/miragee-lab/tutto-in-tempo-sito

## Contenuti

`index.html` presenta le categorie e le funzioni, indica che la beta Android è in preparazione e non pubblica collegamenti a un Play Store inesistente. La schermata nella cornice del telefono è una cattura reale della beta, acquisita con un profilo e una scadenza sintetici in un archivio di prova isolato. Non contiene dati dell’utente.

`privacy.html` distingue gli archivi locali dell’app, le esportazioni volontarie e i dati tecnici del sito ospitato da GitHub. **Nome/ragione sociale del titolare e contatto privacy restano da confermare: finché compare l’avviso in sezione 1, il testo è provvisorio e non costituisce l’informativa definitiva per il lancio.**

Pagine statiche senza dipendenze di runtime, moduli di raccolta, cookie o analisi aggiunti dal sito. Logo, immagini, icone e caratteri sono risorse locali. Non contiene sorgenti dell’app, APK, archivi personali o credenziali.

## Grafica

La revisione applica [Emil Kowalski](https://github.com/emilkowalski/skills), [Impeccable](https://github.com/pbakaus/impeccable) e [Taste](https://github.com/Leonxlnx/taste-skill) come evoluzione dell’identità esistente. Le decisioni e i limiti della revisione sono descritti in [DESIGN-NOTES.md](DESIGN-NOTES.md).

- Lora e DM Sans sono ospitati in `assets/fonts/`, con licenze SIL OFL incluse. Il browser del visitatore non contatta Google Fonts.
- Le icone derivano dalla famiglia outline di [Tabler Icons](https://github.com/tabler/tabler-icons); la licenza MIT è in `assets/tabler-LICENSE.txt`.
- `assets/app-preview.png` è una cattura dell’anteprima dell’app, con dati di esempio, prodotta l’8 ottobre 2026. Il file non è un’app funzionante incorporata nella pagina.
- Tema scuro automatico, preferenza di movimento ridotto, focus da tastiera e indice privacy espandibile su telefono.

## Pubblicazione

GitHub Pages pubblica la radice del branch `main`. `.nojekyll` evita elaborazioni Jekyll. Le modifiche inviate a `main` vengono ripubblicate automaticamente da Pages. I collegamenti tra le pagine sono relativi, compatibili con il percorso del repository.

Per il lavoro da un altro computer: clona questo repository, esegui `git pull --ff-only` prima di modificare, controlla i file e poi esegui commit e push. Non sovrascrivere modifiche o usare force push.

## Verifica

Controllare desktop e schermi da 320 px, navigazione con tastiera, apertura delle FAQ e collegamenti alla privacy. Dopo una pubblicazione verificare gli URL HTTPS del sito e della privacy. Non introdurre strumenti di tracciamento o collegamenti al download senza aggiornare testi e informativa.

Fonti per l’informativa:

- [Garante — Informativa e doveri](https://www.garanteprivacy.it/home/docweb/-/docweb-display/docweb/8981258)
- [Garante — I miei diritti](https://www.garanteprivacy.it/i-miei-diritti)
- [GitHub — Privacy statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement)

La pagina descrive il progetto e non ospita vendite, pagamenti o un servizio SaaS. Prima di introdurre transazioni valutare un hosting adatto e le [condizioni di GitHub Pages](https://docs.github.com/en/site-policy/github-terms/github-terms-for-additional-products-and-features).
