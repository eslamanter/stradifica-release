# STRADIFICA  
**Verifica Tracciati Stradali**  
*v2.2 beta*  

---
## 1. Cos'è  
**Stradifica** è un'applicazione desktop per l’esecuzione, l’analisi grafica e l’esportazione in tempo reale delle 
verifiche plano-altimetriche dei tracciati stradali, in conformità alla normativa italiana.  
In sviluppo continuo dal 2022, il progetto nasce con passione come freeware per aiutare la comunità degli ingegneri ad 
automatizzare i flussi di lavoro. Feedback e suggerimenti sono sempre benvenuti.  

---
## 2. Contesto d'uso  
### 2.1 Destinatari  
Categorie di utenti a cui Stradifica è rivolto:  

- **Docenti, ricercatori e studenti**  
  per corsi di ingegneria civile, trasporti e progettazione stradale,
  come supporto didattico e per attività di analisi e sperimentazione  

- **Studi tecnici e professionisti**  
  per validazioni preliminari e attività illustrative
  a supporto della progettazione stradale e infrastrutturale  

### 2.2 Ambiti di applicazione  
- Verifica della conformità normativa degli elementi plano-altimetrici dei tracciati stradali  
- Analisi grafica e confronto dei diagrammi di velocità e di visibilità   
- Studio della fattibilità di varie soluzioni progettuali o degli scenari ipotetici  

---
## 3. Termini d'uso  
### 3.1 Licenza  
Questa versione del software è distribuita come eseguibile `.exe`:  
- **Uso didattico ed educativo:** Libero.  
- **Uso commerciale:** Consentito previa comunicazione all'autore.  

In ogni caso è **obbligatoria** l'attribuzione dei crediti all'autore.  

### 3.2 Comunicazione uso commerciale  
Per comunicare l'uso commerciale, inviare una descrizione del contesto di applicazione a:  
  **[eslam.anter@outlook.com](mailto:eslam.anter@outlook.com)**  

### 3.3 Restrizioni  
- Vietata qualsiasi modifica o decompilazione  

### 3.4 Raccolta dei dati  
Stradifica **non raccoglie, memorizza né trasmette** alcun dato personale:  
- **Nessuna connessione** a server esterni durante il funzionamento, tranne per:  
  1. il controllo dell'ultima versione all'avvio:  
  `https://raw.githubusercontent.com/eslamanter/stradifica-release/main/version.json`  
  2. la visualizzazione della guida:  
  `https://raw.githubusercontent.com/eslamanter/stradifica-release/main/README.md`  
- **Esecuzione anonima** senza registrazione di dati o log utente  
- Le impostazioni scelte dall'utente vengono salvate **localmente** nel percorso:  
  `C:\Users\<User>\AppData\Local\Stradifica\`  

---
## 4. Avvertenze  
### 4.1 Limiti di funzionalità  
Questa applicazione non sostituisce le competenze professionali né il giudizio tecnico qualificato. 
Il software non è stato testato in tutte le situazioni possibili e l'uso in contesti non previsti può generare risultati inattesi. 
Si raccomanda di verificare sempre i risultati e di non utilizzarli come unica base decisionale in ambiti critici.  

### 4.2 Esclusione di responsabilità  
Questo software è fornito senza alcuna garanzia di prestazioni, affidabilità o risultati. 
L’idoneità del codice e l’utilizzo dei risultati da esso ottenuti sono onere e responsabilità esclusiva dell’utente. 
L’autore declina ogni responsabilità per danni diretti o indiretti derivanti dall’uso del software, 
inclusi errori nei dati, interpretazioni errate o decisioni basate sui risultati generati.  

---
## 5. Requisiti  
- **Sistema operativo**: Windows 10, 11  
- **Spazio su disco**: 289 MB  

**Nota**: Al primo avvio potrebbe comparire l'avviso di **Windows Defender SmartScreen**. 
Per autorizzare l'esecuzione, selezionare "**Più informazioni**" e poi "**Esegui comunque**".  

---
## 6. Aggiornamenti  
All'avvio, l'applicazione verifica automaticamente la disponibilità di nuove versioni. 
Se disponibile, verrà mostrato un messaggio con le informazioni sulla versione e il link per il download.  

Scopri il repository di distribuzione su [https://github.com/eslamanter/stradifica-release](https://github.com/eslamanter/stradifica-release).  

---
## 7. Riferimenti normativi  
### 7.1 D.Lgs. 285/1992  
"NUOVO CODICE DELLA STRADA" - 
Decreto Legislativo 30 aprile 1992, n. 285 e successivi aggiornamenti  
[[Visualizza il testo ufficiale](https://www.mit.gov.it/documentazione/codice-della-strada)]  

**Classificazione delle strade: (Art. 2)**  

L'applicazione include le verifiche delle seguenti categorie stradali:  
- **A - Autostrade**  
 (extraurbane e urbane) (principali e di servizio)  
- **B - Strade extraurbane principali**  
 (principali e di servizio)  
- **C - Strade extraurbane secondarie**  
- **D - Strade urbane di scorrimento**  
 (principali e di servizio)  
- **E - Strade urbane di quartiere**  
- **F - Strade locali**  
 (extraurbane e urbane)  

Nel seguito sono elencati i criteri normativi disponibili nell’applicazione.  
I criteri contrassegnati sono attivati di default al primo avvio, 
mentre quelli non selezionati non lo sono, in quanto rappresentano 
verifiche ridondanti su parametri già considerati implicitamente da altri criteri.  

### 7.2 D.M. 6792/2001  
"NORME FUNZIONALI E GEOMETRICHE PER LA COSTRUZIONE DELLE STRADE" - 
Decreto Ministeriale 5 novembre 2001, n. 6792 (G.U. 04/01/2002)  
[[Visualizza il testo ufficiale](https://www.mit.gov.it/normativa/decreto-ministeriale-protocollo-6792-del-05112001)]  

**Criteri di verifica della visibilità: (§5.1)**  

L'applicazione calcola i seguenti diagrammi di visibilità richiesta per entrambi i sensi di marcia ove applicabile.   
- Diagramma di visibilità richiesta per l'arresto (§5.1.2)  
- Diagramma di visibilità richiesta per il sorpasso (§5.1.3)  
- Diagramma di visibilità richiesta per la manovra di cambiamento di corsia (§5.1.4)  

**Criteri di progettazione del tracciato planimetrico: (§5.2)**  

- Calcolo della pendenza trasversale della piattaforma in curve: (§5.2.4)  
- Calcolo dell'allargamento totale della piattaforma in curva: (§5.2.7)  

L'applicazione adotta i seguenti criteri per la verifica dell'andamento planimetrico dell'asse stradale.  

**Rettifilo:**  
  - [x] Lunghezza minima (§5.2.2)  
  - [x] Lunghezza massima (§5.2.2)  
  - [x] Lunghezza massima di flesso (§5.2.5)  


**Clotoide di transizione:**  
  - [x] Parametro A minimo approssimato da limitazione del contraccolpo (§5.2.5)  
  - [ ] Parametro A minimo esatto da limitazione del contraccolpo (§5.2.5)  
  - [x] Parametro A minimo da criterio ottico (§5.2.5)  
  - [ ] Rapporto parametri A minimo da clotoide precedente/successiva (§5.2.5)  
  - [x] Parametro A minimo da clotoide precedente/successiva (§5.2.5)  
  - [x] Parametro A massimo da criterio ottico (§5.2.5)  
  - [ ] Rapporto parametri A massimo da clotoide precedente/successiva (§5.2.5)  
  - [x] Parametro A massimo da clotoide precedente/successiva (§5.2.5)  


**Curva circolare:**  
  - [x] Sviluppo minimo per corretta percezione (§5.2.2)  
  - [x] Differenza massima di velocità da Vpmax (§5.4.4)  
  - [x] Differenza massima di velocità da curva precedente/successiva (§5.4.4)  
  - [ ] Raggio minimo da differenza di velocità da Vpmax (§5.4.4)  
  - [ ] Raggio minimo da differenza di velocità da curva precedente/successiva (§5.4.4)  
  - [x] Raggio minimo da Vpmin (§5.4.4)  
  - [x] Raggio minimo da rettifilo precedente/successivo (§5.2.2)  

**Pendenze trasversali nelle curve a raggio variabile: (§5.2.6)**  

L'applicazione determina l'andamento dei cigli imponendo:  
- Pendenza longitudinale ∆i minima: lungo gli elementi di transizione in corrispondenza del cambio di segno della pendenza trasversale  
- Pendenza longitudinale ∆i massima: in rettifilo, in assenza di elemento di transizione  


**Allargamento della carreggiata in curva: (§5.2.7)**  

L'applicazione calcola il valore totale di allargamento della piattaforma per l'iscrizione dei veicoli in curva, 
per ciascuna curva planimetrica. Tale valore potrà essere opportunamente ridotto fino alla metà qualora si ritenga poco 
probabile l'incrocio in curva di veicoli pesanti quali: autobus, autocarri di grosse dimensioni, autotreni e autoarticolati.  

**Criteri di progettazione del profilo altimetrico: (§5.3)**  

L'applicazione adotta i seguenti criteri per la verifica dell'andamento altimetrico dell'asse stradale.  

**Livelletta:**  
  - [x] Pendenza massima (§5.3.1)  


**Raccordo parabolico:**  
  - [x] Raggio minimo da distanza di visibilità per l'arresto (§5.1.2, §5.3.3, §5.3.4)  
  - [x] Raggio minimo da distanza di visibilità per il sorpasso (§5.1.3, §5.3.3, §5.3.4)  
  - [x] Raggio minimo per evitare contatto con la superficie (§5.3.2)  
  - [x] Raggio minimo da comfort utenza (§5.3.2)  
  - [ ] Accelerazione verticale massima da comfort utenza (§5.3.2)  

**Criteri di costruzione del diagramma delle velocità: (§5.4)**  

L'applicazione calcola i seguenti diagrammi delle velocità.  
- Diagramma delle velocità-prima fase (§5.4.3)  
- Diagramma delle velocità-fase finale (§5.4.3, §5.4.4)  

### 7.3 D.M. 19/04/2006  
"NORME FUNZIONALI E GEOMETRICHE PER LA COSTRUZIONE DELLE INTERSEZIONI STRADALI" - 
Decreto Ministeriale 19 aprile 2006 (G.U. n.170 del 24/07/2006)  
[[Visualizza il testo ufficiale](https://www.mit.gov.it/normativa/decreto-ministeriale-19042006)]  

**Criteri di progettazione delle rampe per le intersezioni a livelli sfalsati: (§4.7)**  

L'applicazione adotta i seguenti criteri aggiuntivi per la verifica dell'andamento plano-altimetrico dell'asse della rampa.  

**Curva circolare:**  
  - [x] Raggio planimetrico minimo (§4.7.2)  


**Livelletta:**  
  - [x] Pendenza massima in salita (§4.7.2)  
  - [x] Pendenza massima in discesa (§4.7.2)  


**Raccordo parabolico:**  
  - [x] Raggio verticale minimo (§4.7.2)  

### 7.4 D.G.R. 27/09/2006 Regione Lombardia  
"Elementi tecnici puntuali inerenti ai criteri per la determinazione delle caratteristiche funzionali e geometriche per la 
costruzione dei nuovi tronchi viari e per l’ammodernamento ed il potenziamento dei tronchi viari esistenti ex art. 4, r.r. 
24 aprile 2006, n. 7" - 
Deliberazione Giunta Regionale 27 settembre 2006 n.8/3219 
(B.U. Regione Lombardia, 1° Suppl. Straordinario al n.44 del 31/10/2006)  
[[Visualizza il testo ufficiale](https://www.provincia.cremona.it/strade/all/20111110-1155350.pdf)]  

- Questo testo è stato utilizzato come riferimento per i parametri cinematici e i coefficienti relativi a 
velocità di progetto superiori a 140 km/h, ove non esplicitamente fornito nel D.M. 05/11/2001  

---
## 8. Interfaccia  
Stradifica offre un'interfaccia grafica semplice e intuitiva, a partire da una **finestra principale** dalla quale è 
possibile accedere a tutti gli strumenti e comandi.  

### 8.1 <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/main.jpg" width="24" height="24"> Finestra principale  
<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/main_window.jpg">  

La finestra principale è composta da una vista centrale, attorno alla quale sono disposte delle barre contenenti i 
comandi per eseguire le diverse funzioni.  
La vista centrale è suddivisa verticalmente in due sezioni (con estensioni modificabili):  
- **Sezione elementi** (in alto): contiene la **tabella degli elementi**  
- **Sezione verifiche** (in basso): contiene la **tabella delle verifiche** (*a sinistra*) e il **registro delle 
verifiche** (*a destra*)  

**Tabella degli elementi**  

La tabella degli elementi contiene le informazioni geometriche del tracciato o del profilo, in base alla vista 
selezionata dalla barra delle viste.

Per la vista del **tracciato**, vengono visualizzati i seguenti parametri:  
- **N.**: Numero  
- **Elemento**: Tipo di elemento geometrico  
- **Prog. iniziale**: Progressiva iniziale [m]  
- **Prog. finale**: Progressiva finale [m]  
- **Lunghezza**: Lunghezza [m]  
- **A**: Parametro A della clotoide [m]  
- **Raggio**: Raggio di curvatura [m]  
- **Direzione**: Direzione di curvatura (oraria/antioraria)  
- **V. 1° fase**: Velocità massima in curva desunta dal diagramma delle velocità della prima fase [km/h]  
- **V. max**: Velocità massima desunta dal diagramma delle velocità della fase finale [km/h]  
- **Flesso**: Rettifilo di flesso verificato (true/false) (D.M. 05/11/2001 §5.2.5)  
- **Sopraelevazione**: Sopraelevazione massima in curva [%] (D.M. 05/11/2001 §5.2.4)  
- **Allargamento**: Allargamento totale della piattaforma per l’iscrizione dei veicoli in curva [m]  

Per la vista del **profilo**, vengono visualizzati i seguenti parametri:  
- **N.**: Numero  
- **Elemento**: Tipo di elemento geometrico  
- **Prog. iniziale**: Progressiva iniziale [m]  
- **Prog. finale**: Progressiva finale [m]  
- **Lunghezza**: Lunghezza [m]  
- **Pendenza**: Pendenza longitudinale [%]  
- **Raggio**: Raggio di curvatura [m]  
- **Profilo**: Andamento altimetrico  
- **V. max**: Velocità massima desunta dal diagramma delle velocità della fase finale [km/h]  

Passando con il cursore sul numero di riga (intestazione verticale), viene visualizzato un tooltip con i criteri non verificati.  
È possibile navigare nella tabella tramite i tasti freccia su/giù, Pag↑/Pag↓, Home e Fine.  
Con un **doppio clic** su una riga della tabella degli elementi viene aperta la finestra dei **controlli normativi 
personalizzati** per l'elemento selezionato.  
Con il tasto destro nella tabella degli elementi si apre il menu contestuale con i comandi della barra delle azioni.  

**Tabella delle verifiche**  

La tabella delle verifiche mostra i criteri di controllo relativi all'elemento geometrico selezionato nella tabella 
degli elementi.  
L'elenco delle verifiche è organizzato nelle seguenti colonne:  
- **Criterio**: Criterio di verifica previsto dalla normativa  
- **Elemento**: Valore dell'elemento di progetto  
- **Riferimento**: Valore limite di riferimento  
- **Esito**: Risultato della verifica:  
  - Verificato <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/verified.jpg" width="16" height="16"> (*buono*) / 
  <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/acceptable.jpg" width="16" height="16"> (*accettabile*)  
  - Non verificato <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/unverified.jpg" width="16" height="16">  
  - Inattivo <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/inactive.jpg" width="16" height="16">  

I criteri di ogni singolo elemento possono essere attivati o disattivati con un **doppio clic** nella **tabella delle 
verifiche**, agendo sul criterio relativo all’elemento selezionato nella **tabella degli elementi**.  
Con il tasto destro nella tabella delle verifiche si apre il menu contestuale con i comandi:  

<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/active.jpg" width="16" height="16"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/inactive.jpg" width="16" height="16"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/sync_settings.jpg" width="16" height="16">

  - Comando **Attiva tutti**: attiva tutti i criteri di verifica per l'elemento selezionato  
  - Comando **Disattiva tutti**: disattiva tutti i criteri di verifica per l'elemento selezionato  
  - Comando **Applica impostazioni**: applica i criteri di verifica attivi nelle impostazioni per l'elemento selezionato  

**Registro delle verifiche**  

Per ciascun criterio selezionato nella vista delle verifiche, il **registro delle verifiche** fornisce una descrizione 
dettagliata della procedura di calcolo e del confronto con il valore limite previsto dalla normativa.  

**Barre dei comandi**:  

Le barre dei comandi sono suddivise in:  

**Barra di progetto** (*in alto*)   

<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/open.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/save_as.jpg" width="24" height="24">  

  - Comando **Apri file** (Ctrl+O): apre un file `.txt`, `.xlsx`, `.xml`, `.strad`  
  - Comando **Salva progetto** (Ctrl+S): salva il progetto corrente su file `.strad`  

Il comando **Apri file** è accompagnato da un elenco dei file di progetto `.strad` recenti, incluso l'ultimo salvataggio 
automatico (eseguito ogni 5 minuti e alla chiusura dell'applicazione). Passando con il cursore su una voce dell'elenco, 
viene visualizzato un tooltip con il percorso, la data e l'ora dell'ultima modifica.  

**Barra degli strumenti** (*in alto*)  

<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/config.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/speed.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/chart.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/export.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/custom.jpg" width="24" height="24">  

  - Finestra delle **Impostazioni** (Ctrl+,): gestione delle caratteristiche della strada e dei criteri di verifica  
  - Finestra dei **Limiti locali** (Ctrl+L): personalizzazione delle tratte con limiti di velocità locali  
  - Finestra dei **Diagrammi** (Ctrl+D): visualizzazione dei diagrammi di velocità e visibilità  
  - Finestra di **Esportazione rapporti delle verifiche** (Ctrl+P): esportazione dei tabulati riassuntivi  
  - Finestra dei **Controlli normativi personalizzati** (Ctrl+N): verifica dei limiti normativi con parametri personalizzati  

**Barra delle informazioni** (*in alto*)   

<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/info.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/help.jpg" width="24" height="24">  

  - Finestra delle **Informazioni**: versione, note generali e contatti  
  - Finestra della **Guida** (F1): documentazione online completa (richiede connessione a Internet)  

**Barra delle preferenze** (*in alto*)   

<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/language.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/sun.jpg" width="24" height="24"> | <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/language.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/moon.jpg" width="24" height="24">  

  - Comando **Lingua**: seleziona la lingua dell'applicazione  
  - Comando **Tema**: attiva/disattiva il tema scuro  

**Barra dei filtri** (*a destra*)  

<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/highlight_off.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/filter_off.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/next.jpg" width="24" height="24"> | <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/highlight_on.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/filter_on.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/next.jpg" width="24" height="24">  

  - Comando **Evidenzia**: evidenzia gli elementi non verificati e le verifiche non soddisfatte  
  - Comando **Filtra**: mostra solo gli elementi non verificati  
  - Comando **Prossimo elemento non verificato** (Tab): seleziona il prossimo elemento non verificato  

**Barra delle azioni** (*a destra*)  

<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/undo.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/redo.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/copy.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/paste.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/delete.jpg" width="24" height="24">  

  Le azioni di questa barra sono accessibili anche tramite il tasto destro del mouse nella tabella degli elementi:  
  - Comando **Annulla** (Ctrl+Z): annulla l'ultima azione di importazione o eliminazione elementi (max: 20 azioni)  
  - Comando **Ripeti** (Ctrl+Y): ripete l'ultima azione annullata  
  - Comando **Copia** (Ctrl+C): copia il contenuto della vista corrente in formato tabulato, da incollare in Excel  
  - Comando **Incolla** (Ctrl+V): incolla un testo tabulato con i parametri degli elementi della vista corrente  
  - Comando **Elimina** (Canc): elimina tutti gli elementi della vista corrente, previa conferma  

**Barra delle viste** (*in basso*)  

<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/alignment.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/profile.jpg" width="24" height="24">  

  - Vista **Tracciato**: visualizza gli elementi e le verifiche del tracciato  
  - Vista **Profilo**: visualizza gli elementi e le verifiche del profilo  

**Barra della ricerca** (*in basso*)

<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/search.jpg" width="24" height="24">  

  - Comando **Cerca** (Ctrl+F): evidenzia il testo inserito nella tabella degli elementi in tempo reale, senza distinzione 
  tra maiuscole e minuscole  

Quando attivato, il comando **Cerca** è accompagnato da un'etichetta che mostra la posizione della riga selezionata sul 
totale delle righe contenenti il testo cercato, e da due comandi aggiuntivi:  

<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/arrow_up.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/arrow_down.jpg" width="24" height="24">  

  - Comando **Cerca precedente** (F2): seleziona la riga precedente contenente il testo cercato  
  - Comando **Cerca successivo** (F3): seleziona la riga successiva contenente il testo cercato  

**Barra di stato** (*in basso*)  

  La barra di stato mostra i messaggi di conferma delle operazioni di *copia*, *incolla*, *elimina*, *annulla*, *ripeti* 
  ed eventuali errori, con l'ora dell'evento e una breve descrizione.  

### 8.2 <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/config.jpg" width="24" height="24"> Finestra delle impostazioni  
<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/config_window.jpg">  

La finestra delle impostazioni compare di default all'avvio dell'applicazione e all'importazione di un file di progetto 
`.strad`. Contiene una serie di opzioni che l'utente può selezionare e modificare in qualsiasi momento, con effetto 
immediato sui calcoli delle verifiche e sulle informazioni visualizzate nelle altre finestre.  
La finestra è suddivisa in due schede principali: **Piattaforma** e **Verifiche**.

**Scheda Piattaforma**  
  **Tipo di tracciato:**  
  *1. Strada*: per tracciati stradali secondo il D.M. del 05/11/2001  
    **Tipo di strada**: selezionabile tra le categorie stradali previste  
    **Tipo di piattaforma**  
      - *Carreggiata singola*: a doppio senso di marcia  
      - *Carreggiata monosenso*  
      - *Carreggiate separate*: ciascuna a senso unico di marcia  
    **Larghezza del margine interno** [m]: valore non negativo (solo per le carreggiate separate)  

  *2. Rampa*: per tracciati di rampe in intersezioni a livelli sfalsati secondo il D.M. del 19/04/2006  
    **Tipo di strada di provenienza**: selezionabile tra le categorie stradali previste  
    **Tipo di strada di destinazione**: selezionabile tra le categorie stradali previste  
    **Tipo di rampa**  
      - *Diretta*  
      - *Semidiretta*  
      - *Indiretta*  
    **Direzione**  
      - *Monodirezionale*  
      - *Bidirezionale*  
  
  **Posizione dell'asse**: posizione dell'asse di rotazione rispetto alla carreggiata  
    - *Centro*  
    - *Sinistra*  
    - *Destra*  
  **Tipo di sezione**: configurazione della falda in rettifilo  
    - *Doppia falda* (-2.50% | -2.50%)  
    - *Singola falda (ciglio sx alto)* (+2.50% | -2.50%)  
    - *Singola falda (ciglio dx alto)* (-2.50% | +2.50%)  
  **Numero di corsie per senso di marcia**: valore conforme al tipo di strada (max: 6)  
  **Larghezza della corsia** [m]: valore compreso tra 2.75 e 4.00 m  
  **Pendenza trasversale massima** [%]: valore compreso tra 2.5% e 7.0%  
  **Velocità minima di progetto** [km/h]: valore conforme al tipo di strada  
  **Velocità massima di progetto** [km/h]: valore conforme al tipo di strada  

Le opzioni disponibili sono limitate a quelle ammesse dalla normativa per ciascuna combinazione di parametri, al fine di 
ridurre errori non intenzionali nella configurazione della piattaforma.  

Al cambio della categoria stradale viene in automatico aggiornata la larghezza della corsia e la pendenza trasversale 
massima al valore standard di normativa. La modifica manuale del valore viene segnalata con il colore rosso per indicare 
un valore non nominale.  

**Scheda Verifiche**  

La scheda *Verifiche* elenca i criteri di controllo previsti dai riferimenti normativi.  
I criteri sono suddivisi in sottocategorie, ciascuna in una scheda dedicata:  

**Tracciato**  
  - Rettifilo  
  - Clotoide  
  - Arco  

**Profilo**  
  - Livelletta  
  - Parabola  

Le modifiche ai criteri attivati nelle impostazioni per il tipo di elemento hanno effetto solo sui nuovi elementi della 
successiva importazione. Tuttavia, nella parte inferiore della scheda *Verifiche* è presente la casella **Applica in 
tempo reale**: se selezionata, le successive modifiche sovrascriveranno i criteri dei singoli elementi già importati.  

In fondo alla finestra *Impostazioni* è presente la casella **Auto salvataggio**, attiva di default, che consente di 
salvare automaticamente le impostazioni delle schede *Piattaforma* e *Verifiche* alla chiusura dell'applicazione.  

### 8.3 <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/speed.jpg" width="24" height="24"> Finestra dei limiti cinematici locali  
<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/limits_window.jpg">  

La finestra dei limiti cinematici locali consente di aggiungere tratte con parametri specifici, 
come velocità massima, accelerazione e tempo di reazione aggiuntivo rispetto a quello di base.  
Queste tratte sono utili per simulare i seguenti casi reali:  
- Presenza di punti di precedenza o stop  
- Tratte con limite massimo di velocità ridotto rispetto al limite generale  
- Simulazione di un comportamento di guida realistico in prossimità di incroci, dove si prevede 
  un tempo di reazione maggiorato e/o valori di accelerazione/decelerazione diversi da quelli nominali  

Secondo il D.M. 05/11/2001, tali condizioni richiedono il ricalcolo di:  
- Distanza di transizione nella costruzione del diagramma di velocità (§5.1.2)  
- Distanza di visuale minima richiesta per l’arresto (§5.4.1)  

Nella parte superiore della finestra sono presenti i tasti 
<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/add.jpg" width="16" height="16"> e <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/remove.jpg" width="16" height="16"> 
per aggiungere una nuova tratta o eliminare quella selezionata.  

Per ciascuna tratta sono modificabili i seguenti parametri:  
- **Prog. iniziale**: progressiva iniziale della tratta [m] (default: 0+000.000)  
- **Bloc. inizio trac.**: blocco della progressiva iniziale alla progressiva del tracciato (default: false)  
- **Prog. finale**: progressiva finale della tratta [m] (default: 0+000.000)  
- **Bloc. fine trac.**: blocco della progressiva finale alla progressiva del tracciato (default: false)  
- **Lunghezza**: lunghezza della tratta [m] (default: 000.000)  
- **V. max**: velocità massima sulla tratta [km/h] (default: 0; max: 160)  
- **Accelerazione**: accelerazione in uscita dalla tratta a velocità ridotta [m/s²] (e decelerazione in entrata) 
  (default: 0.8; max: 3.0)  
- **+ T. reazione**: tempo di reazione aggiunto [s] (default: 0.0; max: 3.0)  

La progressiva iniziale/finale è modificabile solo se non bloccata alla progressiva del tracciato.  
Se una delle due è bloccata, si attiva la modifica della lunghezza della tratta; altrimenti, la lunghezza viene calcolata 
automaticamente.  

I dati numerici inseriti vengono evidenziati in **arancione** nel caso di valori **inattesi** o **non nominali**.  
Questo non implica un errore, ma segnala all’utente di prestare attenzione ai dati inseriti.  
I casi evidenziati automaticamente sono:  
- Progressiva iniziale precedente alla progressiva iniziale del tracciato  
- Progressiva iniziale successiva alla progressiva finale del tracciato  
- Progressiva finale precedente alla progressiva iniziale del tracciato  
- Progressiva finale successiva alla progressiva finale del tracciato  
- Lunghezza superiore alla lunghezza del tracciato  
- Velocità massima superiore alla velocità di progetto del tracciato  
- Accelerazione diversa da quella nominale prevista dalla normativa (0.8)  
- Tempo di reazione aggiunto non nullo  

Ogni modifica alle progressive, allo sviluppo del tracciato o alla velocità di progetto comporta un riesame automatico 
dei casi sopra elencati. I tratti con un limite locale vengono evidenziati nella **finestra dei diagrammi** con una 
linea grigia nel diagramma delle velocità.  

### 8.4 <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/chart.jpg" width="24" height="24"> Finestra dei diagrammi  
<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/chart_window.jpg">  

Questa finestra offre una visualizzazione grafica in tempo reale del diagramma delle velocità, dell'andamento dei cigli 
e dei vari diagrammi di visibilità, consultabili, copiabili ed esportabili in qualsiasi momento.  

**Barra degli strumenti** (*in alto*)  

  <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/chart_toolbar.jpg" width="243" height="28">  
  
  - Reset  
  - Vista precedente  
  - Vista successiva  
  - Sposta (tasto sinistro) / Zoom (tasto destro)  
  - Zoom rettangolo  
  - Configurazioni  
  - Parametri dell'asse, della curva e dell'immagine  
  - Salva figura  

Oltre agli strumenti della barra, è possibile effettuare le seguenti azioni:  
  - Zoom in/out: **rotella del mouse** 
  - Adatta vista: **F** o doppio clic sulla rotella del mouse  

**Barra dei filtri** (*a destra*)  

<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/highlight_off.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/sync_off.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/forward.jpg" width="24" height="24"> | <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/highlight_on.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/sync_on.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/back.jpg" width="24" height="24">  

  - Comando **Evidenzia**: evidenzia i limiti (inferiore e superiore) e le aree critiche (non verificate)  
  - Comando **Sincronizza**: sincronizza l’intervallo evidenziato (in grigio) con l’elemento selezionato nella tabella 
  degli elementi  
  - Comando **Inverti**: visualizza i diagrammi di visibilità relativi alla direzione inversa del tracciato, attivo per tracciati bidirezionali  

**Barra delle azioni** (*a destra*)  

<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/copy.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/paste.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/delete.jpg" width="24" height="24">  

  - Comando **Copia** (Ctrl+C): copia le coordinate dei diagrammi correnti in formato tabulato, da incollare in Excel  
  - Comando **Incolla** (Ctrl+V): incolla un testo delimitato da virgole contenente le coordinate del diagramma di 
  visuale libera ottenuto dal modello tridimensionale  
  - Comando **Elimina** (Canc): elimina il diagramma di visuale libera, previa conferma  

**Barra di esportazione** (*a destra*)  

<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/log.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/overwrite.jpg" width="24" height="24">  

  - Comando **Esporta CSV**: esporta i diagrammi correnti in file delimitati: 
  `.csv` (semicolon delimited / comma delimited), `.txt` (space delimited)  
  - Comando **Salva XML** (Ctrl+S): salva e, se necessario, sovrascrive i diagrammi correnti nel file `.xml` da cui 
    è stato importato il tracciato e/o il profilo  

**Barra dei diagrammi** (*in basso*)  

<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/speed.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/chart2.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/sight.jpg" width="24" height="24">  

  - **Diagramma delle velocità**  
  - **Andamento dei cigli**  
  - **Diagrammi di visibilità**:  
    - *Visibilità per l'arresto*  
    - *Visibilità per il sorpasso*  
    - *Visibilità per la manovra di cambio corsia*  

Con la rotella del mouse è possibile eseguire lo zoom in/out lungo l'asse delle ascisse di ogni diagramma.  

**Barra di stato** (*in basso*)  
  Come nella finestra principale, la barra di stato mostra i messaggi di conferma delle operazioni di *copia*, 
*incolla*, *elimina*, *salva* ed eventuali errori, con l’ora dell’evento e una breve descrizione.  

### 8.5 <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/export.jpg" width="24" height="24"> Finestra dell'esportazione dei rapporti  
<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/export_window.jpg">  

La finestra dell'esportazione consente di visualizzare in tempo reale i riepiloghi delle verifiche normative relative 
agli elementi importati. La parte centrale della finestra mostra il rapporto selezionato, con un riepilogo dei dati 
generali della strada e degli eventuali limiti locali inseriti.  

**Dati generali e verifiche**  

I dati generali della strada includono gli stessi specificati nella **finestra delle impostazioni** oltre a:  
- **Nome del tracciato**: nel caso sia importato da **LandXML**  
- **Riferimento normativo**: D.M. 05/11/2001 e/o D.M. 19/04/2006  
- **Progressiva iniziale** [m]: per la progressiva iniziale del tracciato (o del profilo se manca il tracciato planimetrico  
- **Progressiva finale** [m]: per la progressiva finale del tracciato (o del profilo se manca il tracciato planimetrico)  
- **Lunghezza** [m]: per la lunghezza totale del tracciato (o del profilo se manca il tracciato planimetrico)  

I limiti locali vengono visualizzati (se esistono) con i parametri precedentemente menzionati per la 
**finestra dei limiti locali**  

Le verifiche planimetriche / altimetriche vengono elencati sotto ogni elemento in forma tabellare con la prima riga 
che contiene l'ordine dell'elemento, il tipo di elemento e *V. max* desunta del diagramma delle velocità fase finale.  
Gli esiti vengono visualizzati successivamente come nella **tabella delle verifiche** nella **finestra principale**.  
Nella prima colonna vengono visualizzati i segnali 
**verde** <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/verified.jpg" width="16" height="16"> e 
**rosso** <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/unverified.jpg" width="16" height="16"> 
per indicare l'esito positivo o negativo del criterio, mentre il segnale rappresentato prima riga indica lo stato della 
verifica dell'elemento se sono soddisfatti tutti i criteri sottoelencati contemporaneamente, sempre con un segnale 
**verde** <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/verified2.jpg" width="16" height="16"> o 
**rosso** <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/unverified2.jpg" width="16" height="16">.

Da notare che i criteri disattivati (con doppio clic) nella **tabella delle verifiche** della **finestra principale** 
non vengono elencati nell'esportazione dei rapporti delle verifiche.  

Oltre alla vista centrale, sono disponibili tre barre:  

**Barra di esportazione** (*in alto*)  

<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/log.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/save_as.jpg" width="24" height="24">  

  - Comando **Esporta registro**: esporta il registro completo con le procedure di verifica di tutti i criteri per gli 
  elementi planimetrici e altimetrici in formato `.txt`  
  - Comando **Salva anteprima** (Ctrl+S): salva l'anteprima corrente in formato `.pdf` / `.html`/ `.xlsx` / `.dxf`  

**Barra delle modifiche** (*in alto*)  

<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/refresh.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/edit_off.jpg" width="24" height="24"> | <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/refresh.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/edit.jpg" width="24" height="24">  

  - Comando **Aggiorna**: aggiorna i tabulati riassuntivi delle verifiche, qualora siano state modificate manualmente  
  - Comando **Modifica**: abilita/disabilita la modifica manuale dei tabulati riassuntivi delle verifiche  

**Barra delle viste** (*in basso*)  

<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/alignment.jpg" width="24" height="24"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/profile.jpg" width="24" height="24">  

  - Vista **Tracciato**: visualizza le verifiche degli elementi planimetrici nella vista centrale  
  - Vista **Profilo**: visualizza le verifiche degli elementi altimetrici nella vista centrale  

**Barra di stato** (*in basso*)  
  Come nella finestra principale, la barra di stato mostra i messaggi di conferma delle operazioni di esportazione del 
registro delle verifiche e il salvataggio dei rapporti.  

### 8.6 <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/custom.jpg" width="24" height="24"> Finestra dei controlli normativi personalizzati  
<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/custom_window.jpg">  

La finestra dei controlli normativi personalizzati di normativa consente il calcolo dei limiti normativi dei vari criteri 
utilizzando parametri di input fittizi, non legati al tracciato reale.  

La finestra è suddivisa orizzontalmente in due sezioni:  

- **Sezione Input** (*a sinistra*)  
  Contiene i tipi di elementi geometrici tra cui selezionare uno, e gli input necessari da definire per l'elemento scelto:  

  - **Tracciato**  
    *Rettifilo*  
      - **V.max**: velocità massima del rettifilo [km/h]  
      - **A1**: parametro di scala della clotoide precedente [m] (per il caso di flesso)  
      - **A2**: parametro di scala della clotoide successiva [m] (per il caso di flesso)  

    *Clotoide*  
      - **V.max**: velocità massima della clotoide [km/h]  
      - **A1**: parametro di scala della clotoide precedente [m]  
      - **A2**: parametro di scala della clotoide successiva [m]  
      - **Ri**: raggio di curvatura nel punto iniziale [m] (nullo per rettifilo)  
      - **Rf**: raggio di curvatura nel punto finale [m] (nullo per rettifilo)  
      - **qi**: pendenza trasversale iniziale del ciglio esterno [m/m]  
      - **qf**: pendenza trasversale finale del ciglio esterno [m/m]  

    *Arco*  
      - **V.max**: velocità massima della curva circolare [km/h]  
      - **L1**: lunghezza del rettifilo precedente [m]  
      - **L2**: lunghezza del rettifilo successivo [m]  

  - **Profilo**  
    *Livelletta*  
      - **V.max**: velocità massima della livelletta [km/h]  

    *Parabola*  
      - **V.max**: velocità massima del raccordo verticale [km/h]  
      - **L**: lunghezza del raccordo [m]  
      - **i**: pendenza longitudinale media del raccordo [m/m]  
      - **Δi**: differenza di pendenza longitudinale (i₂ - i₁) [m/m]  

- **Sezione Output** (*a destra*)  
  Mostra il riepilogo della procedura di calcolo dei limiti normativi per il tipo di elemento selezionato, insieme ai 
valori dei parametri di input inseriti.  

Con un **doppio clic** su una riga della tabella degli elementi viene aperta la finestra dei **controlli normativi 
personalizzati** per l'elemento selezionato.  

---
## 9. Come si usa  
### 9.1 Input  
I dati del tracciato/profilo e le coordinate del diagramma di visuale libera possono essere importati tramite semplice 
**copia-incolla** oppure **trascinando il file** nella finestra corrispondente dell'applicazione.  

**Formati supportati**  

**Tracciato / Profilo**  
- `.txt` (colonne separate da tabulazioni)  
- `.xlsx`  
- `.xml` (formato LandXML)  
- `.strad` (progetto Stradifica)  

**Visuale libera**  
- `.txt` (coordinate separate da virgola)  

**Modalità di importazione**  

I dati del tracciato e del profilo possono essere importati da Autodesk Civil 3D (*Italiano / English*) in Stradifica 
in due modalità:  

1. Impostare la vista desiderata (**Tracciato** o **Profilo**) nella finestra principale, copiare i dati degli elementi 
dall'*editor geometria*/*geometry editor* tramite il comando *copia tutto*/*copy all* e incollarli nella finestra principale 
di Stradifica utilizzando con il comando **Incolla** da:  
  - Tastiera *Ctrl+V*  
  - Menu contestuale (tasto destro del mouse sulla tabella degli elementi)  
  - Barra delle azioni  

<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/geometry_editor.jpg"> <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/grid_view.jpg">  

  In alternativa, è possibile incollare i dati in un file `.txt` o in un foglio Excel `.xlsx`, salvarlo e importarlo 
successivamente in Stradifica.  

Questa modalità di importazione tramite copia-incolla è preferibile durante la fase di modifica del tracciato/profilo, 
tenendo entrambe le finestre aperte contemporaneamente.  

2. Esportare il tracciato e, se disponibile, il profilo in formato LandXML `.xml`, quindi importarlo in Stradifica.

  Dopo l'importazione, verrà richiesto di selezionare il tracciato e, eventualmente, il profilo da caricare.  
  *Nota: il nome del tracciato/profilo selezionato verrà proposto automaticamente per le importazioni successive.*  

Questa modalità di importazione da LandXML è preferibile al termine delle modifiche del tracciato/profilo per salvare 
i diagrammi di velocità e/o visibilità da reimportare successivamente in Civil 3D come profili associati al tracciato.  

Per entrambe le modalità, tutti i formati supportati possono essere importati nella finestra principale con il comando **Apri file** 
(Ctrl+O) specificando il percorso del file, oppure trascinandolo direttamente nella finestra.  

Il diagramma della **visuale libera** può essere importato nella finestra dei diagrammi dal report di visibilità `.txt` 
generato da Civil 3D (impostando *ReportCSV.xsl*). Dopo aver selezionato il tipo di diagramma di visibilità e la direzione 
del tracciato, si può trascinare il report nella finestra oppure, in alternativa, copiare il contenuto del report e 
incollarlo utilizzando il comando **Incolla** da:  
  - Tastiera *Ctrl+V*  
  - Barra delle azioni  

### 9.2 Salvataggio e scambio dati  

Gli elementi importati con le impostazioni scelte possono essere salvati in un file di progetto Stradifica (`.strad`). 
Un formato di scambio che contiene i dati di tracciato, profilo, limiti personalizzati, diagrammi e le impostazioni di 
piattaforma e di verifiche.  

Il formato `.strad` conserva il percorso **assoluto** del file LandXML da cui sono stati importati gli elementi. 
Se un file `.strad` viene aperto in assenza del relativo `.xml` (ad esempio per cambio di percorso o di PC), 
Stradifica cerca automaticamente il file `.xml` nella stessa cartella del file `.strad`, facilitando in qualsiasi 
momento l'esportazione dei profili dei diagrammi di velocità/visibilità nel file LandXML di origine.  

### 9.3 Gestione delle verifiche  
Alla prima importazione degli elementi, vengono attivati esclusivamente i criteri contrassegnati nella finestra delle 
impostazioni per ciascun tipo di elemento. Eventuali modifiche ai criteri attivati per i singoli elementi vengono 
memorizzate e mantenute nelle successive importazioni, a condizione che l'elemento conservi la stessa posizione rispetto 
al tracciato/profilo. In caso contrario, con una nuova importazione, i criteri attivi saranno quelli predefiniti 
indicati nelle impostazioni.  

I criteri di ogni singolo elemento possono essere attivati o disattivati con un **doppio clic** nella **tabella delle 
verifiche**, agendo sul criterio relativo all’elemento selezionato nella **tabella degli elementi**.  
Il criterio di verifica inattivo viene:  

- segnalato con la scritta <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/inactive.jpg" width="16" height="16"> **Inattivo** nella colonna **esito** nella **tabella delle verifiche**  
- escluso dai controlli dei parametri nella **tabella degli elementi** se il filtro <img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/highlight_on.jpg" width="16" height="16"> **Evidenzia** è attivato
- escluso dal riepilogo delle verifiche nella **finestra dell'esportazione dei rapporti**  

Le modifiche ai criteri attivi nelle impostazioni influenzano solo gli elementi nuovi importati.  
Per applicare immediatamente le modifiche a tutti gli elementi attualmente presenti, sovrascrivendo eventuali modifiche 
manuali, è necessario selezionare la casella **Applica in tempo reale**.  

Nei seguenti casi, il criterio viene disattivato automaticamente se non già disattivato, qualora non risulti soddisfatto:  
- **Lunghezza minima** del rettifilo terminale (primo/ultimo) del tracciato  
- **Raggio minimo da Vpmin**, quando la velocità massima della curva circolare è inferiore a Vpmin a causa di un limite 
locale ridotto, e non per insufficienza del raggio planimetrico  

In tali situazioni, i criteri vengono riattivati automaticamente se tornano ad essere soddisfatti.  
La disattivazione manuale (tramite **doppio clic** o l'azione **disattiva tutti**) impedisce la riattivazione automatica, in quanto il criterio è stato 
disattivato esplicitamente dall’utente.  

### 9.4 Analisi dei risultati  
Nella finestra principale è possibile consultare l’analisi delle verifiche e delle velocità attivando il comando 
**Evidenzia**. L’attivazione evidenzia, tramite una scala cromatica, lo stato di verifica dei vari criteri e delle 
velocità.  

I valori dei parametri **Lunghezza**, **A** e **Raggio** vengono evidenziati in **rosso** e affiancati tra parentesi dai 
relativi valori limite quando risultano coinvolti in almeno un criterio non verificato. Passando con il cursore sul 
parametro non verificato viene visualizzato un tooltip con lo scarto da recuperare per raggiungere il valore limite.
Il valore della **sopraelevazione** viene colorato in rosso quando supera **-2.50%** in assenza di transizione precedente 
e/o successiva.  

Per le velocità di 1° fase (**V. 1°fase** delle curve planimetriche) e di fase finale (**V. max** di ogni elemento), i 
colori variano secondo le seguenti condizioni:  

- **<span style="color: #1a6fb5;">Blu</span>**: se **V. 1°fase** o **V. max** è pari a **Vpmax**  
- **<span style="color: #808080;">Grigio</span>**: se **V. max** è inferiore a **Vpmax** per effetto di un limite locale applicato  
- **<span style="color: #ff4444;">Rosso</span>**: se **V. 1°fase** o **V. max** è inferiore a **Vpmin** a causa di un raggio planimetrico insufficiente  
- **<span style="color: #a87208;">Giallo</span>**: se **V. max** è inferiore a **Vpmin** per effetto di un altro elemento planimetrico più vincolante  
- **<span style="color: #c45510;">Arancione</span>**: se la differenza di **V. max** con l’elemento successivo o precedente supera il limite ammesso  
- **<span style="color: #5a9e35;">Verde</span>**: se **V. 1°fase** o **V. max** è superiore a **Vpmin**  

Se più condizioni sono soddisfatte contemporaneamente, viene applicato il colore corrispondente alla condizione di 
ordine superiore.  

A ogni importazione di elementi avvenuta con successo viene evidenziato nella barra di stato, oltre alla descrizione del 
tipo di importazione, il numero di elementi **non verificati** attualmente seguito, tra parentesi, dalla differenza di 
elementi **non verificati** tra l'importazione attuale e quella precedente. Un elemento viene considerato 
**non verificato** quando almeno un criterio di verifica **attivo** risulta **non verificato**.  

Nella finestra dei diagrammi, il comando **Evidenzia** può essere attivato dalla barra delle azioni per mettere in 
risalto le zone critiche con non conformità normative.  
Nel diagramma delle velocità vengono inoltre visualizzati i limiti inferiore e superiore dell’intervallo di velocità 
di progetto, come definiti dall’utente nelle impostazioni.  

### 9.5 Output  
**Formati supportati**  

**Rapporti delle verifiche**  
- `.pdf` / `.html` / `.xlsx` / `.dxf`: riepilogo tabulato delle caratteristiche della strada, limiti locali e verifiche 
planimetriche/altimetriche attive  
- `.txt`: registro completo della procedura di calcolo di tutti i criteri, inclusi quelli non attivati  

**Diagrammi**  
- `.xml`  
- `.png`  
- `.jpeg` / `.jpg`  
- `.pgf`  
- `.pdf`  
- `.ps`  
- `.raw` / `.rgba`  
- `.svg` / `.svgz`  
- `.tif` / `.tiff`  
- `.webp`  

**Modalità di esportazione**  
  
I rapporti delle verifiche e il registro completo possono essere esportati dalla barra delle azioni della 
**finestra di esportazione dei rapporti**, tramite i comandi **Esporta registro** e **Salva anteprima**, 
selezionando nome, formato e cartella di destinazione. Al termine del salvataggio verrà chiesto se aprire il file creato.  

Le catture dei diagrammi di velocità e visibilità possono essere esportate nei formati precedentemente elencati, tramite 
il comando **Salva figura** nella barra degli strumenti della **finestra dei diagrammi**, selezionando nome, formato e 
cartella di destinazione.  

I diagrammi di velocità e visibilità possono essere salvati nel file `.xml` da cui sono stati importati i dati geometrici, 
tramite il comando **Salva xml**. L’operazione salva i diagrammi della vista corrente come nuovi profili associati al 
tracciato importato, sovrascrivendo eventuali profili esistenti con lo stesso nome.
Per il diagramma di velocità, oltre al profilo, vengono esportate nel file `.xml` anche le caratteristiche delle 
**Velocità di progetto**, consultabili dopo la reimportazione in Civil 3D nella sezione **Criteri di progettazione** 
nelle proprietà del tracciato, ed eventualmente rappresentabili come finche nella vista profilo.  

<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/design_speeds.jpg">  

Il comando **Esporta CSV** è utile per importare i diagrammi in Civil 3D senza la necessità di salvarli in LandXML. In particolare:
  - Diagrammi di velocità e visibilità: esporta i profili in un file delimitato da spazio da importare in Civil 3D tramite 
  il comando *Crea profilo da file*  

<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/profile_from_file.jpg">  

  - Andamento dei cigli: esporta il file delimitato da punto e virgola (sistema italiano) o da virgola (sistema inglese) 
  da importare in Civil 3D tramite il comando **Importa dati di sopraelevazione** dall'editor tabellare di sopraelevazioni 
  relativo al tracciato in esame  

<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/superelevation_tabular_editor.jpg">  
<img src="https://raw.githubusercontent.com/eslamanter/stradifica-release/main/images/superelevation_from_file.jpg">  

---
## 10. Come funziona il codice  
### 10.1 Importazione dei dati  

Durante l’importazione dei dati geometrici separati da tabulazione (tramite copia-incolla, file `.txt` o `.xlsx`), 
vengono cercate le seguenti colonne:  

Importazione di un tracciato:  
  - *No. / N.*  
  - *Length / Lunghezza*  
  - *Radius / Raggio*  
  - *A*  
  - *Start Station / Progressiva iniziale*  
  - *End Station / Progressiva finale*  
  - *Start Direction / Direzione iniziale*  
  - *End Direction / Direzione finale*  
  - *Greater than 180 / Maggiore di 180*  

Importazione di un profilo:  
  - *No. / N.*  
  - *PVI Station / Progressiva VA*  
  - *Grade Out / Pendenza % in uscita*  
  - *Profile Curve Length / Lunghezza curva di profilo*  
  - *Curve Radius / Raggio curva*  

La mancanza di uno qualsiasi dei parametri richiesti interrompe l’importazione e genera un messaggio di errore che 
specifica il primo parametro mancante. Alla conferma di lettura del messaggio, viene conservato nella barra di stato.  

Nel caso di importazione da file `.xml`, vengono cercati i seguenti parametri:  

Importazione di un tracciato:  
  - Line: *length*  
  - Spiral: *length, radiusStart, radiusEnd*  
  - Curve: *length, radius, cw*  

Importazione di un profilo:  
  - PVI  
  - ParaCurve  

**Nota bene**  

- Nella variazione dei parametri geometrici di input (es. lunghezza, A, raggio) tra due importazioni successive, 
  i criteri attivi e disattivi di ciascun elemento vengono mantenuti solo se l'elemento conserva la stessa posizione 
  rispetto al tracciato/profilo. Al primo elemento che risulta di tipo diverso rispetto alla posizione corrispondente 
  nell'importazione precedente, vengono associati i criteri di default definiti nella **finestra delle impostazioni**, 
  a partire da quell'elemento in poi. Ad esempio, dato un tracciato *rettifilo-clotoide-curva-clotoide-rettifilo*, 
  se viene reimportato come *rettifilo-clotoide-curva-clotoide-curva-clotoide-rettifilo*, i criteri di default vengono 
  applicati agli ultimi 3 elementi *curva-clotoide-rettifilo*, incluso il rettifilo finale, che ha cambiato posizione 
  a seguito dell'inserimento della clotoide di continuità e della curva policentrica. Eventuali modifiche ai criteri 
  del rettifilo finale verranno sovrascritte.  
  - Non viene verificata la fattibilità geometrica né la correttezza della sequenza degli elementi del tracciato/profilo, 
  in quanto i dati provengono da software di modellazione stradale.  
- Si assume la conformità normativa dei tipi di elementi che compongono il tracciato plano-altimetrico. Pertanto:  
  - Il tipo di elemento di transizione planimetrica non viene verificato: si assume che sia una clotoide.  
  - Il tipo di raccordo altimetrico non viene verificato: si assume che sia una parabola simmetrica (non circolare).  

### 10.2 Flusso di verifica  
Di seguito le operazioni eseguite **automaticamente** in sequenza:  
- Aggiornamento dei parametri geometrici degli elementi planimetrici/altimetrici  
- Calcolo del diagramma delle velocità:  
  - prima fase  
  - fase finale  
- Applicazione dei limiti cinematici locali personalizzati  
- Calcolo dell'andamento dei cigli, con eventuali correzioni della pendenza longitudinale ∆i  
- Verifiche degli elementi:  
  - planimetrici  
  - altimetrici  
- Calcolo delle distanze minime di visibilità per:  
  - **l'arresto**: ogni 20 m, con passo di integrazione dv = 1 km/h (profilo orizzontale assunto in assenza di dati altimetrici)  
  - **il sorpasso**: per i tracciati a carreggiata singola con doppio senso di marcia  
  - **la manovra di cambio di corsia**: per i tracciati a carreggiata monosenso o a carreggiate separate  

Le operazioni sopra elencate vengono eseguite a ogni attivazione di una delle seguenti azioni:  
- **Importazione** (avvenuta con successo) di elementi planimetrici/altimetrici tramite uno dei modi di importazione  
- Modifica di una delle caratteristiche della piattaforma nella finestra delle **impostazioni**  
- Aggiunta, modifica o eliminazione di una tratta nella finestra dei **limiti cinematici locali**  

I risultati numerici e grafici vengono aggiornati **immediatamente** in **tutte le finestre**.  

### 10.3 Approssimazioni  
Durante l’importazione dei dati numerici non viene effettuata alcuna approssimazione sui valori di input.  
Nei calcoli relativi ai parametri geometrici e cinematici, i valori numerici vengono mantenuti con piena precisione. 
Le approssimazioni vengono applicate esclusivamente ai **valori limite normativi** calcolati, secondo le seguenti convenzioni:  

- **Lunghezza [m] / Rapporto tra lunghezze [m/m]**: **3** cifre decimali  
- **Velocità [m/s] / Accelerazione [m/s²]**: **2** cifre decimali  
- **Pendenza [m/m]**: **4** cifre decimali  

Tutti i diagrammi calcolati e importati vengono automaticamente semplificati eliminando i punti intermedi **collineari**, 
mantenendo solo i punti di cambio di direzione.  

---
## 11. Componenti di terze parti  
**PySide6 (Licenza GNU LGPL v3)**  

Questa applicazione include componenti provenienti da PySide6, sviluppato e mantenuto da Qt Group.  
- Libreria e source code: [https://www.qt.io/qt-for-python](https://www.qt.io/qt-for-python)  
- Testo completo della licenza: [https://www.gnu.org/licenses/lgpl-3.0.html](https://www.gnu.org/licenses/lgpl-3.0.html)  

**Matplotlib (Licenza compatibile BSD)**  

Questa applicazione utilizza la libreria Matplotlib.  
- © 2012 Matplotlib Development Team. Tutti i diritti riservati  
- Dettagli sulla licenza: [https://matplotlib.org/stable/project/license.html](https://matplotlib.org/stable/project/license.html)  

**Google Fonts (SIL Open Font License)**  

Questa applicazione utilizza le icone Material Symbols da Google Fonts, distribuite sotto la SIL Open Font License.  
- Testo completo della licenza: [https://scripts.sil.org/OFL](https://scripts.sil.org/OFL)  

---
## 12. Collaboratori  
Un ringraziamento speciale ad [Abdulrahman Khalid](https://github.com/Abdulrahman-Khalid) per il prezioso contributo a 
questo progetto.  

---
**Stradifica v2.2**  
**© 2025 Eslam Anter**  

*Registrato al Registro Pubblico Speciale per i Programmi per Elaboratore della SIAE con il N. D000028853.*  
