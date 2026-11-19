# IWA projekt – katalog pjesama i medijskih kuća

Studentski projekt iz kolegija *Izgradnja web aplikacija* (prijediplomski studij, FOI, 2022.).

## Funkcionalnosti
- PHP + MySQL, bez frameworka
- četiri uloge: administrator, moderator, registrirani i anonimni korisnik
- unos i uređivanje pjesama, medijskih kuća i korisnika
- zahtjevi za kupnju pjesama, lajkovi

## Poznati nedostaci
- **SQL injection** – upiti se grade spajanjem stringova → `mysqli_prepare` + `bind_param`
- **lozinke u čistom tekstu** → `password_hash()` / `password_verify()`
- **nema zaštite od XSS-a** → `htmlspecialchars()` pri ispisu
- konfiguracija baze u kodu → varijable okruženja
