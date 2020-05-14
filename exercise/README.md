# Esercitazione UML/SRS
Le sezioni seguenti tratteggiano il campo di applicazione e le macro funzionalità di alcuni prodotti software. Per ogni software, è possibile allenare le proprie capacità di progettazione sviluppando un documento SRS (vedi Appendice 1), oppure diagrammi UML (casi d'uno e classi in tutti i casi; attività e stati dove possibile).

## Centro di Assistenza
L’applicazione da sviluppare deve supportare un centro di assistenza. I clienti possono chiamare il centro di assistenza per segnalare un guasto, specificando l’apparecchiatura, il tipo di guasto, l’indirizzo, se l’apparecchiatura è in garanzia e ogni altra informazione che possa essere utile per l’intervento.
Le chiamate vengono gestite automaticamente da un call center che attiva i tecnici. Il primo tecnico libero esegue l’intervento, portando con sé alcuni possibili pezzi di ricambio. Al termine dell’intervento, il tecnico deve rendicontarlo, specificando se il guasto è stato riparato, se necessita di altri pezzi di ricambio, e/o di un ulteriore intervento. Deve inoltre confermare se l’intervento era in garanzia.

## App Store
Il sistema informativo richiesto va installato presso uno store di applicazioni. Gli autori di applicazioni possono sottomettere applicazioni, visualizzare lo stato della pratica (sottomessa, approvata, online), e controllare il numero dei download ed i profitti derivanti dalle vendite. Ogni mese, il sistema elabora un documento a fini fiscali e lo invia agli autori parallelamente all’eventuale bonifico. Gli utenti dello store possono visualizzare le applicazioni, scaricarle e fornire un rating.

## Caveau
Il sistema informativo richiesto va installato presso un caveau dedicato a metalli preziosi. I clienti del caveau possono visualizzare un catalogo di prodotti acquistabili (barre, lingotti e monete), visualizzare i prodotti di loro proprietà in custodia presso il caveau, e autorizzare la vendita di prodotti. Il caso di vendita, il sistema provvede ad inviare istruzioni all’ufficio incaricato delle liquidazioni. Inoltre il sistema è collegato digitalmente ai sistemi di aziende produttrici di lingotti ed in base alle fluttuazioni del prezzo suggerisce al manager del caveau quando modificare il prezzo dei prodotti.

## Officina
Il sistema deve gestire gli operai, i ponteggi, le auto da riparare, i pezzi di ricambio, ed i clienti. Prima di avviare i lavori i clienti sottoscrivono un contratto di riparazione con l’officina. Una riparazione si svolge in una specifica fascia oraria, su uno specifico ponteggio, da 1 o 2 operai. Ogni riparazione può richiedere più pezzi di ricambio (annotare prezzo e fornitore) di cui è necessario tenere traccia per il magazzino. Al termine della lavorazione il sistema genera una fattura digitale con i dati della riparazione e dell’anagrafica del cliente.

## Linea produttiva Muffin
Il sistema informativo gestisce la produzione di muffin in un impianto robotizzato. In particolare, gli utenti possono acquistare muffin personalizzati attraverso un’interfaccia web. Una volta ricevuto l’ordine, i muffin vengono infornati. Dopo la cottura, un robot si occupa della guarnizione (presa da un gruppo di tipologie predefinito). I muffin guarniti vengono infine posizionati all’interno di scatole da 4 o da 8 posti (in base alla scelta dell’utente) e spediti attraverso il corriere più economico disponibile nell’area di consegna.

## Gestione tirocini
Le aziende interessate producono delle offerte di tirocinio. Il responsabile dei tirocini approva o rifiuta le offerte. I rifiuti sono notificati all’azienda proponente.

Le offerte accettate diventano visibili agli studenti. Gli studenti visualizzano le offerte. In conseguenza di ciò possono accordarsi con l’azienda proponente. Le aziende assegnano gli studenti graditi ai tirocini offerti. Il responsabile dei tirocini approva o rifiuta gli accoppiamenti studente-tirocinio. In caso di accettazione si stampa l’accordo che dovrà essere firmato da tutte le parti in causa.

Considerati i requisiti precedenti, un tirocinio può modificare il proprio stato interno fra: proposto, accettato, accoppiato, in svolgimento, valutato e interrotto. Un’interruzione può verificarsi solo durante l’effettivo svolgimento e rappresenta un processo reversibile. In ogni stato, tratto quello valutato, il tirocinio può essere abbandonato.

## Impresa edile
Il sistema deve gestire gli operai, i cantieri, il parco mezzi e i clienti. Ad ogni cantiere è assegnata una squadra di almeno due operai ed eventuali mezzi.

I clienti sottoscrivono un contratto che definisce le opera da svolgere in cantiere. Prima di avviare i lavori, entrambe le parti devono firmare la versione definitiva del contratto.

Ogni opera svolta in cantiere, va tracciata separatamente annotando l’operaio responsabile. Al termine dei lavori viene emesso un pagamento che contiene voci separate per ogni lavorazione.

Un contratto può modificare il proprio stato interno fra: proposto, accettato, in svolgimento, in attesa di materiali, pagato e interrotto per motivi esterni all’azienda. I cantieri interrotti da più di 2 anni vengono abbandonati. Un’interruzione può verificarsi solo durante l’effettivo svolgimento e rappresenta un processo reversibile.

## Azienda di distribuzione
Il sistema informativo supporta la logistica di una grande società di distribuzione. L’azienda è organizzata su tre livelli operativi:

* l’ufficio acquisti centralizzato
* alcune piattaforme logistiche
* la rete dei negozi

La gerarchia di distribuzione opera in modo bidirezionale: i negozi inviano le proprie richieste all’ufficio acquisti attraverso le piattaforme logistiche.

L’ufficio acquisti riceve le richieste di rifornimento da parte delle piattaforme e le aggrega in modo da ottenere prezzi più bassi presso i fornitori (i.e., economia di scala).

Viceversa, le merci ricevute dall’ufficio acquisti, sono consegnate ai negozi attraverso le suddette piattaforme. Per tutte le strutture dell’azienda, indipendentemente dal loro livello operativo, è necessario specificare un codice univoco, un indirizzo e un numero di telefono.

Ogni negozio tiene sotto controllo le scorte dei propri prodotti. Quando le scorte scendono sotto una soglia predefinita, il negozio emette un ordine che può specificare diversi prodotti (presi da un elenco predefinito, e associati a una categoria merceologica), associati a diverse quantità.

E’ necessario anche tenere traccia della piattaforma che prenderà in carico l’ordine. Ogni ordine, identificato da un codice e dalla data di emissione, tiene traccia anche della data di evasione. Ciascuna piattaforma logistica ha il compito di rifornire il sottoinsieme dei negozi che si trovano nella stessa area geografica. La piattaforma immagazzina i prodotti che gestisce e organizza di conseguenza il giro delle consegne associando autisti e veicoli in base ad un sistema di turni.

L’ufficio acquisti, infine, genera ordini aggregati da inviare a diversi fornitori. Come nel caso di un ordine semplice, un ordine aggregato specifica diversi prodotti in diverse quantità. E’ necessario tenere traccia di quali ordini semplici (dei negozi) confluiscono (anche solo parzialmente) in un ordine aggregato.

L’ufficio acquisti tiene traccia di tutti i fornitori ai quali si è rivolta specificando, per ognuno di essi, una serie di dati anagrafici. Inoltre, per ogni fornitore, l’azienda registra le categorie merceologiche (prese da un elenco predefinito) di sua competenza. In caso un fornitore cambi le proprie categorie, i cambiamenti vanno opportunamente storicizzati.

## Car sharing
Il sistema informativo supporta una piafforma web di mobility-sharing peer-to-peer. Il principio su cui si basa il servizio consiste nel consentire ad ogni utente la possibilità di:

* guadagnare rendendo un proprio veicolo disponibile ad essere utilizzato da altri utenti
* utilizzare il veicolo di un altro utente pagando una quota di noleggio.

Ogni utente è descritto da un insieme di dati anagrafici (nome, cognome, data e luogo di nascita, codice fiscale...) oltre che da una categoria (presa da un elenco predefinito) che ne esprime il livello di affidabilità.

Ogni utente può decidere di rendere disponibili fino a tre veicoli (ciascuno identificato da marca, modello, colore, targa e tariffa di noleggio oraria). Le tipologie di veicoli gestite dal sistema sono ciclomotori, automobili e furgoni. Per ogni veicolo, ed ogni qualvolta lo desideri, l’utente inserisce le finestre temporali in cui il veicolo è disponibile per il noleggio specificandone la data e l’ora di inizio e fine e le coordinate GPS del veicolo parcheggiato.

Un utente interessato al noleggio può scegliere, in base alla disponibilità, alla posizione o alla tariffa, quale veicolo utilizzare. L’utente può inoltre utilizzare il veicolo per un periodo più breve rispetto alla finestra di disponibilità. Per esempio, può utilizzare per un solo giorno un’auto disponibile per un’intera settimana. Il sistema tiene traccia, per ogni finestra di disponibilità, da quali utenti e per quanto tempo il veicolo è stato utilizzato.

Per motivi di sicurezza automobili e veicoli commerciali sono dotati di un ricevitore GPS il quale invia, in modo incrementale, la traccia GPS seguita dal veicolo. Il sistema memorizza l’intero percorso.

Al termine di ogni utilizzo, ogni utente inserisce eventuali sinistri avvenuti durante il noleggio indicando il numero di pratica della compagnia assicurativa. Per ogni noleggio, il sistema consente inoltre la possibilità di lasciare un giudizio (preso da un elenco predefinito) sulla qualità dell’auto che è stata noleggiata.

Il sistema infine memorizza a fini fiscali tutti i profitti degli utenti che condividono i loro veicoli.

## Progetti di ricerca
Sistema informativo per la documentazione dei progetti di ricerca ai quali partecipano i ricercatori di questa università.

Ogni progetto è caratterizzato da un insieme di dati descrittivi (acronimo, titolo, logo, data d’inizio, durata in mesi, budget, eccetera). Inoltre il progetto è caratterizzato dal nome del programma di ricerca di appartenenza, preso da un elenco pre-definito.

Ad ogni progetto partecipano ricercatori di questa università ed eventualmente di altri atenei. Di ogni ricercatore sono noti i dati anagrafici, il telefono e l’indirizzo eMail, la data a partire dalla quale ha iniziato a lavorare al progetto e l’eventuale data in cui ha lasciato il progetto. Se il ricercatore è di questa università è indicato anche il dipartimento di appartenenza. Un ricercatore può partecipare nello stesso momento a più progetti di ricerca.

Il progetto descrive i propri risultati attraverso la pubblicazione di documenti. Ogni documento ha un suo identificatore unico, un titolo, un tipo (preso da un elenco predefinito), una data di pubblicazione e l’insieme dei ricercatori che l’hanno prodotto (uno o più). Di ognuno dei ricercatori di questa università è calcolato il numero di pubblicazioni di è autore o co-autore per ciascuno dei progetti ai quali partecipa.

Taluni dei documenti sono pubblicati su riviste internazionali. Il sistema deve registrare le riviste su cui pubblicare (nome della rivista, editore, settore) e associarvi tali documenti indicando i nomi dei revisori (almeno tre) che hanno approvato la pubblicazione.

Per la partecipazione a un progetto a ogni ricercatore di questa università è assegnato un budget con cui coprire le spese (apparecchiature, viaggi, eccetera). Nel corso dello svolgimento del progetto occorre registrare tutte le spese effettuate da ciascun ricercatore con indicazione, per ogni spesa, della data, della cifra e della motivazione.

## Rete autostradale
La rete autostradale è suddivisa in un certo numero di tratte ognuna delle quali è rappresentata da un codice, una descrizione, i suoi due punti estremi, il numero di corsie e la lunghezza in chilometri. Ciascun punto estremo è caratterizzato da una sigla, una descrizione e una coppia di coordinate geografiche (LAT, LON).

Del manufatto occorre indicare la tipologia (es. ponte, viadotto, galleria, passaggio, area di sosta) presa da una lista pre-esistente e registrare l’identificatore, la tratta autostradale di appartenenza, varie informazioni descrittive, la posizione geografica, lo stato, l’anno di costruzione (solo se è già completato). Il manufatto è anche corredato di fotografie.

I manufatti autostradali sono soggetti a sopralluoghi periodici. Il singolo sopralluogo è affidato per l’esecuzione ad una delle ditte accreditate presso la società di gestione. La ditta incaricata organizza allo scopo una squadra di tre persone, una delle quali nel ruolo di responsabile e le altre due in quello di operatori.

Le ditte accreditate sono adeguatamente identificate e corredate di dati descrittivi, e le persone cui affidano i sopralluoghi sono a loro volta registrate nel sistema con i tipici dati anagrafici e con la qualifica (responsabile, operatore). In definitiva, è necessario sapere quale ditta, con quali persone, e naturalmente in quale data, esegue ciascun sopralluogo sul singolo manufatto.

Il risultato del sopralluogo è una relazione nella quale sono elencati gli eventuali problemi riscontrati. Di un problema si indica la tipologia (presa da un elenco dato), una descrizione e una misura di gravità compresa fra 1 e 10. La relazione viene presa in carico da uno dei dipendenti della società di gestione, codificato con i soliti dati anagrafici.

Ciascun problema può generare un ordine di intervento. L’ordine presenta una data di emissione, le date entro cui deve essere eseguito, le possibili ditte fra cui scegliere quella da incaricare, la descrizione dell’intervento da effettuare. Per ognuna delle ditte candidate è riportata la stima preventiva dei costi dell’intervento.

Il manufatto è caratterizzato da uno stato che può prendere i valori: progettato, in costruzione, esistente, a rischio, abbandonato, ripristinato.

## Assicurazione
L'assicurazione può assicurare sia persone fisiche sia società, delle une e delle altre serve conoscere i dati anagrafici.

Ad ogni assicurato è attribuito un numero di codice e un giudizio di affidabilità preso da un elenco predefinito.

Ogni assicurato può stipulare una polizza per la copertura di uno o più tipi di rischio, presi da un elenco predefinito.

Il costo della polizza, o premio complessivo, può essere pagato in un’unica soluzione o in rate mensili. Sta all’assicurato scegliere fra queste due possibilità, il sistema informativo prende atto della scelta e registra i pagamenti man mano che avvengono con ammontare e data.

Ogni volta che accade un sinistro che riguarda un assicurato occorre registrarne tutti i dati descrittivi, compreso l’ammontare del danno, ed eventualmente le foto di corredo. Il sistema informativo deve poi associare il sinistro a uno dei tipi di rischio.

Gli stati attraverso cui passa il giudizio di affidabilità sono i seguenti: nuovo, fedele, ottimo, lento, costoso.

## Azienda di motocicli
L’azienda produce diversi tipi di motociclo, ciascuno descritto da codice, nome, descrizione e cilindrata. Per partecipare alle gare l’azienda utilizza alcuni precisi motocicli dei vari tipi, ciascuno caratterizzato dalla targa e dalla livrea scelta da un elenco predefinito.

Ciascun tipo di motociclo è costruito utilizzando componenti, di ogni componente occorre registrare la quantità consumata (es. 12 bulloni B047). I componenti possono essere prodotti internamente o acquistati, nel secondo caso occorre conoscere il fornitore.

Ogni membro del personale è caratterizzato da nome, cognome, età e numero di matricola. Il personale si divide in tre categorie, vale a dire: piloti, meccanici e progettisti, e nessuno fa parte di più categorie contemporaneamente.

Ogni meccanico, di cui è indicata la specializzazione, è assegnato a uno e un solo pilota, che a sua volta può avere assegnati fino a tre meccanici di cui almeno uno “motorista”. Ogni progettista ha un titolo di studio e può aver progettato uno o più tipi di motociclo.

Ogni gara è caratterizzata da denominazione, anno e autodromo abilitato dove si svolge. Non viene disputata sempre necessariamente nello stesso autodromo e può essere disputata più volte in anni diversi, ma al massimo una volta sola nello stesso anno. A ciascuna gara possono partecipare più piloti dell’azienda e ciascuno guida uno dei motocicli della stessa azienda. Per ogni partecipazione a una gara deve essere memorizzata la posizione iniziale del pilota, il suo ordine d’arrivo ed eventuali problemi riscontrati durante la gara. La partecipazione di un pilota a una gara è ulteriormente documentata da un insieme di dati costituiti da articoli, interviste e fotografie.
 
# Appendice 1 - IEEE830 SRS
1. Introduzione
  1. Obiettivo
  1. Campo d’applicazione
  1. Definizioni, acronimi e abbreviazioni
  1. Fonti
  1. Struttura del documento SRS
2. Descrizione generale
  1. Inquadramento
  1. Macro funzionalità
  1. Caratteristiche degli utenti
  1. Vincoli generali
  1. Ipotesi di partenza, assunzioni e dipendenze
  1. Requisiti da analizzare in futuro
3. Specifica dei requisiti
  1. Requisiti dell’interfaccia esterna
  1. Requisiti funzionali
  1. Requisiti non funzionali

Caratteristiche SRS

* Corretto
* Non ambiguo
* Completo
* Consistente
* Ordinato per priorità dei requisiti
* Verificabile
* Modificabile
* Tracciabile
