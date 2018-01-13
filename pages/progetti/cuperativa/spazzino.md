﻿---
directory_name: Progetto Cuperativa
title: Spazzino
in_menu: true
sort_info: 202
---

h2. Lo Spazzino

Lo Spazzino è un gioco di carte italiano variante della Scopa. 
Si pratica con un mazzo di 40 carte da briscola.

Lo Spazzino del software Cuperativa si gioca in due. Il mazziere distribuisce tre carte a ciascun giocatore, 
quindi mette quattro carte sul tavolo. 
Quando tutti i giocatori hanno giocato tutte le proprie carte, il mazziere ne distribuisce altre tre a 
ciascuno fino ad esaurimento del mazzo.

h3(#spazs1). Giocare le carte

Ciascun giocatore a turno gioca una carta e comincia sempre chi non ha fatto il mazzo. Il mazziere cambia ad ogni smazzata, 
sempre procedendo in senso antiorario.

<ul>
  <li> Se la carta giocata è di valore uguale a quello di una carta, o alla somma dei valori di più carte 
che si trovano sul tavolo, il giocatore
prende la carta da lui giocata e quella o quelle di valore corrispondente ponendole coperte in un 
mazzetto a parte. Se la carta non effettua prese, rimane sul tavolo. 
Le figure (fante, cavallo e re) non possono prendere carte sommate, ma prendono solo le corrispondenti figure. 
Ad esempio un fante di spade non può prendere un asso, un tre e un quattro, ma solo il fante di un altro segno.</li>
  <li> Se un giocatore prende una carta che il giocatore a lui precedente ha giocato senza prese, vale a dire è rimasta sul tavolo,
realizza una _picula_ (piccola) e vale un punto. Per contrassegnare la piccola effettuata, 
il giocatore pone nel mazzetto delle sue prese una carta scoperta e la mette di traverso alle altre. </li>
  <li> Se un giocatore prende tutte le carte che si trovano sul tavolo, realizza una spazzino e anche 
questo vale un punto. Per contrassegnare la spazzino effettuato, il giocatore pone nel mazzetto delle 
sue prese una carta scoperta e la mette di traverso alle altre. </li>
  <li> Se un giocatore prende con una carta due o più carte dello stesso seme (es. un 5 di coppe e un 
2 di coppe con un 7 di coppe) si realizza un bàgher e ognuna delle carte vale un punto. 
Nell'esempio citato, il giocatore che ha giocato il 7 di coppe realizza 3 punti. </li>
  <li> Al termine della smazzata, tutte le carte eventualmente rimaste sul tavolo
  vengono prese dal giocatore che per ultimo ha giocato una carta con presa. Se il
  giocatore che gioca l'ultima carta prende la carta del giocatore precedente,
  questa non vale come picula, o se prende tutte le carte sul tavolo, questa non
  vale come spazzino.</li> 
</ul>

h3(#spazs2). Punteggio

Al termine di ogni mano viene calcolato il punteggio ottenuto da ciascun giocatore nel seguente modo:

<ul>
  <li> Si assegnano i 7 punti di "mazzo" dati da:</li>
  <ul>
    <li> il giocatore che ha preso più carte di tutti gli altri giocatori ottiene due punti
       Se vi è un pari merito viene assegnato un punto a ciascuno.</li>
    <li> il giocatore che ha preso più carte del seme di spade ottiene due punti. Se vi è un pari merito viene assegnato un punto a ciascuno. </li>
    <li> il giocatore che ha preso il "sette di denari" (onore) ottiene un punto.</li>
    <li> il giocatore che ha preso il "fante di spade" (onore) ottiene un punto.</li>
    <li> il giocatore che ha preso il "due di spade" (onore) ottiene un punto.</li>
  </ul>

  <li> Inoltre vengono assegnati i seguenti punti:
    <ul>
    <li> ogni "picula" effettuata durante la smazzata vale un punto.</li>
    <li> ogni "bàgher" vale un punto per ogni carta presa.</li>
    <li> ogni "spazzino" effettuato durante la smazzata vale un punto.</li>
    <li> il giocatore che prende l'asso, il due e il tre di spade realizza la "napola". 
		  La napola vale tre punti; se però il giocatore ha preso anche il quattro di spade, 
		  ne vale quattro. Se ha preso anche il quattro e il cinque, ne vale cinque; 
		  se ha preso anche il quattro, il cinque e il sei, ne vale sei; e così via. 
		  La napola da dieci punti, che si realizza se il giocatore prende tutte le carte di spade, 
		  si chiama anche "napoleone".</li>
     </ul>
</ul>

I punti ottenuti in ogni smazzata vengono sommati a quelli ottenuti nelle smazzate precedenti.
La partita è vinta dal giocatore che per primo raggiunge o supera i 21 punti. 
Se più giocatori raggiungono o superano i 21 punti nella stessa smazzata, vince chi ha raggiunto il punteggio più alto. 
Se vi è un pari merito, si giocano una o più smazzate di spareggio ad oltranza, finché la parità non termina con un vincitore.
La soglia dei 21 punti viene usata nel software della Cuperativa, ma è di uso comune usare i 31 punti.

