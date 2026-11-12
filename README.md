# ksiegowa.dysza.app — Księgowa

Moduł Dysza.App dla Pracowni Sushi. Pierwsza funkcja: **uzgodnienie faktur Księgowa ↔ FIRMINO** —
rejestr zakupów od księgowej porównany z dokumentami zakupu w FIRMINO, dokument po dokumencie, z wyjaśnieniami różnic.

Strona nie zawiera żadnych danych. Po zalogowaniu (login z karty i PIN z manager.dysza.app) dane przychodzą z funkcji bazy
`ksiegowa_*`, które same pilnują dostępu: Architekt i osoby z rolą „Księgowa” nadaną w managerze.
Pliki czyta przeglądarka; do bazy trafiają tylko kolumny potrzebne do uzgodnienia.

Wersja 2026-11-12 15:08 · de6cf0b
