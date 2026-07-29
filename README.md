# Web stranica — izrada i montaža kuhinja po mjeri

Svih pet stranica je u glavnoj mapi. Svaka je samostalna: HTML i CSS u istoj datoteci, bez JavaScripta.

## Stranice

| Datoteka | Stranica |
|---|---|
| `index.html` | Naslovnica — tri slike preko cijelog ekrana |
| `onama.html` | O nama |
| `projekti.html` | Projekti — Prije / Poslije |
| `galerija.html` | Galerija fotografija |
| `kontakt.html` | Kontakt |

## Boje

Sve su na vrhu svake datoteke u `:root` bloku. Promjena ondje mijenja cijelu stranicu.

| Boja | Kod |
|---|---|
| tamno smeđa | `#2A1B10` |
| svijetlo smeđa | `#A97C50` |
| narančasta | `#E2661A` |
| svijetlo narančasta | `#F5A85C` |
| bijela | `#FFFFFF` |
| crna | `#120C07` |
| krem (dodatna, za polja obrasca) | `#F7F0E6` |

## Pozadina

`img/pozadina.svg` — kosi, nepravilni oblici. Ista je na svim stranicama, fiksna je
(ne miče se dok se skrola), a zaglavlje i podnožje su prozirni pa se vidi kroz njih.
U svakoj datoteci nosi je `<div class="pozadina">` i CSS blok `POZADINA`.

## Slike

Sve su privremene i lokalne, u mapi `img/`:

- `foto-1.svg` … `foto-6.svg` — male slike (galerija, projekti, O nama)
- `foto-1-v.svg` … `foto-6-v.svg` — velike slike (naslovnica, povećani prikaz)
- `uzorak.svg` — uzorak s 2D oblicima ormara
- `logo.svg` — logo

Zamjena fotografije: promijeni putanju u `src="..."`, odnosno u
`style="background-image:url('...')"` na naslovnici.

## Što treba urediti prije objave

U kodu je označeno komentarom `<!-- UREDI ... -->`:

- `NAZIV_FIRME`, `EMAIL_ZA_KONTAKT`, telefon, `SJEDIŠTE_FIRME`, `OIB_BROJ`, `FACEBOOK_LINK`
- logo i sve fotografije
- za WordPress: linkove u izborniku promijeniti u `/o-nama/`, `/projekti/`, `/galerija/`, `/kontakt/`
- kontakt obrazac zamijeniti WordPressovim Form blokom (`mailto:` nije pouzdan)
