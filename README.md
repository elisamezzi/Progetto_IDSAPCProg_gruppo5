# Progetto_IDSAPCProg_gruppo5
Progetto del corso *Introduzione al Pensiero Computazionale e alla Data Science* —
Università di Bologna, A.A. 2025/2026 — Gruppo 5.

## Descrizione del progetto
Il progetto sviluppa una piccola analisi di data science, riproducibile e documentata, sul fenomeno dell'*employee attrition*, cioè l'abbandono volontario dei dipendenti dall'azienda.

## Descrizione del dataset
Il dataset contiene informazioni su dipendenti aziendali, tra cui  caratteristiche demografiche, lavorative e di soddisfazione. La variabile target è **Attrition**.


## Obiettivo
Prevedere quanto è probabile che un dipendente lasci l'azienda

## Struttura del repository

```
.
├── data/        # dataset e descrizione delle variabili
├── notebooks/   # notebook di analisi
├── images/      # grafici esportati dall'analisi
└── README.md
```
## Fasi del progetto

- **Fase 1 – Descrizione e comprensione del dataset** (Maddalena Vannini): analisi
  descrittiva, statistiche, distribuzioni, qualità dei dati e prime ipotesi.

- **Fase 2 – Analisi esplorativa e visualizzazione** (Elisa Mezzi): analisi tramite
  *seaborn* che approfondisce le relazioni tra le variabili e la variabile target, con
  l'obiettivo di individuare quali feature sono più utili a prevedere l'*Attrition*.
  L'analisi è impostata in questo modo:
    - due **heatmap di correlazione** (una per le variabili numeriche e una per le
      categoriche codificate) che mostrano sia quali variabili sono legate all'abbandono, sia quali sono ridondanti tra loro;
    - sulla base dei risultati delle due heatmap, approfondimento delle variabili più
      significative con **grafici di tipo diverso** (countplot, barplot, boxplot,
      istogramma, pointplot, barre impilate, grafico a torta e scatterplot), includendo
      **confronti tra classi e tra variabili**;
    - **sintesi finale** che indica esplicitamente quali variabili sono utili e quali no per prevedere l'abbandono.

- **Fase 3 - Modellazione** (Isabella Manetti): sviluppo e analisi di tre modelli predittivi relativi all'abbandono lavorativo, in partciolare
    - **k-NN**
    - **Random Forest**
    - **Regressione logistica**

## Istruzioni per l'esecuzione
Il notebook è pensato per **Google Colab** (con Python 3). Le librerie usate
(`pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`) sono già disponibili su
Colab. Aprire il notebook in `notebooks/` ed eseguire le celle in ordine. Il dataset viene letto da `data/Employee_Attrition.csv`.

## Membri del gruppo

- Maddalena Vannini - matr.0001180470, maddalena.vannini@studio.unibo.it - `maddalena/fase1` - Descrizione dataset 
- Elisa Mezzi - matr. 0001231137 - elisa.mezzi@studio.unibo.it - `elisa/fase2` - Analisi esplorativa e visualizzazione
- Isabella Manetti - matr.0001216209, isabella.manetti2@studio.unibo.it - `Isabella/fase3`- Modellazione
