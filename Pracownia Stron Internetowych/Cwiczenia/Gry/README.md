Zadanie 4: Gra „Refleks”

Wykonaj stronę internetową z grą sprawdzającą refleks użytkownika.

Po kliknięciu przycisku Start program powinien rozpocząć grę i wyświetlić komunikat:

Czekaj...

Po losowym czasie od 2 do 5 sekund program powinien zmienić komunikat na:

Kliknij teraz!

Użytkownik musi jak najszybciej kliknąć odpowiedni przycisk lub pole gry. Program powinien zmierzyć czas reakcji użytkownika i wyświetlić wynik w milisekundach.

Jeżeli użytkownik kliknie za wcześnie, program powinien wyświetlić komunikat:

Za wcześnie!
Wymagania HTML

Strona powinna zawierać:

Nagłówek strony:
Gra Refleks
Krótki opis gry, np.:
Kliknij przycisk Start, poczekaj na komunikat i kliknij jak najszybciej.
Przycisk:
Start
Przycisk lub pole do kliknięcia:
Kliknij
Miejsce na komunikat, np.:
Czekaj...
Kliknij teraz!
Za wcześnie!
Miejsce na wynik reakcji, np.:
Twój czas reakcji: ... ms
Przycisk nie może odświeżać strony.
Wymagania JavaScript

Po kliknięciu przycisku Start program powinien:

Wyczyścić poprzedni wynik.
Wyświetlić komunikat:
Czekaj...
Ustawić zmienną informującą, że użytkownik nie może jeszcze kliknąć.
Wylosować czas oczekiwania od 2 do 5 sekund.

Podpowiedź:

let czasLosowy = Math.floor(Math.random() \* 3000) + 2000;
Po upływie wylosowanego czasu wyświetlić komunikat:
Kliknij teraz!
Zapisać aktualny czas rozpoczęcia reakcji.

Podpowiedź:

let startCzasu = Date.now();
Pozwolić użytkownikowi kliknąć.
Po kliknięciu pola lub przycisku „Kliknij”

Program powinien:

Sprawdzić, czy użytkownik kliknął za wcześnie.

Jeżeli kliknął za wcześnie, wyświetl:

Za wcześnie!
Jeżeli użytkownik kliknął po komunikacie Kliknij teraz!, program powinien obliczyć czas reakcji:
let czasReakcji = Date.now() - startCzasu;
Wyświetlić wynik:
Twój czas reakcji: ... ms
Zablokować dalsze klikanie do rozpoczęcia nowej gry.
Przykład działania

Użytkownik klika:

Start

Program wyświetla:

Czekaj...

Po losowym czasie program wyświetla:

Kliknij teraz!

Użytkownik klika przycisk.

Program wyświetla:

Twój czas reakcji: 342 ms

Jeżeli użytkownik kliknie przed komunikatem Kliknij teraz!, program wyświetla:

Za wcześnie!
