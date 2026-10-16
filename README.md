# Jarvis CLI

Proiect individual în dezvoltare, aflat într-un stadiu exploratoriu. Scopul este construirea unui asistent accesibil din terminalul Linux, cu un CLI local în C/C++ și integrarea unor modele AI externe sau locale.

Acest repository documentează direcția proiectului. Nu conține încă o implementare publicată, iar funcțiile de mai jos sunt planificate, nu prezentate ca fiind funcționale.

## Obiectiv

Vreau să construiesc o interfață prin care să pot pune întrebări, să păstrez local istoricul întrebărilor și răspunsurilor și să aleg ce informații trimit modelului. Urmăresc să înțeleg legătura dintre o aplicație locală, fișierele sale și un serviciu AI.

## Arhitectură propusă

- CLI local în C/C++ pentru citirea comenzilor și afișarea răspunsurilor.
- Stocarea locală a conversațiilor, inițial într-un format simplu de fișier.
- Un modul separat pentru comunicarea cu modelul ales.
- Ulterior, căutarea în istoricul local pentru selectarea contextului relevant.

## Ce studiez

- Organizarea codului C/C++, structuri de date și biblioteca standard.
- Linux și Bash: redirecționări, pipe-uri, variabile de mediu și procese.
- Git pentru versiuni și colaborare: `status`, `diff`, `add`, `commit`, `branch`, `switch`, `merge`, `fetch`, `pull` și `push`.
- Integrarea modelelor AI și conceptele de context, tokeni și RAG.
- Separat, fundamente ML: mecanismul attention, arhitectura Transformer și backpropagation. Acestea sunt teme de studiu, nu implementări proprii declarate în proiect.

Comenzile Git gestionează istoricul codului; pipe-urile și redirecționările Bash conectează fluxurile de intrare și ieșire ale programelor. RAG presupune recuperarea unor informații relevante și furnizarea lor modelului, nu antrenarea acestuia.

## Costuri și evaluare

Reducerea costurilor este un obiectiv de verificat. Un CLI local nu reduce automat tokenii facturați de un API. Vreau să compar consumul cu și fără selectarea contextului, folosind aceleași întrebări, și să urmăresc și calitatea răspunsurilor. Cache-ul sau un model local pot fi direcții ulterioare; nu sunt funcții deja realizate.

## Primul prototip planificat

1. O comandă care primește o întrebare și o salvează local.
2. Integrarea unui model și tratarea erorilor de comunicare.
3. Salvarea și afișarea istoricului conversației.
4. Măsurarea consumului și experimentarea cu selectarea contextului.

Acesta este momentan un repository de documentație. Sursele și instrucțiunile de rulare vor fi adăugate odată cu primul prototip public. Cheile API vor fi păstrate în variabile de mediu, în afara repository-ului.
