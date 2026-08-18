# STRADIFICA  
**Verifica Tracciati Stradali**  

---
## Note di rilascio  

---
### Verifica Tracciati Stradali v1.0: (08/2024)  

- Interazione dalla finestra dei comandi.  
- Importazione impostazioni piattaforma ed elementi di tracciato e profilo da `.txt` pre-formattati.  
- Importazione tratte a limiti di velocità ridotti da `.txt` pre-formattato.  
- Controllo automatico della coerenza dei parametri geometrici importati.  
- Implementazione criteri di verifica di normativa del D.M. 05/11/2001.  
- Calcolo puntuale del diagramma di velocità di prima fase e di fase finale.  
- Calcolo dei diagrammi di visibilità richiesta per l'arresto, il sorpasso e la manovra di cambio corsia.  
- Esportazione dati generali, verifiche, diagrammi di velocità e di visibilità in `.txt`.  

### Novità Stradifica v2.1: (12/2025)  

- Uso educativo e didattico gratuito senza registrazione.  
- Interfaccia utente Qt multi-finestra semplice con supporto automatico del tema chiaro/scuro rilevato dal sistema.  
- Ricerca automatica degli aggiornamenti.  
- Implementazione verifiche delle rampe per le intersezioni a livelli sfalsati da D.M. 19/04/2006.  
- Impostazione piattaforma con autocontrollo dei parametri geometrici e cinematici.  
- Autosalvataggio locale delle impostazioni di piattaforma e di verifiche.  
- Importazione tracciati stradali da `.txt`, `.xlsx`, `.xml` e da Copia-Incolla da Autodesk Civil 3D.  
- Inserimento tratte con limiti cinematici personalizzati.  
- Ottimizzazione calcolo diagramma di velocità e correzione calcolo allargamento in curva.  
- Ottimizzazione precisione visibilità richiesta per l'arresto con calcolo dell'integrale.  
- Gestione manuale/automatica dei criteri da attivare sul singolo elemento importato e su tutti gli elementi.  
- Disattivazione automatica, ed eventuale attivazione, dei criteri non verificati nei contesti in cui non sono ritenuti necessari.  
- Calcolo, visualizzazione ed esportazione, in formati raster, vettoriali e `.xml`, dei diagrammi di velocità e visibilità.  
- Importazione diagrammi di visuali libere da Civil 3D e confronto grafico con le distanze di visibilità richieste.  
- Esportazione rapporti di verifiche planimetriche e altimetriche nei formati `.pdf` e `.html`.  
- Visualizzazione registro della procedura di verifica del singolo criterio per ogni elementi ed esportazione del registro completo in `.txt`.  
- Controllo limiti normativi personalizzati con parametri fittizi.  
- Analisi grafica dello stato di verifica per elemento con comandi Evidenzia e Filtra elementi non verificati.  

### Novità Stradifica v2.2: (09/2026)  
[Documentazione](https://github.com/eslamanter/stradifica-release/blob/main/README.md) | 
[Licenza](https://github.com/eslamanter/stradifica-release/blob/main/LICENSE.md)  

- Uso commerciale consentito previa comunicazione.  
- Interfaccia utente Qt dinamica, moderna e più leggibile con tema chiaro/scuro modificabile e supporto multi-lingua.  
- Salvataggio di impostazioni ed elementi, apertura progetti recenti e autosalvataggio ogni 5 min nel formato `.strad`.  
- Configurazione del tipo di falda singola/doppia nella sezione in rettifilo, per maggiore personalizzazione della piattaforma.  
- Validazione dei dati geometrici degli elementi importati, con segnalazione di eventuali anomalie.  
- Attivazione e disattivazione globale di tutti i criteri per tipo di elemento, dalle impostazioni.  
- Attivazione e disattivazione locale di tutti i criteri per elemento, oppure sincronizzazione con le impostazioni globali.  
- Ottimizzazione tempi di verifica dei tracciati lunghi (>100 elementi).  
- Comandi Annulla (Ctrl+Z) e Ripeti (Ctrl+Y) per navigare tra le importazioni successive (fino a 20).  
- Comando per navigare tra gli elementi successivi non verificati.  
- Comando Cerca per evidenziare parole chiave e navigare tra i risultati nella tabella degli elementi.  
- Tasti rapidi per tutte le finestre e i comandi principali.  
- Miglioramento di grafica, leggibilità e navigazione nella finestra dei diagrammi.  
- Calcolo dell'andamento dei cigli di corsie e banchine ed esportazione in `.csv` per Civil 3D.  
- Esportazione diagrammi di velocità e visibilità in `.txt` per Civil 3D.  
- Esportazione caratteristiche della velocità associate al tracciato nel formato `.xml` per Civil 3D.  
- Possibilità di modifica manuale dei rapporti di verifica prima dell'esportazione.  
- Calcolo tempo di viaggio del tracciato con ogni importazione e cambio impostazioni cinematiche.  
- Esportazione rapporti di verifica nei formati `.xlsx` e `.dxf`.  
- Collegamento dei controlli normativi personalizzati ai parametri dell'elemento selezionato.  
- Creazione di un file `.txt` di log per eventuali errori.  

### Novità Stradifica v3.0: (Work in Progress)  

- Supporto importazione dei tracciati ferroviari, calcolo sovralzo e verifiche dei ranghi di velocità.  
- Implementazione criteri dal Manuale di Progettazione Armamento RFI e Norme ANSFISA per i vari scartamenti.  
- Integrazione funzionalità desktop in plug-in per Civil 3D.  

---
Se trovi utile Stradifica, puoi offrirmi un caffè ☕  

<p align="left">
  <a href="https://www.buymeacoffee.com/eslamanter">
    <img src="https://img.buymeacoffee.com/button-api/?text=Offrimi%20un%20caff%C3%A8&emoji=%E2%98%95&slug=eslamanter&button_colour=FFDD00&font_colour=000000&font_family=Cookie&outline_colour=000000&coffee_colour=ffffff" width="220" />
  </a>
</p>  

---
**Stradifica**  
**© 2025 Eslam Anter**  

*Registrato al Registro Pubblico Speciale per i Programmi per Elaboratore della SIAE con il N. D000028853.*  
