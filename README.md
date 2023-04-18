# Proactive Robot
Il progetto permette di eseguire il gioco "*Sequence Memory Game*" con l'assistenza del robot reale Furhat. Prima di iniziare a giocare, viene mostrato al partecipante un tutorial con le istruzioni di gioco su come ottenere punti e richiedere assistenza. Dopo che l'utente accetta di partecipare, gli si richiede di compilare prima un questionario demografico su età, sesso e livello di istruzione e poi il questionario Demographic Game Design. Infine, l'utente inizia a giocare con la possibilità di chiedere assistenza vocale al robot, se lo ritiene necessario, o di ricevere assistenza, se il robot Furhat lo ritiene necessario. Il gioco termina se l'utente preme il pulsante di fine o raggiunge il livello massimo. Successivamente, all'utente è richiesto di compilare un questionario post-interazione: prima il questionario sull'intelligenza sociale percepita, e poi sulla proattività del servizio robotico. Per ogni utente che ha finito di giocare, abbiamo raccolto in un file JSON le risposte ai questionari e la cronologia del gioco, mossa per mossa. 

## Dettagli
- Il file **third_main.py** contiene il main dell'applicativo web sviluppato con Flask, un modulo basato su Python che produce un'applicazione web utilizzando HTML, CSS e JavaScript. 
- La cartella *templates* contiene i file HTML, mentre la cartella *static* contiene i file CSS, JavaScript o le immagini utilizzate. 
- La cartella *json* contiene i file utilizzati per settare la lingua dell'applicativo (italiano/inglese).
- I file *svc_* rappresentano i classificatori SVM implementati per la predizione di quale assistenza fornire, quando, e con quale confidenza.
- I file *id_* rappresentano i diagrammi di influenza implementati per decidere quale assistenza fornire, quando, e con quale confidenza.
- Da installare: 
  - pip install flask (versione 2.2.2)
  - pip install pyagrum (0.22.8)
  - pip install furhat_remote_api
  - pip install scikit-learn (1.1.3)
  
- Per eseguire:
  python third_main.py
