HTTP/3 utilizza QUIC come protocollo di trasporto, quindi gira sopra UDP anziché TCP come nelle versioni precedenti di HTTP. 
Grazie a QUIC, la connessione HTTP/3 può essere stabilita in 0-1 round-trip se il client si è già collegato in precedenza al server, riducendo la latenza rispetto a HTTP/2.
Se si verifica una perdita di pacchetti durante una sessione HTTP/3, QUIC ritrasmette solo i pacchetti mancanti senza bloccare tutte le altre richieste, permettendo alle altre stream di continuare a funzionare fluidamente, superando il problema di “head-of-line blocking” presente in TCP.
