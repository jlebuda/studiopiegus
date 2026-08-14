# Studio Piegus — strona WWW

Statyczna strona (HTML/CSS/JS, bez backendu). Zdjęcia są osadzone w plikach — każdy `.html` jest samowystarczalny.

## Pliki
- `index.html` — **strona główna** (wejście serwisu)
- `zajecia.html` — Zajęcia
- `cennik.html` — Cennik
- `voucher.html` — Voucher podarunkowy
- `dla-firm.html` — Warsztaty dla firm
- `kontakt.html` — Kontakt
- `studio-piegus-home-foto.html` — przekierowanie na `index.html` (dawna nazwa strony głównej; zostaje, by stare linki działały)

Linki między stronami są względne — działają w katalogu głównym domeny i pod ścieżką `…github.io/repo/`.

## Publikacja / commit na GitHub
1. Wgraj wszystkie pliki do głównego katalogu repo (Add file → Upload files, albo `git add . && git commit && git push`).
2. Settings → Pages → Deploy from a branch → main → /(root).
3. Strona: `https://<login>.github.io/<repo>/` (otworzy się `index.html`).

## Edycja treści
Dwujęzyczność: atrybuty `data-pl` / `data-en` + przełącznik PL/EN. Zmieniając tekst, edytuj i widoczną treść, i odpowiedni atrybut.
