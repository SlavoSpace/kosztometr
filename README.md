# kosztometr.dysza.app — Kosztometr

Moduł Dysza.App dla Pracowni Sushi. Karty w kolejności **F, P, A, OD, M, D, E, IS**:

- **F** — uzgodnienie faktur Księgowa ↔ FIRMINO: rejestr zakupów od księgowej (towary i koszty) porównany z dwoma plikami
  FIRMINO (zakupy towarów i koszty), dokument po dokumencie, z wyjaśnieniami różnic. Każdy plik wgrywa i zatwierdza jego
  strona: rejestr — Księgowa, zakupy towarów — Magazynier, koszty — Zarządzająca (Architekt — każdy). Gdy trzy pliki są
  zatwierdzone, UZGODNIJ zapisuje uzgodnienie i dopiero wtedy widać wynik.
- **P** podatki, **A** koszty administracyjne, **OD** obsługa długów, **M** marketing, **D** utrzymanie Dysza.App,
  **E** ekstra opłaty, **IS** wynagrodzenia właścicieli — wpis wiersz po wierszu (nazwa, data, okres, kwota),
  ZATWIERDŹ, KOREKTA (nowa wersja, poprzednia w historii), USUŃ; podsumowanie miesiąca w nagłówku karty.

Każdy widzi wszystkie kafle; karty bez dostępu są szare. Dostęp wynika z roli w module Kosztometr (manager.dysza.app).

Strona nie zawiera żadnych danych. Po zalogowaniu (login z karty i PIN z manager.dysza.app) dane przychodzą z funkcji bazy
`ksiegowa_*`, które same pilnują dostępu i ról nadanych w managerze.
Pliki czyta przeglądarka; do bazy trafiają kolumny potrzebne do uzgodnienia, a dokumenty FIRMINO także wierszami.

Wersja 2026-11-13 07:51 · 0b01b74
