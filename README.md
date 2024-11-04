Metrica

•LOC (pentru proiectul complet, adică pentru toate fişierele în mod colectiv);
•complexitatea ciclomatică şi cognitivă a metodelor evaluateExpression şi Calculate.


Masurarea dimensiunii programului software calculator-java pe baza numarului de linii de cod:
LOC: 215 (188 linii de cod - fisierul Calculator.java, 27 linii de cod - fisierul Start.java)
          21 linii de cod - fișierul License

Complexitatea ciclomatica - cat de greu e de testat un cod
            -   plugin-ul Code Metrics -IntelliJ Idea:
- evaluateExpression: 24
- Calculate: 56
           - instrumentul Codalize , în Visual Studio Code
- exista o funcție evaluateExpression pe a 28 a linie a codului pana la a 72 a  linie a codului, cu o complexitate ciclomatica de 12, are un totul de 33 linii de cod și 1 parametru
- exista o funcție Calculate pe a 74 a linie a codului pana la a 186 a  linie a codului, cu o complexitate ciclomatica de 12, are un totul de 77 linii de cod și 2 parametrii

Complexitatea cognitiva- cat de greu este de înțeles și mentinut un cod
         -  plugin-ul Code Complexity -IntelliJ Idea:

- evaluateExpression: very complex (175%)
- Calculate: very complex (287%)
         

Calculator.java
fisier: Calculator.java - numărul liniei de cod: 1 - observaţie: Codul folosește două clase pentru a crea liste, ceea ce este bine. Totuși, ar fi mai clar dacă am folosi importuri specifice pentru simbolurile pe care le folosim mai des.

fisier: Calculator.java - numărul liniei de cod: 4 - observaţie: Clasele utilitare nu trebuie să aibă constructori publici (Utility classes should not have public constructors)

fisier: Calculator.java - numărul liniei de cod:  6- observaţie: Variabila `finalResult` este statică. Asta înseamnă că toată lumea care utilizează clasa `Calculator` va avea aceeași valoare pentru `finalResult`. Acest lucru poate crea confuzie, mai ales dacă mai multe calcule sunt făcute în paralel.

fisier: Calculator.java - numărul liniei de cod: 8 - observaţie: Clasa `Operations` ar trebui să fie marcată ca finală (final), ceea ce ar însemna că nu o putem extinde. Acest lucru este util pentru claritate și securitate în cod.

fisier: Calculator.java - numărul liniei de cod: 13 - observaţie: Numele metodei `ToString` ar trebui să fie `toString` conform standardelor Java. Acest lucru ajută la menținerea unei convenții uniforme în întregul cod.

fisier: Calculator.java - numărul liniei de cod: 16 - observaţie: Metoda `ToString` nu include toate simbolurile de operatie necesare. Ar trebui să ne asigurăm că toate operațiile aritmetice sunt prezentate corect.

fisier: Calculator.java - numărul liniei de cod: 18 – observaţie: Numele metodelor trebuie să înceapă cu o literă minusculă (Method names should comply with a naming convention)

fisier: Calculator.java - numărul liniei de cod: 24 – observaţie: Numele metodelor trebuie să înceapă cu o literă minusculă (Method names should comply with a naming convention)

fisier: Calculator.java - numărul liniei de cod: 24 - observaţie: Dacă utilizatorul introduce o expresie goală sau care începe cu `+` sau `-`, codul poate da o eroare. Se recomanda o verificare suplimentară.

fisier: Calculator.java - numărul liniei de cod: 39 - observaţie: Când convertim texte în numere, trebuie să ne asigurăm că textul este valid. Ar trebui să gestionăm cazurile în care textul nu poate fi convertit în mod corespunzător, altfel programul ar putea sa nu funcționeze corect.

fisier: Calculator.java - numărul liniei de cod: 69 - observaţie: Metoda `Calculate` are mult cod repetat. Ar fi recomandată refactorizarea codului, adică să reducem codul duplicat, pentru a îmbunătăți lizibilitatea.

fisier: Calculator.java - numărul liniei de cod: 70 - observaţie: Variabilele locale nu trebuie să fie declarate ș i apoi imediat returnate sau aruncate (Local variables should not be declared and then immediately retutnrd or thrown)

fisier: Calculator.java - numărul liniei de cod: 74 - observaţie: Dacă avem deja toate operațiile necesare, nu trebuie să apelăm din nou metoda `Calculate`. Putem returna rezultatul direct, ceea ce face codul mai eficient.

fisier: Calculator.java - numărul liniei de cod: 74 – observaţie: Numele metodelor trebuie să înceapă cu o literă minusculă (Method names should comply with a naming convention)

fisier: Calculator.java - numărul liniei de cod: 93 - observaţie: Metoda `Calculate` folosește multe ramificări (if-uri) similare, care ar putea fi mutate într-o altă metodă pentru a face codul mai curat și mai ușor de întreținut.

fisier: Calculator.java - numărul liniei de cod: 113 - observaţie: Returnarea "ERROR" ca mesaj poate fi confuză. Ar trebui să folosim excepții pentru a explica mai clar problema și a oferi mesaj de eroare mai detaliat.

fisier: Calculator.java - numărul liniei de cod: 106 - observaţie: Lista pentru operații nu este foarte eficientă. O structură de date alternativă ar putea face gestionarea/stergerea operațiilor mai simplă.

fisier: Calculator.java - numărul liniei de cod: 106 - observaţie: Declarația de salt nu trebuie să fie redundantă.

 Concluzii fisier Calculator,java
1. Codul este funcțional, dar conține redundanțe și ar putea beneficia de restructurare.
2. Folosirea variabilelor statice nu este ideala deoarece poate crea confuzii atunci cand mai multi utilizatori lucreaza cu clasele.
3. Gestionarea erorilor ar putea fi imbunatatita, astfel incat utilizatorul sa primeasca mesaje mai clare despre problemele intampinate.
4. Gestionarea erorilor ar putea fi îmbunătățită prin utilizarea excepțiilor.
5. În general, validarea certitudinii datelor de intrare este insuficientă și ar trebui să fie o prioritate. Se doreste prevenirea erorilor si asigurarea unei functionari corecte a programului.



Start.java
fisier: Start.java - numărul liniei de cod: 1 - observaţie: Codul importă clasa Scanner din pachetul java.util, ceea ce este corect pentru a putea citi input de la utilizator.

fisier: Start.java - numărul liniei de cod: 3 - observaţie: Numele clasei Start sugerează un punct de început pentru aplicație, ceea ce este adecvat.

fisier: Start.java - numărul liniei de cod: 5 - observaţie: Definirea metodei main este corectă, aceasta fiind metoda de intrare a aplicației Java.

fisier: Start.java - numărul liniei de cod: 6 - observaţie: Declarația variabilei Expression ar trebui să fie mai clară, adică să se utilizeze o convenție de denumire care să sugereze că este o expresie de intrare.

fisier: Start.java - numărul liniei de cod: 8- observaţie: Ieșirile standard nu ar trebui să fie directe pentru a înregistra ceva (Standard outputs should not be directly to log anything)

fisier: Start.java - numărul liniei de cod: 9- observaţie: Declarația variabilei scanIn este bine realizată, dar inițializarea acesteia se face în interiorul buclei. Ar fi mai eficient să o inițializezi o singură dată, înainte de while.

fisier: Start.java - numărul liniei de cod: 11- observaţie: Utilizarea unei bucle while pentru a continua citirea input-ului până când utilizatorul introduce exit este o abordare corectă.

fisier: Start.java - numărul liniei de cod: 12- observaţie: Inițializarea unui nou Scanner la fiecare iterație a buclei nu este eficientă. Este recomandat să instanțiezi scanner-ul o singură dată, pentru a evita posibilele scurgeri de resurse.

fisier: Start.java - numărul liniei de cod: 16- observaţie: Închiderea scanner-ului în cazul în care utilizatorul a introdus exit este corectă, dar ar trebui menționat că metoda close() ar trebui apelată doar o singură dată dacă scanner-ul este instanțiat o singură dată.

fisier: Start.java - numărul liniei de cod: 17- observaţie: Modificarea valorii active pentru a ieși din buclă este o practică corectă.

fisier: Start.java - numărul liniei de cod: 19- observaţie: Afișarea rezultatelor returnate de metoda Run din clasa Calculator presupune că aceasta este definită și funcționează corect. Ar fi util să se facă o verificare asupra validității expresiei înainte de a o trimite către calculator.

fisier: Start.java - numărul liniei de cod: 19- observaţie: Ieșirile standard nu ar trebui să fie directe pentru a înregistra ceva (Standard outputs should not be directly to log anything)

fisier: Start.java - numărul liniei de cod: 22- observaţie:  Să te asiguri că sunt respectate bunele practici TDD (Test Driven Development) pentru a testa comportamentul aplicației pentru diferite expresii.

Codul programului Start,java este bine structurat, dar există câteva optimizări și îmbunătățiri care ar putea fi implementate pentru a crește eficiența și claritatea aplicației. Este recomandată verificarea metodele din clasa Calculator pentru a te asigura că funcționează conform așteptărilor. 
1. Initializarea Scannerului se face în fiecare iteratie a buclei while dar acesta nu e necesar, ar trebui să fie creat o singura data.
2. Gestionarea mai buna a exceptiilor ar avea un impact pozitiv. Folosiți un bloc gen try-catch sau o structura pentru a trata exceptiile.
3. Validarea expresiei introduse ar putea fi luata și ea în calcul. Structura gen „isValid Expression” ar putea fi folosita pentua a verifica structura expresiei.
4. Se recomanda  adaugarea de mesaje sulimentare despre ce tipuri de expresii pot fi introduse. Mesajul de utilizare este recomandat să fie mai explicativ.
5. Se mai pot face imbunatatiri pe structura și organizarea codului. 
6. Documentarea codului folosind comentariile ar putea fi ceva util pentru o înțelegere mai buna a codului. Se pot adauga comentarii pentru fiecare metoda și bucata de cod pentru a fi mai evidente anumite părți din cod.
