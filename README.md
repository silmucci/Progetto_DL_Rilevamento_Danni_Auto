# Progetto Deep Learning - Rilevamento Danni Auto

Questo progetto è stato sviluppato per il corso di Deep Learning e ha come obiettivo il rilevamento automatico dei danni alla carrozzeria delle automobili tramite immagini.

Il sistema utilizza un modello di Object Detection basato su YOLO11, addestrato tramite fine-tuning su un dataset in formato YOLO contenente immagini di automobili danneggiate.

## Dataset

Il dataset utilizzato per il progetto è disponibile su Roboflow Universe:

https://universe.roboflow.com/nibm-7v215/car-damage-detected-dataset-crackdentsctratch/dataset/1

Il dataset contiene immagini di automobili con danni alla carrozzeria annotate in formato YOLO.

Le classi utilizzate nel progetto sono:

- crack
- dent
- scratch

Il dataset completo non è incluso direttamente nel repository GitHub per motivi di dimensione. Nel notebook viene caricato e utilizzato in ambiente Google Colab.

## Workflow

Nel notebook sono presenti le principali fasi del progetto:

- caricamento e preparazione del dataset;
- configurazione del modello YOLO11n;
- addestramento del modello;
- validazione sul validation set;
- analisi delle metriche di valutazione;
- generazione di predizioni visive con bounding box;
- salvataggio dei pesi del modello su Google Drive.

## File principale

Il file principale del progetto è:

`Progetto_DL_Rilevamento_Danni_Auto.ipynb`

I pesi finali del modello, `best.pt` e `last.pt`, sono stati salvati su Google Drive per evitare la perdita dei risultati al termine della sessione Google Colab.
