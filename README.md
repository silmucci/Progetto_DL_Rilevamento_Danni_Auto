# Progetto Deep Learning - Rilevamento Danni Auto

Questo progetto è stato sviluppato per il corso di Deep Learning e ha come obiettivo il rilevamento automatico dei danni alla carrozzeria delle automobili tramite immagini.

Il sistema utilizza un modello di Object Detection basato su YOLO11, addestrato tramite fine-tuning su un dataset in formato YOLO contenente immagini di automobili danneggiate.

Le classi considerate nel progetto sono:

- crack
- dent
- scratch

Nel notebook sono presenti le principali fasi del workflow:

- caricamento e preparazione del dataset;
- configurazione del modello YOLO11;
- addestramento del modello;
- validazione sul validation set;
- analisi delle metriche di valutazione;
- generazione di predizioni visive con bounding box;
- salvataggio dei pesi del modello su Google Drive.

Il file principale del progetto è:

`Progetto_DL_Rilevamento_Danni_Auto.ipynb`

I pesi finali del modello, `best.pt` e `last.pt`, sono stati salvati su Google Drive per evitare la perdita dei risultati al termine della sessione Google Colab.
