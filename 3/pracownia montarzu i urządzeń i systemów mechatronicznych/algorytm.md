             +--------------------+
             |        1           |  <-- Krok początkowy (siłownik wsunięty, żarówka zgaszona, obudowa zamknięta)
             |       STOP         |  (H1 = OFF, Y1 = OFF, Y2 = ON (domyślnie wsunięty))
             |                    |  (Warunek dla Y2=ON: tylko w stanie wsuniętym i dla utrzymania tego stanu;
             |                    |   w kroku 2 i kolejnych Y2 jest dezaktywowane w celu wysunięcia)
             +--------------------+
                       |
                       | S1 AND B3   <-- Przejście: Przycisk startu i obudowa zamknięta
                       |             [cite: 80, 83]
             +--------------------+
             |        2           |  <-- Krok: Siłownik wysuwa się, żarówka świeci (sygnalizacja pracy)
             |      PRACA1        |  (Y1 = ON, Y2 = OFF, H1 = ON) [cite: 80]
             |      D1: H1 (N)    |
             |      D2: Y1 (N)    |
             |      D3: T1 (D t=3s)| (Timer odlicza 3s, po których siłownik ma się wsunąć) [cite: 80]
             +--------------------+
                       |
                       | B1 AND T1   <-- Przejście: Siłownik wysunięty (B1) i upłynęły 3 sekundy (T1) [cite: 80]
                       |
             +--------------------+
             |        3           |  <-- Krok: Siłownik wsuwa się
             |      PRACA2        |  (Y1 = OFF, Y2 = ON)
             |      D4: Y2 (N)    |
             +--------------------+
                       |
                       | B2          <-- Przejście: Siłownik wsunięty (B2) [cite: 81]
                       |
             +--------------------+   +-------------------------------------------------------------+
             |        4           |<--|  Powrót do kroku 2 (kontynuacja cyklu) - domyślnie cykl trwa bez przerwy [cite: 81]
             |     PRACA3         |   |
             +--------------------+   +-------------------------------------------------------------+
                       |  <-- Brak warunku, automatyczny powrót do kroku 2 po zakończeniu akcji w kroku 3
                       |
                       +--------------------+
                       |                   |
                       |                   | S2 AND B2  <-- Przejście: Przycisk S2 wciśnięty i siłownik wsunięty (przed wejściem w stan STOP) [cite: 81]
                       |                   |
                       +-------------------------------------------------+
                       |                                                 |
                       |                                                 |
             +--------------------+  <-- Krok: Koniec pracy (siłownik wsunął się, żarówka zgasła)
             |        1           |   (powrót do kroku początkowego, H1 = OFF) [cite: 81]
             |       STOP         |
             +--------------------+

                       ^
                       |
                       | (B3 = 0)  <-- Przejście z dowolnego aktywnego kroku (2, 3, 4) do stanu AWARYJNEGO, jeśli obudowa otwarta [cite: 82]
                       |             (To jest przykład przejścia awaryjnego, które przerywa normalną sekwencję)
                       |
             +--------------------+
             |        5           |  <-- Krok: Awaryjne wyłączenie (obudowa otwarta)
             |     AWARYJNY       |  (Y1 = OFF, Y2 = ON, H1 = MIGAJĄCA) [cite: 82]
             |     D5: Y2 (N)     |
             |     D6: H1 (S)     |  <-- (H1 = MIGAJĄCA) - oznacza specjalną akcję migania
             +--------------------+
                       |
                       | B3 AND S1   <-- Przejście: Obudowa zamknięta i przycisk S1 wciśnięty (aby ponownie uruchomić układ) [cite: 83]
                       |             (lub po prostu B3=1 dla powrotu do stanu "STOP" po zamknięciu obudowy)
                       |
             +--------------------+
             |        1           |  <-- Powrót do kroku początkowego (STOP)
             |       STOP         |
             +--------------------+
