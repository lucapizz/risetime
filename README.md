# risetime
formulas memo


il tempo di salita è quello impiegato per passare dal 10% al 90% del livello di un segnale.

la lunghezza d'onda è l'inverso del tempo di salita.

la velocià di propagazione di un segnale elettrico in un cavo coassiale vale circa il 66% della
velocità della luce ossia 300000000 * 0,66 = 200000000 m/s circa.

in linea di massima la lunghezza di una linea di trasmissione per non creare riflessioni dovrebbe
essere inferiore a un quarto (1/4) della lunghezza d'onda del segnale.

lunghezzamax = 200000000 * t / 4

ad esempio se ho un tempo di salita di 0,2 us posso calcolare la lunghezza massima
pari a

50000000 * 0,0000002 = 10 metri

oltre la quale ho bisogno di terminare la linea.

Quanto suddetto è una stima, infatti possiamo anche stimare la distanza con un modo diverso.

Usando la frequenza si ottiene

distanza = 200000000 / (2 * 2 * pigreco * f)

ad esempio con 0,2 us abbiamo una banda di 0,35 / 0,2 = 1,75MHz

e poi
distanza = 200000000 / (4 pigreco 1750000) = 9,09 metri

che in effetti è piuttosto simile ai 10 metri della stima precedente.

#
# terminazione linee di trasmissione
La R di terminazione deve coincidere con l'impedenza caratteristica della linea
che si calcola dall'induttanza a dalla capacità distribuite.

La formula è R = radice di (L[Henry]/ C[Farad])

infatti
<br>Henry = V * s / A
<br>Farad = A * s / V
<br> H/C = (Vs/A) / (As/V) = V/A
