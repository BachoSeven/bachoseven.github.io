---
title: "Domande orali Ricerca Operativa"
math: true
---

## Appello Gennaio 2022

---

- Definizione e caratterizzazione algebrica direzioni ammissibili e di crescita + considerazioni varie su Lemma di farkas e la mutua esclusività dei due problemi
- Formulazione in PL problema di flusso di costo minimo, variante se volessi minimizzare il flusso su ogni singolo arco
- Trovare i piani di taglio di Gomory su un esempio pratico

---

- Cosa succede nell'algoritmo del simplesso primale se $A_N \xi<=0$ e collegamento con il teorema fondamentale della PL.
- Data un'istanza del problema del flusso di costo minimo come stabilire se esistono flussi ammissibili.
- Modello PLI per il problema ddl commesso viaggiatore.

---

- Direzione di crescita del simplesso duale
- Esercizio di modellazione con annessa una domanda sul flusso che non ricordo precisamente, ma era scrivere come problema lineare uno dei problemi di flusso
- L'algoritmo del rilassamento del TSP

---

- Mi ha chiesto il teorema forte della dualità e un esercizio di branch and bound TSP

## ??/2023

- Teorema forte della dualità
- Caratterizzazione dell'ottimalità per il problema dei cammini minimi
- Piani di taglio di Gomory

---

- Caratterizzazione algebrica delle direzioni di ammissibilità e di crescita
- (DR) ha soluzione, che posso dire della soluzione duale?
- Esempio geometrico di soluzione primale unica e duale degenere
- Formulazione di TSP in PLI con rilassamento MST
- Caratterizzazione dell'ottimalità per il problema dei cammini minimi
- Se so che $3x_1+6x_2+9x_3<=13$ è un piano di taglio, allora posso dire che anche $x_1+2x_2+3x_3<=4$ è un piano di taglio?

---

- Cosa si può dire se $A_N \xi \leq 0$?
- Formulazione di CSP in PLI con rilassamento
- Discutere l'ottimalità di CSP al variare del parametro L
- Discutere l'esistenza di una soluzione ammissibile per CSP (trovare un algoritmo: cammini minimi con costi=lunghezze)

---

- Verificare mediante scarti complementari se una soluzione del duale è ottima
- Relazione tra flusso massimo e taglio minimo
- Esempio di grafo con più tagli di capacità minima
- Rilassamento convessificato di un problema di programmazione lineare intera

---

- Caratterizzazione direzioni ammissibili e di crescita
- Piani di taglio di Gomory
- E' possibile che il problema di flusso massimo sia vuoto? Può essere che il valore del flusso massimo sia zero? Quando è possibile?

---

- Esegui un'iterazione del simplesso duale
- Definisci piani di taglio di Gomory e trovane uno per il problema precedente
- Dato un grafo, esibire dei bilanci, costi e capacità tali che il problema di flusso di costo minimo ammetta più di una soluzione (e dire quante)

---

- Dato il problema $\max(x_1+2x_2)$ soggetto ai vincoli : $$x_2 \leq 4,~x_1 \leq 2,~x_1-2x_2 \leq 10,~2x_1 + x_2 \leq 4,~-x_1 \leq -4,$$ come decidere da $B = {4,5}$ quale algoritmo utilizzare ?
- Dimostrare che $y(\theta)$ è una direzione di decrescita nell'algoritmo del simplesso duale
- Flusso massimo - taglio minimo con dimostrazione
- Data una rete, fornire un algoritmo per trovare il cammino minimo dal nodo $s$ al nodo $t$ supponendo che ogni nodo costi $T$, con tempi di percorrenza degli archi $t_{ij} , t_{i' j'}$ (??)

---

- Modello PL del problema di flusso di costo minimo
- Un flusso ammissibile è di costo minimo se e solo se non esistono cicli amumentanti negativi
- Modellazione di un problema di cammino minimo "doppio", con due coppie sorgente-destinazione
- Come cambia il modello se impongo che i cammini (da $s1$ a $t1$, da $s2$ a $t2$) non abbiano archi in comune?
