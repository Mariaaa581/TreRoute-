<br><br>
<img src="immagini/LogoViavai.png" width="200px" align="left" style="margin-right:60px">

<p align="center" style="margin:20px">Documentazione del progetto Viavai, un'applicazione web di carpooling per gli spostamenti quotidiani brevi, che mette in contatto passeggeri e conducenti che fanno la stessa strada ogni giorno, per dividere le spese del viaggio.</p>

Sviluppato da:

- Meriame Benantar, 1087369
- Zineb Machal, 1100565
- Zineb Chakraoui, 1086381

<br clear="left">

Corso di Ingegneria del Software, A.A. 2026/2027, Università degli Studi di Bergamo.<br>
Docente: prof. Angelo Gargantini. Esercitatrice: Silvia Bonfanti.

Storico delle versioni:

| Versione | Modifiche |
|---|---|
| 0.1 | Struttura del documento con i capitoli |

# INDICE
0. [Definizioni e abbreviazioni](#definizioni-e-abbreviazioni)
1. [Introduzione](#1-introduzione)
2. [Gestione del progetto](#2-gestione-del-progetto)
3. [Requisiti](#3-requisiti)
4. [Design](#4-design)
5. [Testing](#5-testing)
6. [Manutenzione](#6-manutenzione)


## Definizioni e abbreviazioni

| Termine | Significato |
|---|---|
| Passaggio | *Da completare* |
| Prenotazione | *Da completare* |
| Zona | *Da completare* |

| Abbreviazione | Significato |
|---|---|
| FUN | Requisito funzionale |
| GUI | Requisito dell'interfaccia grafica |
| MDA | Model Driven Architecture |


## 1. Introduzione
#### 1.1 Viavai
*Da completare.*

#### 1.2 Struttura del documento
*Da completare.*


## 2. Gestione del progetto
#### 2.1 Ciclo di vita del software
*Da completare.*

#### 2.2 Configuration management
*Da completare.*

#### 2.3 Organizzazione del team
*Da completare.*


## 3. Requisiti
#### 3.1 Raccolta dei requisiti
*Da completare.*

#### 3.2 Requisiti funzionali

##### 3.2.1 Registrazione e accesso

| ID | Requisito / Motivazione | Dipende da |
|---|---|---|
| FUN.1 | Il visitatore deve poter registrarsi inserendo nome, cognome, email e password. L'email non può essere già usata da un altro utente.<br>*Motivazione:* per offrire o prenotare un passaggio serve un account personale, e l'email permette di riconoscere l'utente. | – |
| FUN.2 | Durante la registrazione l'utente deve scegliere il proprio ruolo: conducente o passeggero. Un utente ha un solo ruolo.<br>*Motivazione:* il ruolo decide cosa può fare: il conducente pubblica i passaggi, il passeggero li prenota. | FUN.1 |
| FUN.3 | L'utente registrato deve poter accedere con email e password.<br>*Motivazione:* proteggere i dati e le prenotazioni di ogni utente. | FUN.1 |
| FUN.4 | Il conducente deve registrare almeno un veicolo indicando modello, targa e numero di posti.<br>*Motivazione:* il numero di posti limita i passaggi che può pubblicare e le prenotazioni che può accettare. | FUN.2 |

##### 3.2.2 Passaggi e prezzo

| FUN.5 | Il conducente deve poter pubblicare un passaggio ricorrente indicando zona di partenza, zona di arrivo, orario, almeno un giorno della settimana, numero di posti liberi e prezzo. Può aggiungere facoltativamente punto d'incontro, note, pedaggi e bagagli.<br>*Motivazione:* i pendolari fanno lo stesso tragitto ogni giorno, quindi il passaggio si pubblica una volta sola per tutti i giorni scelti. | FUN.4 |
| FUN.6 | Il sistema deve calcolare il prezzo massimo per persona e per viaggio come distanza in km tra le due zone × 0,20 € ÷ numero di persone in auto (posti liberi più il conducente), arrotondato per difetto al centesimo.<br>*Esempio:* da Seriate a Dalmine (14 km) con 3 passeggeri il massimo è (14 × 0,20) ÷ 4 = 0,70 €.<br>*Motivazione:* Viavai deve restare una condivisione delle spese e non un servizio a pagamento. Il valore di 0,20 € al km è vicino al più basso delle tabelle ACI per un'auto piccola. | FUN.5 |
| FUN.7 | Il sistema non deve permettere di pubblicare un passaggio con un prezzo superiore al prezzo massimo e deve mostrare il limite al conducente. Un prezzo uguale al massimo è accettato.<br>*Motivazione:* è una richiesta del committente: il conducente non deve guadagnare dal passaggio. | FUN.6 |
| FUN.8 | Il numero di posti liberi di un passaggio deve essere almeno 1 e non può superare i posti del veicolo meno uno. Per esempio, con un'auto da 5 posti se ne possono offrire al massimo 4.<br>*Motivazione:* il conducente occupa un posto, e un passaggio senza posti liberi non serve a nessuno. | FUN.4, FUN.5 |

##### 3.2.3 Prenotazioni e notifiche

| ID | Requisito / Motivazione | Dipende da |
|---|---|---|
| FUN.9 | *Da completare* | |

#### 3.3 Requisiti dell'interfaccia

| ID | Requisito / Motivazione | Dipende da |
|---|---|---|
| GUI.1 | *Da completare* | |

#### 3.4 Requisiti non funzionali
*Da completare.*

#### 3.5 Qualità del software
*Da completare.*


## 4. Design
#### 4.1 Diagrammi UML
*Da completare.*

#### 4.2 Architettura del software
*Da completare.*

#### 4.3 Design del software e design pattern
*Da completare.*


## 5. Testing
#### 5.1 Casi di test
*Da completare.*

#### 5.2 Copertura dei test
*Da completare.*


## 6. Manutenzione
#### 6.1 Refactoring
*Da completare.*

---

*Versione 0.1*
