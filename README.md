# ksiegowa.dysza.app — Księgowa

Moduł Dysza.App dla Pracowni Sushi. Pierwsza funkcja: **uzgodnienie faktur Księgowa ↔ FIRMINO** —
rejestr zakupów od księgowej (towary i koszty) porównany z dwoma plikami FIRMINO (zakupy towarów i koszty),
dokument po dokumencie, z wyjaśnieniami różnic.

Każdy plik wgrywa i zatwierdza jego strona: rejestr — Księgowa, zakupy towarów — Magazynier, koszty — Zarządzająca
(Architekt — każdy). Gdy trzy pliki są zatwierdzone, UZGODNIJ zapisuje uzgodnienie i dopiero wtedy widać wynik.

Strona nie zawiera żadnych danych. Po zalogowaniu (login z karty i PIN z manager.dysza.app) dane przychodzą z funkcji bazy
`ksiegowa_*`, które same pilnują dostępu i ról nadanych w managerze.
Pliki czyta przeglądarka; do bazy trafiają kolumny potrzebne do uzgodnienia, a dokumenty FIRMINO także wierszami.

Wersja 2026-11-12 19:25 · 629ae03
