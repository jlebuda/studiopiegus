# Studio Piegus — strona WWW

Statyczna strona (czysty HTML/CSS/JS, bez backendu). Wszystkie zdjęcia są osadzone
w plikach — nie ma osobnego folderu z grafiką, każdy plik `.html` jest samowystarczalny.

## Pliki

| Plik | Rola |
|------|------|
| `index.html` | Wejście — **przekierowuje** na stronę główną |
| `studio-piegus-home-foto.html` | Strona główna |
| `zajecia.html` | Zajęcia |
| `cennik.html` | Cennik |
| `voucher.html` | Voucher podarunkowy |
| `dla-firm.html` | Warsztaty dla firm |
| `kontakt.html` | Kontakt |

Linki między stronami są względne — działają zarówno w katalogu głównym domeny,
jak i pod ścieżką projektu (`https://uzytkownik.github.io/repo/`).

> Uwaga: bramka hasła („coming soon") została usunięta — strona otwiera się od razu.

## Publikacja na GitHub Pages

1. Wgraj wszystkie pliki `.html` (i ten `README.md`) do **głównego katalogu** repo
   (przez „Add file → Upload files", albo `git add . && git commit && git push`).
2. **Settings → Pages** → Source: **Deploy from a branch**, Branch: **main**, folder: **/ (root)** → Save.
3. Po chwili strona będzie pod `https://<login>.github.io/<repo>/` (otworzy się strona główna).

### Własna domena (studiopiegus.pl)
Settings → Pages → Custom domain + rekordy DNS u rejestratora; zaznacz „Enforce HTTPS".

## Edycja treści
Teksty są dwujęzyczne (atrybuty `data-pl` / `data-en`, przełącznik PL/EN w menu).
Zmieniając tekst, edytuj **zarówno** widoczną treść, **jak i** odpowiedni atrybut
`data-pl` / `data-en` w danym elemencie.

## Do potwierdzenia / dokończenia (opcjonalnie)
- Realne ceny na `zajecia.html` przy zajęciach dla dorosłych (miejscami dane przykładowe).
- Adres e-mail (obecnie `kontakt@studiopiegus.pl`) i podpięcie formularza kontaktowego do skrzynki/CRM.
- Żywa mapa Google na `kontakt.html` (teraz jest klikalna karta lokalizacji — patrz sekcja „Dojazd").
- Dla produkcji warto wynieść zdjęcia do osobnego folderu `/img` + lazy-loading (lżejsze pliki).
