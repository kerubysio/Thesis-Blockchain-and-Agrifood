# Argomento della tesi

Agrifood e tecnologia blockchain
Verifica stato attuale di implementazione e uso per certificare i
processi di produzione agricola
Cercare tipologie fallite e di successo
Linguaggi utilizzati
Progetto più di successo
Progetti falliti e comune denominatore tra di essi se lo trovi
Includendo blog e materiale grigio
Ossia materiale non scientifico ma prodotto dagli autori o giornalisti

Per quanto riguarda la struttura della tesi può procedere al contrario: ricercando informazioni sull'adozione delle tecnologie blockchain nel settore agrifood, ogni volta che trova nomi e concetti tecnici che necessitano di spiegazione, li aggiunge ad un capitolo di "concetti principali". alla fine di questo lavoro di ricerca aggiungerà (nell'introduzione)
anche delle definizioni comuni per la blockchain, l’algoritmo di consenso, la politica di gestione e conclusioni

# Materiale da studiare

come riferimenti (soprattutto per i termini e per eventuali approfondimenti) può usare
[Intro to Ethereum](https://ethereum.org/en/developers/docs/intro-to-ethereum "https://ethereum.org/en/developers/docs/intro-to-ethereum")

per gli aspetti architetturali:
[Aspetti architetturali](https://web.archive.org/web/20240901090042/https://blog.ipfs.tech/dapps-ipfs/#primer-on-web-app-architectures-spas-mpa-pwa-and-dapps "https://web.archive.org/web/20240901090042/https://blog.ipfs.tech/dapps-ipfs/#primer-on-web-app-architectures-spas-mpa-pwa-and-dapps")

Un buon confronto tra le diverse blockchain, con definizioni, caratteristiche principali, ecc. è questo:
[Confronto tra blockchain](https://doi.org/10.1016/j.cosrev.2023.100575 "https://doi.org/10.1016/j.cosrev.2023.100575") (non è necessario scendere nel dettaglio della descrizione tecnica, ma è buono capire quali varianti ci sono, cosa e significa quella variante)

# Cose da tenere a mente

Presenti anche in [[RICORDA]]
Archive.org (https://web.archive.org)
Google Scholar
Scopus
(Se fai login con unina su questi siti puoi scaricare materiale pdf)

Conserva tutto il materiale che utilizzi (pdf, siti web, articoli, ecc)

Segnare le parole chiave usate per la ricerca su Scholar, Scopus ecc.

Connected Papers è un sito che, usando il titolo di un articolo scientifico, il DOI o l'arXiv ID, mostra articoli che citano o che sono citati da quell'articolo. I più citati sono di solito più importanti.

Osserva bene il titolo e l’abstract. Poi leggi introduzione e conclusioni. Nient’altro.

# Consigli di ChatGpt

Per prima cosa prova a vedere la tesi come un viaggio che parte da un fatto concreto – l’uso della blockchain nell’agrifood – e poi risale pian piano alle radici teoriche e tecniche che lo sostengono. Immagina di scoprire prima che cosa si sta facendo “oggi” (i casi di successo, quelli falliti, i linguaggi usati, il materiale non convenzionale) e poi di costruire man mano il tuo apparato di definizioni e concetti per far capire al lettore perché tutto questo funziona (o perché non ha funzionato).

Ti suggerisco di cominciare dall’**introduzione**, dove presenti l’obiettivo generale: capire a che punto siamo con l’adozione della blockchain nell’agrifood, con un cenno veloce alle ragioni del tuo interesse (trasparenza, tracciabilità, certificazione). Qui puoi già accennare che seguirai un approccio “dal concreto al concetto”: prima esporrai progetti reali, poi costruirai il capitolo dei concetti fondamentali e infine offrirai le conclusioni sullo stato dell’arte.

Quando incontri nomi tecnici o concetti che ritieni non scontati, fermati e trascrivili in un documento di lavoro che diventerà il **capitolo dei “concetti principali”**. Lì, a posteriori, spiegherai cosa si intende con “algoritmo di consenso”, quali sono le principali politiche di governance di una blockchain permissioned versus permissionless, e da dove nasce l’esigenza di tokenizzare un bene agricolo. In tal modo, mentre navighi tra casi concreti, costruisci un glossario che servirà poi al lettore per orientarsi.

Nel **capitolo successivo** puoi focalizzarti sulle “tipologie di progetto”, raccontando una o due esperienze di successo e una o due di insuccesso. Descrivi la “storia” di ognuno: quali erano gli obiettivi, come si sono mosse organizzazione e sviluppatori, quali ostacoli tecnici o culturali hanno incontrato. Quando un progetto si interrompe, cerca di isolare il “comune denominatore” dei fallimenti (ad esempio bassissima adozione da parte degli agricoltori, difficoltà nell’integrazione con sistemi gestionali preesistenti, costi di transazione troppo elevati).

Subito dopo, dedica un quarto capitolo ai **linguaggi e alle piattaforme**: confronta Solidity, Go, JavaScript (usati per smart contract su Ethereum) con Chaincode di Hyperledger Fabric scritto in Go, o con linguaggi emergenti in soluzioni permissioned. Per ciascuno spiega pregi e limiti in termini di performance, sicurezza e facilità di apprendimento per team con background agrario piuttosto che informatico.

Non dimenticare, lungo tutto il percorso, di includere anche **materiale grigio**: blog di aziende blockchain, post di LinkedIn da parte di start-up agritech, white paper di consorzi di filiera e articoli giornalistici specializzati. Molte volte, su queste fonti trovi dettagli operativi (diagrammi di flusso, metriche di progetto, interviste ai product manager) che nelle pubblicazioni accademiche non compaiono.

Infine, arriva al **capitolo delle conclusioni**, dove riepiloghi quanto hai scoperto. Qui torna a collegare la tua indagine empirica con i concetti del glossario: spiega perché le scelte di consenso adottate in un caso A hanno avuto esiti migliori che in un caso B, o perché un certo linguaggio ha rallentato lo sviluppo. Chiudi suggerendo possibili vie future: quali domande restano aperte, quali gap tecnologici o culturali andrebbero colmati per far decollare davvero la certificazione blockchain in agrifood.

In breve, procedi così: esplora un progetto, annota ogni parola o tecnica che non hai ancora definito, riversala nel capitolo “concetti principali”, quindi torna ai casi concreti con gli strumenti teorici appena acquisiti. Alla fine, il lettore ti seguirà in un percorso logico che va dall’esperienza sul campo ai fondamenti tecnici, passando per analisi critica dei successi e dei fallimenti.

## Struttura della tesi - discussa col professore

1. **Introduzione:** nell'introduzione si limiti a riassumere brevemente il contenuto della tesi, e come ha effettuato la ricerca (motori, parole chiave/prompt , criteri di selezione e valutazione delle fonti)
    
2. **Capitolo 1 – Concetti principali e stato dell'arte:** In questo capitolo inizia a spiegare nomi e concetti tecnici, partendo dalle definizioni di Agrifood e di Blockchain.
   Dopodiché prosegui spiegando come viene implementata oggi, in quali ambiti viene utilizzata e da chi.
   Infine, aggiungi una sezione dedicata a tecnologie e linguaggi di programmazione in cui descrivi sia i linguaggi maggiormente utilizzati che le varie tipologie di consenso
    
3. **Capitolo 2 – Progetti:** analizzo un paio di aziende che implementano con successo tale tecnologia (es.: Walmart, nota catena di supermercati americana) e cerco un fattore comune tra di essi. Esempi di fallimenti, cercando un fattore comune tra di essi
    
4. **Capitolo 3 - Conclusioni  e prospettive future**
   
5. **Bibliografia e materiale grigio utilizzato** 