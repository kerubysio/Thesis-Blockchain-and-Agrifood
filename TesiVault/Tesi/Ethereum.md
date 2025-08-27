# Introduzione

## Blockchain

Con il termine blockchain si intende un database che viene aggiornato e condiviso tra più computer su una rete.
Questo database è formato da una serie di blocchi in cui ognuno è collegato a quello precedente. I blocchi non sono altro che dei pacchetti di dati che contengono delle informazioni più un riferimento al blocco precedente. Tale riferimento è un hash crittografico, ossia un indirizzo che si ottiene passando alcuni parametri relativi al blocco precedente ad una funzione di hash (ossia una funzione che riceve in ingresso dei dati e li trasforma in un'unica stringa di lunghezza fissa e praticamente mai genera stringhe ripetute).
I dati in un blocco non possono essere modificati senza modificarne anche l'hash, alterando quindi tutto il resto della catena di blocchi.
Ogni computer nella rete deve essere d'accordo per l'aggiunta di un nuovo blocco e deve concordare sullo stato complessivo della blockchain. Affinché questa cosa sia possibile è necessario affidarsi ad un meccanismo di consenso (consensus mechanism).

## Proof of Stake

Ethereum usa il Proof of Stake (PoS), come meccanismo di consenso: chiunque voglia aggiungere un nuovo blocco deve mettere in stake (ossia bloccare come garanzia) degli ETH ed eseguire un software da validator (l'equivalente dei miner nel [[Consensus mechanism|PoW]]).
In questo modo, se ti comporti bene vieni ricompensato con nuovi ETH, mentre se ti comporti male ne parti una parte o addirittura tutti. Per scegliere quale validator potrà aggiungere nuovi blocchi si procede in questo modo: un validator scelto a caso propone uno o più blocchi da aggiungere alla rete, dopodiché gli altri validator controllano il suo operato e verificano che non ci siano incongruenze o tentativi di hacking.
Alla fine di questo controllo ogni validator vota si o no. Se la maggior parte dei voti è favorevole allora i blocchi vengono aggiunti.
Qualcuno di malintenzionato dovrebbe avere quindi il controllo sul 51% della rete, così da poter proporre e accettare blocchi malevoli. Tuttavia per farlo dovrebbe mettere in stake una quantità di ETH molto alta, che sarebbe probabilmente superiore al guadagno che trarrebbe da un'azione de genere.
Il minimo da mettere in stake è 32 ETH, anche se puoi partecipare a delle validator pool con meno ETH. Volendo è anche possibile mettere in stake più di 32 ETH, ma questo non aumenta e tue possibilità di essere scelto. Per ogni 32 ETH che metti in stake, la rete ethereum genera un account validator che ha le stesse chance di essere selezionato rispetto agli altri.
Questo perché se un validatore potesse mettere 10.000 ETH in un unico nodo, basterebbero poche persone ricchissime per controllare gran parte della rete. Limitando a 32 ETH per validatore, chi ha tanti ETH deve comunque far girare molti nodi diversi → più decentralizzazione.
Inoltre, se un validatore con tantissimi ETH fa un errore (es. rimane offline o viene hackerato), senza il limite potrebbe perdere o bloccare una fetta enorme della rete. Con blocchi da 32 ETH il rischio è distribuito (no single point of failure).

## Nodo 
Per nodo si intende ogni computer che partecipa alla rete Ethereum in tre modi:
* Tiene una copia aggiornata della blockchain
* Verifica e propaga nuove transazioni
* Se è un validator, propone e approva nuovi blocchi

# Che cos'è Ethereum?

Ethereum è una blockchain con un computer integrato che viene utilizzato per costruire applicazioni e organizzazioni in maniera del tutto decentralizzata e resistente alla censura.
Al centro di Ethereum c'è quindi un singolo computer virtuale che prende il nome di Ethereum Virtual Machine (EVM). Ogni nodo sulla rete ethereum deve essere d'accordo sullo stato di questo computer.
Non è un oggetto fisico, ma uno **strato software** che funziona in modo identico su tutti i nodi.

Le sue funzioni sono:
* **Eseguire smart contract**, cioè programmi caricati dagli utenti sulla blockchain.
    
- Mantenere in memoria lo **stato globale della rete**, ossia: saldi degli account, smart contracts esistenti e i loro dati e il registro delle transazioni eseguite fino a quel momento.

Tutti i nodi devono avere lo **stesso stato dell’EVM**, così la rete mantiene coerenza, sicurezza e immutabilità delle informazioni.
In pratica, l’EVM garantisce che ogni calcolo o transazione abbia **lo stesso risultato in tutta la rete**, indipendentemente dal nodo che la esegue.
Ogni membro della rete può chiedere all'EVM di eseguire degli smart contracts o eseguire determinate azioni (queste richieste prendono il nome di transazioni), ogni volta che questo accade, tutti gli altri nodi verificano, validano ed eseguono la richiesta.
Questo processo causa una modifica dello stato dell'EVM, che viene eseguito e propagato sull'intera rete.

## Ether (ETH)

**Ether (ETH)** è la criptovaluta nativa di Ethereum. Lo scopo di ETH è consentire un mercato per il calcolo. Un mercato di questo tipo fornisce un incentivo economico affinché i partecipanti verifichino ed eseguano le richieste di transazione e forniscano risorse di calcolo alla rete.

Ogni partecipante che trasmette una richiesta di transazione deve anche offrire un certo importo di ETH alla rete a titolo di ricompensa. La rete brucerà parte della ricompensa, elargendo il resto a chiunque alla fine svolgerà il lavoro di validator.

L'importo di ETH pagato corrisponde alle risorse necessarie a eseguire il calcolo. Queste ricompense impediscono ai partecipanti malevoli di intasare intenzionalmente la rete, richiedendo l'esecuzione di calcoli infiniti o di altri script ad alta intensità di risorse, poiché tali partecipanti devono pagare per le risorse di calcolo.

L'ETH è inoltre usato per fornire sicurezza cripto-economica alla rete in tre modi principali: 1) è usato come un mezzo per ricompensare i validatori che propongono i blocchi o segnalano i comportamenti disonesti degli altri validatori 2) è messo in staking dai validatori, fungendo da garanzia contro i comportamenti disonesti: se i validatori tentano di comportarsi in modo malevolo, i loro ETH possono esser distrutti 3) è usato per ponderare i 'voti' per i blocchi appena proposti, alimentando la parte di scelta della diramazione del meccanismo di consenso.

## Smart contracts

Quando qualcuno vuole richiedere all'EVM di svolgere dei calcoli, non è sempre necessario che scriva del codice. Spesso infatti è possibile utilizzare codice scritto da altri sviluppatori sotto forma di applicazioni chiamate smart contracts (o contratti intelligenti).

Un contratto intelligente è uno script che, quando chiamato entro certi parametri, esegue delle azioni o dei calcoli, se certe condizioni sono soddisfatte.

Qualsiasi sviluppatore può creare un contratto intelligente e renderlo pubblico sulla rete, usando la blockchain come database e in cambio di una commissione pagata alla rete. Qualsiasi utente può, quindi, chiamare il contratto intelligente a eseguire il proprio codice, anche in questo caso sarà necessario pagare una piccola commissione alla rete.

Dunque, con i contratti intelligenti, gli sviluppatori possono creare e distribuire arbitrariamente app e servizi rivolti agli utenti, come: mercati, strumenti finanziari, giochi, etc.

