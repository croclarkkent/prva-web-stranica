# Web stranica — izrada i montaža kuhinja po mjeri

U repozitoriju su **dvije verzije dizajna**.

## Verzija 1 — u glavnoj mapi

Topla paleta (gotovo crna, krem, mjed). Svih pet stranica:

| Datoteka | Stranica |
|---|---|
| `index.html` | Naslovnica |
| `onama.html` | O nama |
| `projekti.html` | Projekti (Prije / Poslije) |
| `galerija.html` | Galerija fotografija |
| `kontakt.html` | Kontakt |

Izbornik je u sve tri crte, sa svim stavkama unutra.
Fotografije su privremene i dolaze s `placehold.co` — zamijeni ih svojima.

## Verzija 2 — mapa `verzija-2-teren/`

Zasad samo naslovnica. Pozadina je "teniski teren": ljubičasti rub (out),
narančasti pravokutnici lijevo i desno, drveni teren u sredini za sadržaj.
Preko svega ide uzorak s 2D oblicima ormara.

Slike su lokalne, u `verzija-2-teren/img/`:

- `tile-out.svg`, `tile-play.svg`, `tile-panel.svg` — uzorak ormara
- `logo-mark.svg` — logo

## Što treba urediti prije objave

U kodu je sve označeno komentarom `<!-- UREDI ... -->`:

- `NAZIV_FIRME`, `EMAIL_ZA_KONTAKT`, telefon, `SJEDIŠTE_FIRME`, `OIB_BROJ`, `FACEBOOK_LINK`
- logo i sve fotografije
- za WordPress: linkove u izborniku promijeniti u `/o-nama/`, `/projekti/`, `/galerija/`, `/kontakt/`
- kontakt obrazac zamijeniti WordPressovim Form blokom (`mailto:` nije pouzdan)

Sve boje su na vrhu svake datoteke u `:root` bloku — promjena ondje mijenja cijelu stranicu.
