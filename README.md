314 CA Pinzaru Mihaela Tema2
Backend:
Am folosit o lista dublu inlantuira de stringuri.
Pentru UNDO si REDO am folosit 2 array-uri de liste de stringuri.
In undo, la ADD, CUT copiez textul curent in array. Daca se executa un UNDO, textul curent pe ecran, este pun in arrayul de redo.
Redo se goleste de fiecare dara cand adaug un cuvant sau fac paste.
In sumaPoz memorez pentru fiecare cuvant pozitia pe care incepe in cadrul textului.
Il folosesc pentru a stabili, mai usor, pozitiile de start / stop pentru diferite metode.
La fiecare modificare a textului de pe ecran, se actualizeaza si sumaPoz.
Fata de metodele de baza, am adaugat alte 3 ajutatoare.
Alte detalii de implementare:
 		ostringstream ss;
        ss << x->value;
        Afisare += ss.str();

Aceasta parte de cod o folosesc pentru a convertii de la un tip de date T la string.
