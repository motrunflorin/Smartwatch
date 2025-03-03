- pentru traseele de putere (3V3) am respectat dimensiunea de 0.3 mm, 
  iar restul au 0.127 mm;

!! rectificare: din cauza ca nu mi s au salvat fisierele cum trebuie, am avut erori
 de sync intre schematics si pcb, si a trebuit sa sterg traseele de 3v3 si sa le modific
 cu width 0.127 mm;

- test padurile nu le-am putut grupa in forma regulata, iar test pad-ul TX nu
  se afla in grupare, pentru a-l putea lega la pinul corespunzator;
  (initial am gandit asezarea test pad-urilor ca 3 grupari distincte,
   amplasate cat mai strategic in apropierea de pinii la care trebuiau conectati,
   pentru a avea trasee cat mai optime);

- condensatoarele de decuplare de 100 nF au fost amplasate cat mai aproape de pinii
  de alimentare;

- componentele principale au fost amplasate conform specificatilor din documentul cu
  dimenisuni, cu erori aproape inexistente, de ordinul 10^-3 mm;

- antena modulului ESP32 a fost amplasata spre exteriorul PCB-ului, iar PCB-ul a
  fost decupat cat mai exact sub antena;

- test pad urile, soclul pentru cardul sd, a conectorului lcd si a circuitului
  NOR Flash au fost puse pe Top;

- footprint-urile pentru butoane si conectorul display LCD au fost realizate conform
  datasheet-ului;

- am incercat pe cat posibil sa pastrez toate componentele din gruparile din Schematics laolalta, 
cum ar fi gruparea de diode de exemplu;

- de asemenea am incercat sa pozitionez piesele cat mai aprope de corespondentul lor ca legatura
  din Schematics in PCB, cum ar fi de exemplu rezistorul R1-USB de modului USB4110-GF-A;


- ERORI: rezistentele R11, R9 nu au fost conectate intrucat nu am putut gasi traseu 
  viabil;
 
- silkscreen a fost facut pentru test pad-uri cu width de 0.4mm
	