# MOU. — cukrářský ateliér (DEMO 2030)

Kompletní responzivní demo web cukrárny vytvořený pomocí čistého HTML, CSS a JavaScriptu. Bez frameworků, instalace, databáze a externích odkazů na obrázky.

## Obsah složky

- `index.html` — struktura webu, sekce a modální okna.
- `styles.css` — design, animace, responzivita.
- `app.js` — produkty, ceny, interaktivní katalog, demo košík, konfigurátor dortu a galerie.
- `assets/images/` — **21 lokálních WebP obrázků**. V projektu nejsou potřebné externí fotobanky.
- `assets/favicon.svg` — vlastní ikona záložky.

## Jak web spustit

Otevřete `index.html` v prohlížeči. Pro vývoj lze také použít VS Code a Live Server. Web funguje z relativních cest, takže je vhodný na GitHub Pages.

## GitHub Pages

1. Založte samostatný repozitář, například `mou-cukrarna-demo`.
2. Nahrajte **obsah této složky** do kořene repozitáře (soubor `index.html`, `styles.css`, `app.js` i celou podsložku `assets`).
3. V repozitáři nastavte **Settings → Pages → Deploy from a branch → main / (root)**.
4. Po publikaci web najdete na GitHub Pages daného repozitáře.

Pozor: Pokud jsou obrázky v podsložce `assets/images`, zachovejte jejich názvy i velikost písmen; GitHub Pages je rozlišuje.

## Úprava nabídky a cen

V souboru `app.js` najděte pole `PRODUCTS`. Každá položka má `name`, `description`, `price`, `category`, `image`. Název obrázku je bez přípony `.webp`. Po přidání další fotografie do `assets/images` ji lze hned přiřadit novému produktu; galerie se tvoří automaticky.

Pro změnu ceny nebo varianty dortu upravte `cakeOptions` v `app.js`.

Pokud přidáte produkty, změňte také text „20“ ve statickém nadpisu a filtru ceníku v `index.html` (nebo jej napojte na délku pole `PRODUCTS`).

## Co opravdu funguje

- Responzivní navigace a mobilní menu.
- Katalog s filtrováním a zobrazením celého ceníku.
- Přidávání a odebírání produktů, množství a součet ceny.
- Uchování výběru přes `localStorage` tam, kde to prohlížeč dovoluje.
- Konfigurátor dortu s přepočtem ceny a přidáním do výběru.
- Galerie s 21 obrázky, zvětšením a klávesami (Escape, šipky).
- Rozbalovací FAQ, animace při scrollování, indikátor posouvání.
- Vygenerování a zkopírování textového souhrnu výběru.

## Důležitá demo omezení

**MOU. není skutečná cukrárna.** Produkty a ceny jsou pouze ukázkové; obrázky byly vytvořeny pro tento koncept. Košík, konfigurátor ani souhrn **neodesílají objednávku** a nepřijímají platby. Pro skutečný provoz by bylo nutné doplnit autentické informace, kontakty, alergeny, obchodní podmínky a zabezpečený objednávkový systém.

Projekt nevyžaduje instalaci závislostí ani internet pro obrázky, CSS nebo JavaScript.
