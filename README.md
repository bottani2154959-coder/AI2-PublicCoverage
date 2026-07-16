# Analisi predittiva della copertura sanitaria pubblica

## Applicazione della regressione logistica e valutazione della fairness

**Corso:** Intelligenza Artificiale II

**Università:** Sapienza Università di Roma

**Studentesse:**
- Ilaria Bottani (2154959)
- Claudia De Rossi (1992222)


## Descrizione del progetto

Questo progetto analizza la previsione della copertura sanitaria pubblica attraverso un modello di **Regressione Logistica** applicato al dataset **ACSPublicCoverage**.

Oltre alla valutazione delle prestazioni del classificatore, viene studiato il comportamento del modello rispetto ai principali gruppi sensibili della popolazione mediante metriche di **algorithmic fairness**, al fine di individuare eventuali differenze nelle prestazioni.


## Domanda di ricerca

> **In che misura le disparità presenti nei dati storici influenzano le prestazioni di un modello di regressione logistica e quali implicazioni etiche emergono dalla valutazione della sua fairness in assenza di tecniche di de-biasing?**


## Dataset

Il dataset utilizzato è **ACSPublicCoverage**, estrapolato tramite la libreria **Folktables** e derivato dall'**American Community Survey (ACS)** dello **U.S. Census Bureau**.

L'analisi è stata svolta sui dati relativi allo **Stato della California** nell'anno **2019**.

La variabile target (**PUBCOV**) indica se un individuo possiede o meno una copertura sanitaria pubblica.


## Struttura del notebook

Il notebook principale è organizzato nelle seguenti sezioni:

1. Definizione del contesto
2. Identificazione delle feature sensibili
3. Analisi esplorativa dei dati (EDA)
4. Preprocessing
5. Regressione Logistica
6. Valutazione del modello
7. Analisi della Fairness
8. Conclusioni


## Librerie utilizzate

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Fairlearn
- Folktables


## Metriche di valutazione

### Prestazioni del modello

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix
- ROC Curve

### Fairness

- MetricFrame
- Demographic Parity Ratio
- Equalized Odds Ratio


## Come eseguire il notebook

Per riprodurre il progetto è sufficiente:

1. Aprire il notebook **ACSPublicCoverage.ipynb**.
2. Installare le librerie richieste, se non già disponibili.
3. Eseguire le celle nell'ordine in cui sono presentate.


## File presenti nella consegna

- `README.md` → informazioni sul progetto.
- `ACSPubliCoverage.ipynb` → notebook completo con codice, analisi e risultati.
- `Bottani DeRossi Progetto IA2.pdf` → relazione finale.
- `PresentazioneBottaniDeRossi.pdf` → slide della presentazione.


## Risultati principali

Il modello di regressione logistica ha ottenuto prestazioni complessivamente soddisfacenti nella previsione della copertura sanitaria pubblica. L'analisi di fairness ha evidenziato alcune differenze tra i gruppi sensibili considerati, confermando l'importanza di affiancare alle tradizionali metriche di classificazione anche una valutazione dell'equità del modello.


## Riferimenti

- American Community Survey (ACS)
- U.S. Census Bureau
- Folktables
- Scikit-learn
- Fairlearn
