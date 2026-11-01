# Złota Podkowa

Quiz o koniach w przeglądarce na telefon. Ma trzy poziomy trudności: Źrebak, Galop i Grand Prix. Za każdą dobrą odpowiedź gracz dostaje podkowy, a w Stajni wymienia je na karty ras z ciekawostkami.

Gra nie potrzebuje instalacji ani serwera. Składa się z pliku `index.html`, pliku `credits.js` (autorzy zdjęć) i folderu `img` ze zdjęciami.

Postęp (podkowy, rozetki, odkryte konie) zapisuje się w przeglądarce na danym telefonie.

## Publikacja na GitHub Pages (przez przeglądarkę)

1. Zaloguj się na https://github.com i kliknij **New repository**.
2. Nazwij repozytorium, na przykład `zlota-podkowa`, ustaw je jako **Public** i kliknij **Create repository**.
3. Na stronie repozytorium kliknij **uploading an existing file**. Przeciągnij całą zawartość folderu `github-pages`: pliki `index.html`, `credits.js`, `README.md` oraz folder `img` (razem ze zdjęciami). Kliknij **Commit changes**.
4. Przejdź do **Settings → Pages**. W sekcji **Build and deployment** wybierz **Source: Deploy from a branch** oraz **Branch: `main`** i folder **`/ (root)`**, a następnie kliknij **Save**.
5. Po 1–2 minutach gra będzie dostępna pod adresem:
   `https://<twoja-nazwa-użytkownika>.github.io/zlota-podkowa/`

Na telefonie możesz wybrać „Dodaj do ekranu głównego”. Gra otworzy się wtedy jak aplikacja.

## Aktualizacja

Źródłem gry jest plik `../zlota-podkowa.html`, czyli wersja dla claude.ai. Po każdej zmianie zbuduj stronę od nowa:

```bash
node build-pages.mjs
```

Potem wrzuć nowy `github-pages/index.html` do repozytorium: otwórz plik na GitHubie, kliknij ikonę ołówka albo **Add file → Upload files** i zatwierdź zmianę.

## Zdjęcia

Wszystkie zdjęcia pochodzą z Wikimedia Commons i są na wolnych licencjach (CC BY, CC BY-SA, CC0 lub domena publiczna). Lista autorów jest w grze, w zakładce **Zdjęcia**. Licencje CC BY i CC BY-SA wymagają podania autora, dlatego ta zakładka musi zostać w grze.
