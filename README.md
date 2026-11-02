# Statistička analiza podataka – projekt u R-u

Timski projekt iz kolegija Statistička analiza podataka (ak. g. 2024./25.), izrađen u programskom jeziku R.

Analiziran je skup podataka o jednoj ciljanoj telefonskoj marketinškoj kampanji banke (45 211 klijenata) s ciljem da se statističkim metodama odgovori na četiri istraživačka pitanja:

1. **Postoji li zavisnost između zanimanja i bračnog statusa klijenta?** Hi-kvadrat test nezavisnosti uz analizu standardiziranih reziduala. Varijable su zavisne, a najveća odstupanja pokazuju studenti (većinom neoženjeni) i umirovljenici.
2. **Imaju li klijenti s otvorenim kreditom više novca na računu od ostalih?** Welchov t-test (jednostrani) nad Box-Cox transformiranim stanjem računa, posebno za stambeni i nenamjenski kredit. Nema dokaza da klijenti s kreditom imaju više novca na računu.
3. **Razlikuje li se trajanje poziva među klijentima različitog obrazovanja?** ANOVA nad Box-Cox transformiranim podacima ne pokazuje razliku u prosjecima, dok Kruskal-Wallisov test pokazuje razliku u medijanima.
4. **Mogu li dostupne varijable predvidjeti uspješnost kampanje?** Logistička regresija za ciljnu varijablu `term_deposit_accepted`, uz provjeru multikolinearnosti (VIF) i usporedbu modela (analiza devijance). Najjači prediktori su trajanje poziva, ishod prethodne kampanje i mjesec kontakta.

## Sadržaj

* [`data.csv`](data.csv) – skup podataka
* [`opis_varijabli`](opis_varijabli.xlsx) – opis varijabli
* [`Statisticka_analiza-podataka_projekt`](Statisticka_analiza-podataka_projekt.Rmd) - R kod projekta
* [`Statisticka_analiza_podataka_projekt.pdf`](Statisticka_analiza_podataka_projekt.pdf) – izvještaj s cjelokupnom analizom, grafovima i zaključcima

## Tehnologije

R, ggplot2, MASS (Box-Cox transformacija), car (VIF), caret


## Autorice

Iva Rengel, Matea Bušić, Marta Bandur, Karla Budimir
