# Pasi de implementare

## 1. Acomodarea cu tematica 
- intelegere enunt si descarcare biblioteci necesare

## 2. Schematic
- am incercat sa fie cat mai asemanator cu imaginea pdf pusa pe ocw

## 3. PCB
- la generarea pcb-ului pe baza schematicului, piesele erau deja puse. 
- singurul lucru care a fost de modificat aici a fost forma butoanelor si a adaptorului. 
- am inceput cu butoanele caci au fost mai simplu. am incercat sa ma tin cat mai aproape de dimensiunile din datasheet-uri. ca sa am dimensiunile convenabile am setat gridul la 0.1 mm pentru o precizie sporita.
- acelasi lucru si la adaptorul lcd, unde am facut cateva calcule spre aflarea tuturor dimensiunilor necesare. aici a trebuit sa modific schematicul adaptorului, pinii MP1 si MP2 nefiind necesari.

## 4. Pregatire pentru "asamblare"
- am grupat componentele dupa cum erau grupate in schematic, pentru o asezare mai usoara pe planul ceasului.
- am folosit mirror pentru a pune componentele de pe bottom conform cerintei, asta inca din acest punct, pentru a vizualiza mai usor planurile

## 5. Forma ceas
- apoi am creat forma ceasului, la fel, cu multe ajustari, dupa dimensiuni (am incercat sa fac sa intre in carcasa).

## 6. GND
- am creat planul de masa cu polygon pour si linie care se poate curba, incercand cu greu sa tin conturul ceasului. copy-paste pentru bottom, selectat impruna si redenumit (legat) la GND.

## 7. Punere elemente
- am pus toate elementele in interiorul formei de ceas, incercand pe cat posibil sa pastrez restrictiile (condensatoarele fiecarui tip de piesa cat mai aproape de pini) (evebtual asa si la rezistente). 
- am pus antena pe mijloc, la margini sd-reader-ul si usb-ul, pe langa si celelalte piese, la fel, am incercat sa nu pun nor-flash sub antena pe planul de desesubt.

## 8. Finisare PCB
- am taiat forma de ceas, stergand pcb-ul, ramanand numai cercul ceasului cu planurile de masa si piesele.

## 9. Rutare
- am trecut de data aceasta la auto-route, dupa lungi incercari de a ruta manual si a reaseza piesele pentru o rutare manuala mai usoara.
- si la auto-route a trebuit sa rearanjez piesele de cateva ori (respectand restrictiile) pentru o eficienta mai sportita (88-100% routing).
chiar si asa am avut 5 air-wires.

## 10. Ajustare dupa auto-route
- am inlocuit grosimea firelor de putere (GND, VIBE-OUT, VBUS, VUSB, 3V3 etc). in acest proces mi-au aparut multe overlap-uri.
- acest lucru l-am facut ori schimbat grosmiea firului din proprieteti, ori stergandu-l si trasandu-l la loc, acolo unde am avut loc.
- pe anumite portiuni am combinatie de 0.127 - 0.3 mm

## 11. Altele
- am un overlap la un footprint care nu a fost realizat sau modificat de mine.
