﻿---
directory_name: Progetti
title: Progetto Tressette
in_menu: true
sort_info: 62
---

h2. Tressette

<img src="{relocatable: /images/tressette/in_partita_small.jpg}">

*__Tressette__* è un gioco di carte molto famoso in Italia, che viene giocato in numerosissime
varianti locali. Il programma, compresi i sorgenti, ho fatto in modo che venisse
ospitato su sf.net in modo da potere agevolare lo sviluppo open source del tressette.
È disponibile per molte piattaforme(Windows, Linux, Freebsd) e si può scaricare dalla pagina del
"progetto tressette":http://sourceforge.net/projects/tressette/.

h3. Sommario

    * "Giocatori":#prj_tre_giocatori
    * "Le carte":#prj_tre_carte
    * "Distribuzione delle carte":#prj_tre_cartedistr
    * "Il gioco":#prj_tre_gioco
    * "Il punteggio":#prj_tre_punteggio
    * "Localizzazioni":#prj_tre_locale
    * "Algoritmo di gioco":#prj_tre_algoritmo

h3(#prj_tre_giocatori). Giocatori

Il Tressette è un gioco di carte molto famoso in Italia. Si gioca in quattro in coppia. Conta numerose varianti, anche molto diverse, a seconda della zona dove viene praticato.

Il programma tre.exe nasce col proposito di simulare il gioco del Tressette in quattro mantenendo intatte le varie localizzazioni. Leggendo vari testi che descrivono il gioco si ha sempre l'impressione di trovare la vera fonte del gioco. Si trova quindi una lista di regole che nella pratica del gioco giocato non trova riscontri, se non in circoli o tornei particolari. Alla fine chi gioca a tressette vuole giocare il tressette che ha sempre giocato e non è molto interessato al gioco che si pratica in altre zone.

h3(#prj_tre_carte). Le carte

Viene usato il mazzo di carte da briscola con 40 carte. L'ordine delle carte è il seguente, dalla carta pi alta a quella pi bassa: tre, due, asso, re, cavallo, fante, sette, sei, cinque e quattro.

h3(#prj_tre_cartedistr). Distribuzione delle carte

Il mazzo da briscola viene mescolato dal mazziere e distribuito ai 4 giocatori. Ogni giocatore riceve 10 carte, distribuite 5 per volta dal mazziere, in senso antiorario. Il mazziere cambia, in senso antiorario, alla fine della smazzata.

h3(#prj_tre_gioco). Il gioco

Il giocatore successivo, in senso antiorario, al mazziere comincia il gioco. Esso gioca una carta e i giocatori successivi devono rispondere al seme della prima carta giocata. Se questo non è possibile, allora il giocatore gioca un'altra carta qualsiasi. Rifiutare il segno non è consentito.

Vince la mano chi ha giocato la carta pi alta del primo segno giocato.

h3(#prj_tre_punteggio). Il punteggio

Quando tutte e 10 le mani sono state giocate, si contano i punti. Il punteggio massimo raggiungibile in una giocata, senza accuse, è di 11 punti. Un punto viene attribuito alla coppia che vince l'ultima mano, ogni asso preso vale un punto, mentre un due, un tre, un re, un cavallo e un fante, valgono rispettivamente un terzo di punto.

Un punteggio extra viene garantito dall'accusa. Le accuse da tre punti sono sono: Napoletana (asso, due, tre in un seme), tre tre, tre due e tre assi. Quelle da 4 punti sono: quattro assi, quattro due e quattro tre.

Il gioco termina quando viene raggiunto il punteggio stabilito.

h3(#prj_tre_locale). Localizzazioni

Il programma *__tre.exe__* implementa le seguenti localizzazioni:

    * Bredese (bassa mantovana)
    * Neutra (classica o senza patria)

h3. Variante Bredese

La variante bredese è quella del gioco del tressette che si gioca a Breda Cisoni nel bar della cooperativa o al bar acli. In questa variante si usano le accuse dei buoni giochi. Per una perfetta simulazione del gioco è meglio impostare la lingua sul dialetto bredese per distinguere meglio i segnali.

I segnali utilizzati vengono normalmente eseguiti con la mano, e sono, a volte, accompagnati anche da una espressione vocale. Nel programma essi vengono tutti dichiarati, anche se nel gioco reale nessun giocatore dice "ho il tre", ma dà un pugno sul tavolo mentre gioca la carta.

I segnali utilizzabili nel programma sono:

 *  Busso (Cioca), il giocatore butta la carta forte sul tavolo perché vuole dal compagno la carta migliore
 * Volo, il giocatore va girare la carta in aria e dice "volo". Significa che il giocatore gioca l'ultima carta del seme della mano.
 * Striscio lungo, il giocatore striscia la carta sul tavolo. Significa che egli possiede molte carte del seme della mano.
 * Punto, il giocatore punta la carta col pollice e dice "la punto", anche per non confondere il segno con l'asso. Significa che egli possiede ancora una sola carta del seme della mano.
 * Via, il giocatore butta via la carta sul tavolo e dice "via". Significa che il socio non deve giocare il seme "buttato via" dal giocatore che ha fatto il segno.
 * Busso il tre, il giocatore da un pugno sul tavolo e non dice nulla. Significa che egli ha il tre nel seme della mano.
 * Busso il due, il giocatore bussa con le nocche sul tavolo e non dice nulla. Significa che egli ha il due nel seme della mano.
 * Punta l'asso, il giocatore punta la carta col pollice e non dice nulla. Significa che egli ha l'asso nel seme della mano.

Il giocatore al proprio turno, può giocando una carta, effettuare un qualsiasi segnale sopraelencato, anche se non corrisponde alle carte che ha in mano (segnare falso). I segnali non sono mai obbligatori

Di solito il gioco finisce quando una coppia raggiunge il punteggio di 101 e la coppia perdente passa al banco a pagare il caffè alla coppia vincitrice, oppure lancia una rivincita a briscola, ma questo è un altro gioco.

h3. Variante Neutra (classica)

Partendo dal presupposto che il tressette è un gioco locale, diventa difficile definire un insieme di regole del gioco che vadano bene al nord come al sud dell'Italia. Basta vedere le regole definite da Wikipedia.it, oppure da Pagat. In realtà questa variante non dovrebbe neanche esserci, ma visto che non è possibile implementare tutte le varianti in una volta sola, meglio averne una che possa permettere di giocare anche senza localizzazione.

Questi sono i segnali supportati:

 * Busso, invita il compagno a giocare la carta migliore.
 * Volo, l'ultima carta del seme della mano.
 * Liscio, quando il giocatore possiede altre carte basse dello stesso seme.

Non è possibile effettuare segnali falsi ed è possibile segnalare le carte al proprio turno.

h3(#prj_tre_algoritmo). Algoritmo di gioco

L'algoritmo di gioco si ispira alle soluzioni adottate nel gioco del bridge. L'implementazione attuale (ver 0.69) è lontana dall'essere efficiente in tutte le fasi del gioco. L'idea alla base è quella di utilizzare un algoritmo alpha-beta, come quello che viene usato nei programmi di scacchi. La differenza con gli scacchi è che, nel caso del tressette, le carte dell'avversario non sono conosciute e devono essere supposte, per esempio a caso. Se si riescono a fare numerose supposizioni e per ognuna di esse, si calcola l'algoritmo, si può avere come risultato una strategia che, a lungo andare, può essere vincente (metodo montecarlo). Il problema da risolvere, nell'implementazione corrente, è la limitatezza del tempo di calcolo di una giocata. Tempi superiori a qualche secondo non sono tollerati durante il gioco del tressette.

