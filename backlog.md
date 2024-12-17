User stories:


In calitate de ______(utilizator) sistemul trebuie sa __________(actiune) pentru _______(rezultat)

1.In calitate de CLIENT sistemul trebuie sa CREEZE UN TICKET pentru INITIERE PROBLEMA.
-- CREATE (INSERT IN DB)

2. In calitate de CLIENT sistemul trebuie sa PERMITA DETALIEREA UNEI PROBLEME pentru ACTUALIZAREA BAZEI DE DATE COMPLETA(rezultat). -- UPDATE (UPDATE IN DB -- PE BAZA ID AL TICKETULUI)

3.In calitate de CLIENT sistemul trebuie sa VERIFICE STAREA TICKETULUI pentru STATUS PROBLEMA. -- READ(SELECT IN DB -- PE BAZA ID AL TICKETULUI)

4.In calitate de CLIENT sistemul trebuie sa PERMITA EDITAREA UNUI TICKET pentru ACTUALIZAREA PROBLEMEI. -- UPDATE (UPDATE IN DB) -- PE BAZA ID AL TICKETULUI

5.In calitate de CLIENT sistemul trebuie sa PERMITA STERGEREA UNUI TICKET pentru ELIMINAREA PROBLEMEI. DELETE (DROP IN BD )

5BIS.In calitate de CLIENT sistemul trebuie sa PERMITA ELIMINAREA PROLEMEI UNUI TICKET pentru ELIMINAREA PROBLEMEI. UPDATE in BD

6.In calitate de CLIENT sistemul trebuie sa VIZUALIZAREA UNOR RAPOARTE pentru STATUS PROBLEMA. -- READ (SELECT IN BD CU JOIN)

MANAGER
1.In calitate de MANAGER(utilizator) sistemul trebuie sa OFERE O LISTA DE TICKETE(actiune) pentru VIZUALIZARE PROBLEME(rezultat). -- READ(SELECT IN DB)

2.In calitate de MANAGER (utilizator) sistemul trebuie sa POSIBILITATEA DE VIZUALIZARE A UNUI TICKET(actiune) pentru VIZUALIZARE PROBLEME(rezultat). -- READ(SELECT IN DB)

3. In calitate de MANAGER(utilizator) sistemul trebuie sa PERMITA ACTUALIZAREA STATUS-ULUI - DONE (actiune) pentru VIZUALIZARE PROBLEME(rezultat) -- UPDATE (UPDATE IN DB)

4. In calitate de ______(utilizator) sistemul trebuie sa ACTUALIZAREA INFORMATIILOR PRIMITE(actiune) pentru VIZUALIZAREA PROBLEME(rezultat)-- UPDATE (UPDATE IN DB)


CRUD(CREATE READ UPDATE DELETE) - BAZA DE DATE 
HTTP(POST GET PUT DELETE)

II, Crearea backlogului
$$ vb despre serviciu web -- componenta de server care raspunde la solicitarea clientului

http: requesturi - responses
	-	 requests: GET (cer o resursa)
	- 				POST (adauga o resursa sau date)
					PUT (actualizeaza o resursa)
					DELETE
					PATCH = PUT
1. o functie in C# care raspunde la un request de top POST pentur U1 (INSERT into db cu date provenite din request (POST)
2. o functie in C# care raspunde la un  request de tip PUT pentru U2 -- UPDATE into DB cu datele provenite din request
3. o functie in C# care raspunde la un  request de tip GET pentru U3 -- SELECT ticket unde ticketID - val primita in request  [ ] select ticket unde ticketOwner= numeClient primit in reqest
4. o functie in C# care raspunde la un  request de tip PUT pentru U4 -- UPDATE ticket info unde ticketID - val primita in request si info este primit in request
5. o funcție în C# care răspunde la un request de tip DELETE pentru U5: DELETE ticket pe baza ID-ului.
6. o funcție în C# care răspunde la un request de tip GET pentru U6: SELECT rapoarte detaliate folosind JOIN.

min 2* requesturi/student
