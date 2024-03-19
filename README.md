# EV3Python2024

EV3Python2024/
└── TestRemote
    ├── README.md
    ├── ev3RemoteAssistant.py
    ├── ev3RemoteCommander.py
    ├── testAvgTime.py
    ├── testTouchSensor.py
    └── testUSonicSensor.py

Nella cartella TestRemote c'è il test per connettere i due EV3 in remoto con il cavetto USB. I passaggi necessari sono:
1. Accendere i due EV3 in ev3dev
2. Connettere i due EV3 con il cavetto USB (il principale sarà quello connesso con l'USB A, quello secondario con il mini USB)
3. Attivare il gadgeting sul secondario
    1.  Wireless and Networks
    2.  Tethering
    3.  Attivare il gadget, apparirà un ip in alto a sinistra
    4.  Se l'ip scompare, disattivare il gadget e attivare la modalità offline, poi riattivare il gadget. Va fatto anche quando si disconnette il cavetto
4. Avviare  ev3RemoteAssistant.py sul secondario
5. Avviare il programma sul primario, che deve avere all'interno anche ev3RemoteCommander.py
