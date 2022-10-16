# ICONIC GAMES
  
## PROBLEMA 1

Durata implementarii: 1.5h
Rezolvare: Sortarea perechilor de cuvinte in functie de gradul acestora.
Functia **compute_grade** primeste ca parametrii doua cuvinte si verifica daca sunt anagrame (functia ###   **is_anagram**), iar in caz contrar returneaza raportul dintre rezultat si lungimea totala a sirurilor.

##  PROBLEMA 2

Durata implementarii: 3h
Rezolvare: 
Am construit o matrice ('sah') in care elementele respective sunt 1, iar restul sunt 0. 
Am parcurs matricea pentru a gasi valorile de 1. Pentru fiecare, am apelat functiile search_dp si search_ds care returneaza numarul de nebuni cu care se ataca pe diagonala paralela cu cea principala si, respectiv, cu cea secundara pe care se afla nebunul.
Am salvat in variabila 'per' suma acestor valori, pe care am injumatatit-o deoarece fiecare nebun a fost gasit de 2 ori. Astfel, in variabila 'per' este numarul perechilor de nebuni care se ataca.
Pentru cea de-a doua parte a problemei, in cazul in care numarul de perechi este diferit de 1, se afiseaza "NU". Altfel, am parcurs din nou matricea, iar pentru fiecare valoare am verificat:
-daca este egala cu 1; 
-daca nebunul face parte din perechea gasita (prin verificarea pe diagonale prin cele doua functii);
-daca se poate muta astfel incat sa nu se atace cu niciun nebun (functia move);
In cazul in care sunt indeplinite conditiile, se afiseaza "DA".

##  PROBLEMA 3

Durata implementarii: 6h
Rezolvare: 
Am facut cate o functie pentru fiecare miscare, care modifica matricea cubului rubik. Fiecare dintre ele include rotirea fetei respective si mutarea culorilor de pe marginea fetei.

##  PROBLEMA 4

Durata implementarii: 2h
Rezolvare: 
Am transformat ficare numar citit intr-un sir binar si le-am salvat in vectorul de cuvinte 'AC', pe cate o linie.
Pentru fiecare caracter din AC, am salvat corespondentul intreg in matricea 'A'.
Am calculat A^2 ('A2') - functia inmultire. Am calculat transpusa lui A ('T') - functia transpusa. Am calculat A*(A^t) ('AT') - functia inmultire.
Am calculat scorurile pentru fiecare matrice (functie sum_X_0) si maximul dintre ele.
In functie de scorul maxim, am salvat intr-o matrice intregii corespunzatori fiecarui caracter, pentru a putea folosi functia bin_to_dec, pentru a afisa numerele in baza 10.