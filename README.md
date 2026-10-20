# Peron Panika

Zarazna puzzle igra s autobusima. Tapni bus da izađe s parkinga, parkira se na peron, a putnici iste boje ulaze sami. Ako se svih 5 perona zatrpa pogrešnim bojama, nivo je izgubljen.

## Prepreke kroz nivoe

| Od nivoa | Prepreka | Kako radi |
|---|---|---|
| 2 | Tajni bus | Sivi bus s upitnikom otkrije boju kad mu se put oslobodi |
| 3 | Čunjevi | Fiksne prepreke na parkingu |
| 4 | Lanac i ključ | Zaključan bus čeka da bus s ključem iste boje ode |
| 5, 10, 15… | Špica | Nivo na vrijeme, muzika ubrzava |
| 6 | Led | Broj pokazuje koliko autobusa mora otići da se led otopi |

Pojačanja: **Dizalica** (40), **Sortiraj red** (30), **+1 peron** (80), **+20 s** na špici (50).

Svaki nivo se generiše nasumično i provjerava solverom, pa uvijek ima rješenje sa 5 perona.

## Tehnički

Jedan statični `index.html`: Canvas 2D, Web Audio sintetizovani zvukovi i muzika, napredak u `localStorage`. Bez build koraka, deploy na Vercel kao statični sajt.

Autor: Emir Imamović
