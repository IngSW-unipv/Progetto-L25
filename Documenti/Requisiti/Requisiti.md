# 1. Introduzione

## 1.1 Scopo del documento

Questo documento ha lo scopo di descrivere le funzionalità offerte dal nostro programma insieme ai requisiti da rispettare per un funzionamento corretto del prodotto.

## 1.2 Scopo del prodotto 

OptoManage serve per gestire in modo veloce ed efficiente i prodotti
presenti all’interno del magazzino di un negozio di ottica,
permettendo all’utente che lo utilizza di gestire gli ordini dei
fornitori e dei clienti, dando così una visione totale e una riduzione
dei tempi di gestione e ordine.

Gli ordini potranno essere effettuati direttamente dal software
anche su richiesta del cliente, fornendo i suoi dati anagrafici
e la prescrizione oculistica precedentemente ricevuta dal medico
oculista.

I clienti invece attraverso il software potranno vedere i dati
descritti in precedenza oltre che lo stato dei loro ordini.

### 1.2.1 Nome
OptoManage

### 1.2.2 Scopo
Gestione negozio ottica di ordini, vendite,
dati clienti.

### 1.2.3 Vantaggi
Questo programma ha il vantaggio di poter effettuare gli
ordini direttamente dal software, di rendere più veloce
l’accesso ai dati dei clienti, di facilitare la gestione
del magazzino e di rendere trasparente lo stato degli
ordini ai clienti.


## 1.3 Definizioni, acronimi e abbreviazioni

- *Diottrie*: La diottria è un’unità di misura che indica il potere
refrattivo di una lente o di un sistema ottico, ovvero la capacità
di intercettare e deviare i raggi luminosi provenienti da un oggetto
in modo da mettere a fuoco un’immagine nitida. 

- *Busta*: Quando viene ordinato l'occhiale viene creata
una busta, questa contiene una serie di informazioni, quali:
  - Dati del Cliente
  - Prescrizioni ottiche
  - Note del cliente

- *Montatura*: Struttura in cui vengono inserite le lenti
oftalmiche. (Occhiale senza lenti)

- *Lenti oftalmiche*: Lenti che vengono montate sulla
montatura

- *Prescrizione ottica*: L'insieme delle misurazioni effettuate
dall’ottico o dall’oculista per determinare la correzione visiva
necessaria al cliente. Comprende parametri come sfera (SPH),
cilindro (CYL), asse (AXIS), addizione (ADD) e distanza
interpupillare (PD).

## 1.4 Riferimenti

## 1.5 Overview
  Nel resto del documento parleremo del funzionamento del
  nostro programma, i requisiti che dovrà rispettare per
  fornire le funzionalità previste.

<br>
<br>

***

# 2. Descrizione generale 

## 2.1 Prospettiva del prodotto

  Il software è progettato per funzionare autonomamente con il
  suo DBMS.

## 2.2 Funzioni del prodotto

Il software offre una serie di funzionalità atte a semplificare
l'amministrazione del punto vendita tramite una visione completa
del magazzino e degli ordini da parte dei clienti e verso i fornitori,
inoltre punta a migliorare l’esperienza del cliente fornendogli un
portale dove trovare tutte le informazioni utili.


### 2.2.1 Funzionalita' in generale

I *lavoratori* possono:
- Gestire Clienti
- Gestire Ordini
- Gestire Magazzino
- Fare ordini
- Aggiungere/togliere clienti 
- Aggiungere/togliere prodotti
- Fare scontrini (vendita finale)

I *clienti* possono:
- Ordinare lenti a contatto già ordinate
- Visualizzare stato e storico ordini 
- Visualizza punti della card

I *fornitori* possono:
- Fornire prodotti (attraverso gli ordini)
- Richiedere resi (dei prodotti non venduti)

## 2.3 Caratteristiche utente
L’utente dev’essere un ottico o un dipendente che conosce
il linguaggio tecnico dell’ottica. E avere conoscenze base
nell’uso di computer.

## 2.4 Presupposti e dipendenze
- Windows
- Java
- MySQL

<br>
<br>

***

# 3. Requisiti specifici

## 3.1 Interfacce esterne
- Tastiera
- Mouse 
- Schermo
- Connessione internet

## 3.2 Requisiti funzionali

- **RF1**: Creazione profilo utente
- **RF2**: Creazione ordine
- **RF3**: Gestione magazzino
  - **RF3.1**: Aggiunta/Rimozione prodotti
  - **RF3.2**: Visualizzazione stato magazzino
- **RF4**: Creazione fatture
- **RF5**: Sistema punti fedeltà
 

## 3.3 Requisiti non funzionali
		
- **RNF1**: Prestazioni

		Il sistema deve essere in grado di gestire almeno 1000 ordini
		simultanei senza degrado delle prestazioni.

		Il tempo di risposta per il caricamento dei dati cliente deve
		essere inferiore a 2 secondi.

		Il software deve elaborare un ordine in meno di 3 secondi.

- **RNF2**: Portabilità e Compatibilità

		Il software è sviluppato con Java SE 23.
		Il software deve essere compatibile con Windows 10, 11.
		Il database deve supportare MySQL 8.0.

- **RNF3**: Scalabilità

		Deve poter gestire contemporaneamente almeno 50 utenti senza perdita di performance.

## 3.4 Tipi di utente

-Capo azienda
-Dipendente
-Clienti
-Fornitori

<br>
<br>

***

# 4 Indice

- 1 **Introduzione**

  - 1.1 Scopo del documento
  - 1.2 Scopo del prodotto
    - 1.2.1 Nome del prodotto
    - 1.2.2 Cosa fa il prodotto
    - 1.2.3 Vantaggi, obiettivi

  - 1.3 Definizioni, acronimi, abbreviazioni

  - 1.4 Riferimenti

  - 1.5 Overview

- 2 **Descrizione generale**

  - 2.1 Prospettiva del prodotto
  - 2.2 Funzioni del prodotto
    - 2.2.1 Funzionalita' in generale
  - 2.3 Caratteristiche utente
  - 2.3 Presupposti e dipendenze

- 3 **Requisiti specifici**

  - 3.1 Interfacce esterne
  - 3.2 Requisiti funzionali
  - 3.3 Requisiti non funzionali
  - 3.4 Tipi di utente

- 4 **Indice**







				


