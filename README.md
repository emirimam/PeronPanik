# Peron Panika

Zarazna puzzle igra s autobusima. Tapni bus da izađe s parkinga i stane na peron. Gomile putnika s lijeve i desne strane ulaze u centralni krug, vrte se oko fontane i iskaču u bus svoje boje. Ako je krug pun, a nijedan putnik ne odgovara autobusima na peronima, nivo je izgubljen.

## Prepreke kroz nivoe

| Od nivoa | Prepreka | Kako radi |
|---|---|---|
| 2 | Tajni bus | Sivi bus s upitnikom otkrije boju kad mu se put oslobodi |
| 3 | Čunjevi | Fiksne prepreke na parkingu |
| 4 | Lanac i ključ | Zaključan bus čeka da bus s ključem iste boje ode |
| 5, 10, 15… | Špica | Nivo na vrijeme, muzika ubrzava |
| 6 | Led | Broj pokazuje koliko autobusa mora otići da se led otopi |

Pojačanja: **Dizalica** (40), **Dozovi** (30, dovodi potrebne putnike u krug), **+1 peron** (80), **+20 s** na špici (50).

Svaki nivo se generiše nasumično i provjerava solverom, pa uvijek ima rješenje sa 5 perona.

## Tehnički

Jedan statični `index.html`: Canvas 2D sa pre-renderovanim spriteovima ljudi, Web Audio sintetizovani zvukovi i pjesma od 32 takta (groove, refren, breakdown, drop), napredak u `localStorage`. Bez build koraka, deploy na Vercel kao statični sajt.

Autor: Emir Imamović
