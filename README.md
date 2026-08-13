# Studio Piegus — strona WWW

Statyczna strona (czysty HTML/CSS/JS, bez backendu). Wszystkie zdjęcia są osadzone
w plikach, więc nie ma osobnego folderu z grafiką — każdy plik `.html` jest samowystarczalny.

## Pliki

| Plik | Rola |
|------|------|
| `index.html` | **Strona startowa** (splash „Budujemy dla Was naszą stronę") z bramką hasła |
| `studio-piegus-home-foto.html` | Właściwa strona główna |
| `zajecia.html` | Zajęcia |
| `cennik.html` | Cennik |
| `voucher.html` | Voucher podarunkowy |
| `dla-firm.html` | Warsztaty dla firm |
| `kontakt.html` | Kontakt |

Linki między stronami są względne — działają zarówno w katalogu głównym domeny,
jak i pod ścieżką projektu (`https://uzytkownik.github.io/repo/`).

## Hasło (admin access)

Wejście do serwisu chroni proste, przeglądarkowe okienko na `index.html`.
Hasło: **KHMC**. Po jego wpisaniu strona zapisuje znacznik sesji i wpuszcza dalej;
pozostałe podstrony przy braku znacznika zawracają na `index.html`.

> Uwaga: to zabezpieczenie „coming soon" po stronie przeglądarki — wystarczające,
> by ukryć stronę przed przypadkowym gościem, ale **nie jest** twardą ochroną
> (pliki są publicznie dostępne pod swoimi adresami). Mocniejsze zabezpieczenie
> wymaga hostingu z autoryzacją serwerową.

## Publikacja na GitHub Pages

1. Załóż repozytorium na GitHub (np. `studio-piegus`).
2. Wgraj wszystkie pliki `.html` (oraz ten `README.md`) do **głównego katalogu** repo
   — przez stronę GitHub „Add file → Upload files", albo `git push`.
3. W repo: **Settings → Pages**.
4. W sekcji „Build and deployment" ustaw **Source: Deploy from a branch**,
   Branch: **main** (lub `master`), folder: **/ (root)**. Zapisz.
5. Po chwili (1–2 min) pojawi się adres, np. `https://twoj-login.github.io/studio-piegus/`.
   Otworzy się `index.html` (splash).

### Własna domena (studiopiegus.pl)
W **Settings → Pages → Custom domain** wpisz domenę i skonfiguruj rekordy DNS
u rejestratora (GitHub pokaże wymagane wartości). Zalecane: włącz „Enforce HTTPS".

## Edycja treści
Teksty są dwujęzyczne (atrybuty `data-pl` / `data-en`, przełącznik PL/EN w menu).
Aby zmienić tekst, edytuj **zarówno** widoczną treść, **jak i** odpowiedni atrybut
`data-pl` / `data-en` w danym elemencie.

## Do dokończenia (opcjonalnie)
- Żywa mapa na `kontakt.html` (teraz jest klikalna karta lokalizacji — patrz kod sekcji „Dojazd").
- Realne ceny/harmonogram na `zajecia.html` (miejscami dane przykładowe).
- Potwierdzenie adresu e-mail (obecnie `kontakt@studiopiegus.pl`) i podpięcie formularza kontaktowego do skrzynki/CRM.
- Dla produkcji warto wynieść zdjęcia do osobnego folderu `/img` i podłączyć lazy-loading (pliki będą lżejsze).
