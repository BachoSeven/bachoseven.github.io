# MOTI CENTRALI

## TROVARE ORBITE CIRCOLARI

- Calcolo

$$ V_{eff} = - \int f(\rho) d\rho + \frac{c^2}{2mp^2} $$

  Le traiettorie circolari corrispondono ai punti stazionari di questa funzione

- Calcolo $V_{eff}'=0$ e trovo le radici. Attenzione: non è necessario trovarle esplicitamente, mi serve solo sapere quante ce ne sono. Come farlo?
  - **Regola di cartesio**: vedo quanti cambi di segno consecutivi  ci sono nell'equazione. Questi corrispondono al numero di radici reali positive che troveremo
  - Faccio i limiti e vedo se riesco a fare osservazioni con il teorema di Rolle utilizzando la derivata seconda

## PUNTI DI INVERSIONE

Sono gli zeri di

$$ \bar E - V_{eff} (p) =0$$

Dove spesso viene data $\bar E$
## ENERGIA

### Energia Totale

$$ E_{tot} = \frac{1}{2}m \dot \rho^2 + V_{eff} $$

### Energia minima

$$ E_{min} = V_{eff}(\bar \rho) $$

## DIRE SE UN ORBITA È CIRCOLARE DATE CONDIZIONI INIZIALI

- Per risolvere questo punto dobbiamo già aver trovato i punti stazionari $\bar \rho$ che danno le orbite circolari ai punti precedenti

Ci vengono date delle condizioni per $(x(0), \dot x(0))$ ad esempio, parametriche

$$ x(0) = 2 e_\rho \qquad \quad \dot x(0) = a e_\rho + b e_\theta \qquad a,b \in \mathbb{R}$$

- Come prima cosa in assoluto, possiamo subito dire che $a$ deve essere uguale a zero, perché l'orbita circolare deve essere della forma $(\bar \rho,0)$

- Per trovare $b$ scriviamo

$$ c =  x(0) \times m \cdot \dot x(0)$$

- Poniamo inoltre (tenendo in conto l'esempio)

$$ \rho(0) = 2 $$

- Avevamo trovato ai punti precedenti $\bar \rho$ in funzione di $c$, adesso che lo abbiamo esplicito in funzione di b, possiamo sostituirlo

- Poniamo infine $\bar \rho = \rho(0)$ e otteniamo un valore di $b$

## PERIODO DELL'ORBITA

### Caso facile

Il periodo di un orbita circolare è dato da

$$ T = \frac{2\pi}{|\dot \theta|} = \frac{2\pi}{|c|} m \bar p^2 $$

dove $\bar p$ è il punto stazionario trovato prima alla $V_{eff}$

### Con integrale

Sappiamo che

$$ E = \frac{1}{2} m \dot x + V(x) $$

Quindi

$$ \dot x = \sqrt{\frac{2}{m}(E - V(x))} $$

Andiamo a separare le variabili e otteniamo che il periodo è dato da

$$ T = 2 \sqrt{\frac{m}{2}} \int_{x_{min}}^{x_{max}} \frac{1}{\sqrt{(E - V(x))}} $$

Dove $x_{min}$ e $x_{max}$ sono i punti di inversione della funzione trovati tramite

$$ E = \frac{1}{2} m \dot x^2 + V(x) = 0 $$

ma stiamo considerando $\dot x = 0$ quindi $E = V(x)$

## PUNTI DI INVERSIONE

Di norma in questo caso vengono forniti dei valori numerici per $\rho(\bar t), \dot \rho(\bar t), v(\bar t)$

- Calcolo $|c| = \rho(\bar t) v(\bar t)$
- Calcolo

$$ E = E_{eff}^c (\rho(\bar t), \dot \rho(\bar t)) = \frac{\dot p^2 m}{2} + V_{eff}^c (\rho)$$

  dove ovviamente trovo un valore numerico sostituendo i valori dati per ipotesi
- I punti di inversione sono definiti dalla relazione

$$ E - V_{eff}^c (\rho) = 0 $$

  Basta trovare gli zeri di questa equazione e saranno i punti di inversione (potrebbe servire ruffini per risolverla)

# CINEMATICA RIGIDA

## ASSE CENTRALE

Sono tutti quei punti $Q$ tale che

$$ N_Q \times R =0 $$

Possiamo trovare un punto $P$ dell'asse centrale tramite la formula

$$ Q - P = \frac{R\times N_p}{|R|^2} $$

Quindi l'asse centrale

$$ Q + \lambda R$$

Dove $R$ è la sommatoria delle forze agenti sul sistema


## TROVARE IL CENTRO ISTANTANEO DI ROTAZIONE
[DI NORMA DI UN ASTA]

- Fisso un sistema di riferimento $Oe_1e_2e_3$ e mi scrivo la velocità angolare $\omega$ dell'asta
- Prendo un punto solidale all'asta, $B$, e detto $C_0$ il centro istantaneo di rotazione si ha

$$ C_0 - O = B-O + \frac{\omega \times v_B}{|\omega|^2}  $$

Il punto $B$ in generale è un punto solidale all'asta (o quello che ci interessa). Se non abbiamo modo di calcolare la velocità, usiamo la formula fondamentale della cinematica dei moti rigidi. Prendiamo per esempio il caso di un asta, di estremo $A$, solidale all'origine $O$.

$$ v_O = v_A + \omega_a \times (O-A) $$

- Attenzione: nel caso di puro rotolamento di un disco/anello, la velocità nel punto di contatto è nulla. Ma se ad esempio è su un piano inclinato ad angolo variabile, devo usare la formula fondamentale della cinematica rigida per trovare la velocità del punto di contatto

## POLARE FISSA E MOBILE

### Polare Fissa

Una volta trovato il centro istantaneo di rotazione, di norma guardandolo si capisce che la polare fissa descritta è una qualche figura, di norma è sempre sempre una circonferenza. Basta scrivere l'equazione della circonferenza

### Polare mobile

Fisso un sistema solidale all'oggetto, per esempio nel caso di una asta $AB$ ad un estremo. Quindi $Ae_1'e_2'e_3'$ con $e_1'$ parallelo e concorde ad $A-B$. Mi scrivo $e_1,e_2$ in funzione di $e_1', e_2'$ e vado a sostituire nelle coordinate del centro di rotazione che ho trovato con la polare fissa.

## TROVARE IL COEFFICIENTE DELLA REAZIONE VINCOLARE

Basta semplicemente scrivere la seconda equazione cardinale rispetto ad un polo. Se ad esempio ho un asta $AQ$ su cui agisce una forza in $P$ e la gravità, e voglio trovare la reazione vincolare dell'asse $Ox$ sul suo estremo $Q$ che gli si appoggia, basta scrivere

$$ N_A = (P-A) \times (-F e_1) + (B-A) \times (-mg e_2) + (Q-A) \times \Phi e_2 = 0 $$

Si fanno i conti e se al punto precedente si era trovata una condizione di equilibrio, si sostituisce

## EQUAZIONI DEL MOTO CON EQUAZIONI CARDINALI

### Prima equazione cardinale

La prima equazione della meccanica, associata ad un corpo con baricentro $B$

$$ m \cdot a_b = R $$

dove $R$ è la risultate delle forze. Una volta scritta l'equazione, si proietta su $e_1$ o $e_2$ e basta.

- Ricordiamo se il sistema è in equilibrio, $R$ vale 0

### Seconda equazione cardinale

Consideriamo un polo $A$ e un baricentro $B$, la seconda equazione cardinale ha forma

$$ \dot M_A = N_A - \dot x_A \times m \dot x_B $$

Dove, prendendo $B$ come il baricentro

$$ M_A = M_B + m(x_B - x_A) \times \dot x_A  $$

con

$$ M_B = I\omega$$

Ottengo quindi un valore $M_A$ che vado a derivare per ottenere $\dot M_A$. Una volta trovato, calcolo le altre componenti di $(1)$

- $N_A$ si calcola facendo la sommatoria dei prodotti scalari di tutte le forze per la posizione del punto in cui sono applicate meno la posizione di $A$. Se ad esempio avessimo solo la forza di gravità nel baricentro

$$ N_A = (x_B - x_A) \times -mg e_2 $$

Sostituendo tutto alla fine, ottengo una equazione pura

## TROVARE IL BARICENTRO DI UNA LAMINA

- Supponiamo che la lamina sia omogenea di massa $m$ e si fissi un sistema di riferimento $Oxyz$ con $Oxy$ nel piano della della lamina. Vogliamo trovare le coordinate del baricentro

- Trovo la densità di massa $\sigma$ (varia da figura a figura)

- Parametrizzo la superficie come ad analisi due $\tau = \{(x,y) :  ... \}$

Le coordinate del baricentro allora sono

$$ x_B = \frac{\sigma}{m} \int_\tau x dxdy \qquad y_B = \frac{\sigma}{m} \int_\tau y dxdy     $$

## SISTEMA DI FORZE EQUILIBRATO

Per un sistema di forze essere equilibrato, il momento risultato delle sue forze rispetto ad un polo deve essere equilibrato. Quindi faccio la sommatoria dei prodotti vettoriali tra le forze esterne applicate in un punto e quel punto rispetto al polo

# MOMENTI DI INERZIA

Considero la densità di massa, è una funzione

$$ \rho : \mathbb{R^3} \to \mathbb{R^3} $$

mentre la massa

$$ m = \int_c \rho(x') dx' $$

I momenti di inerzia sono

$$ I_{ij} = \int_c \rho(x')(e_i' \times x')(e_j' \times x') dx' $$

Quindi ad esempio, dati $(x,y,z) \in c$

$$ I_{11} = \int_c \rho(x,y,z)(y^2 + z^2)~dxdydz $$

$$ I_{12} = \int_c \rho(x,y,z)(x^2 + z^2)~dxdydz $$

$$ I_{33} = \int_c \rho(x,y,z)(x^2 + y^2)~dxdydz $$

Se dovesse adesso venirci chiesto di trovare il momento di inerzia rispetto ad un punto, possiamo usare il teorema di Huygens-Steiner. Calcoliamo prima il 1. momento di inerzia rispetto all'origine con

$$ I_{Oe_3} = \sigma \int_\tau (x^2 + y^2) ~dxdy$$

Infine, se dovessimo averne bisogno rispetto ad un punto $G$

$$ I_{Ge_3}  = I_{Oe^3} - m|G-O|^2 $$

## TROVARE I MOMENTI DI INERZIA

- Come prima cosa bisogna sempre trovare un riferimento principale di inerzia in maniera intelligente, ad esempio dato un punto $G$, prendiamo $Ge_1e_2e_3$

- Cercare eventuali simmetrie: se ad esempio il corpo è sta nel piano $Gxy$ ed è simmetrico per rotazione attorno a $Ge_3$ allora i momenti principali di inerzia soddisfano

$$ I_1 = I_2 = \frac{1}{2}I_3 $$

 e basterebbe quindi calcolare solo $I_3$

## Momenti di inerzia noti

<!-- ![[inerzia.png.png]] -->

# LAGRANGIANE

## CALCOLARE LA COMPONENTE LAGRANGIANA DELLE FORZE ATTIVE

- Trovare le coordinate di tutti i punti su cui agisce una forza (anche gravità)
- Trovare l'espressione di tutte queste forze
- Calcolare la componente, ad esempio rispetto a $\theta$, come la sommatoria del prodotto della derivata di un punto rispetto a theta per la forza

## EQUAZIONI DEL MOTO TRAMITE LAGRANGIANE

- Calcolo l'energia cinetica del sistema $T$
- Calcolo l'energia potenziale del sistema $V$

Ottengo infine

$$ L = T - V $$

Per scrivere le equazioni di lagrange, dobbiamo calcolare le derivate. Supponiamo di avere come coordinate lagrangiane $s, \theta$. Le equazioni di lagrange sono

$$ \frac{d}{dt} \Big( \frac{\partial L}{\partial \dot s} \Big) = \frac{\partial L}{\partial s} \qquad \qquad \frac{d}{dt} \Big( \frac{\partial L}{\partial \dot \theta} \Big) = \frac{\partial L}{\partial \theta} $$


## RUTH

Ci viene dato un problema, di norma con una figura in 3 dimensioni parametrizzata ed un punto che vi scorre sopra. Ci viene chiesto di trovare la lagrangiana del sistema e ridurre il sistema ad un solo grado di libertà tramite Routh

- Calcolare $v_P$ facendo le derivate delle 3 componenti $x,y,z$ del punto parametrizzato
- Energia cinetica
- Energia potenziale
- $L = T-V$
- Calcolare

$$ P_\theta = \frac{\partial L}{\partial \dot \theta} $$

  Una volta calcolato, pongo questo questo uguale a $c$. In questo modo posso trovarmi $\dot \theta$ in funzione di $c$ e un'altra variabile

- Calcolare

$$ L_R^c = [L - c \dot \theta] = [(T-V) - c \dot \theta] $$

  In realtà è molto più veloce fare

  $$ L_R^c = -L_2^R + L_0^R$$

  il tutto valutato in $\dot \theta = v(\theta)$ dove $v$ è la funzione trovata prima

- Calcolare

$$ J_R^c = \frac{\partial L}{\partial \dot z} \dot z - L = L_2 - L_0$$

  Questa espressione sarà divisa in due blocchi: uno dove si raccoglie qualsiasi cosa abbia $\dot z$, ed il resto. A noi interessa questo resto (quello dove non si raccoglie), che diventa la $V_{eff}$

- Una volta ricavata la $V_{eff}$ posso trovare $V'_{eff}$ e da questa mi ricavo gli zeri, che saranno i punti stazionari, come negli esercizi dei moti centrali

# CONFIGURAZIONI DI EQUILIBRIO

- Scrivere l'energia potenziale del sistema

Supponiamo che abbiamo i parametri $\phi, \theta$, allora scrivo e risolvo il sistema

$$ \begin{cases}
  \frac{\partial V}{\partial \phi} = 0\\
  \frac{\partial V}{ \partial \theta} = 0
\end{cases} $$

E trovo coppie $(\phi, \theta)$ di soluzioni, queste sono le configurazioni di equilibrio.

## STUDIO DELLE CONFIGURAZIONI DI EQUILIBRIO

Dopo aver trovato le configurazioni di equilibrio scriviamo la matrice hessiana della energia potenziale

<!-- ![](https://www.algebrapracticeproblems.com/wp-content/uploads/2021/02/hessian-matrix-formula.png) -->

- Per ogni configurazione di equilibrio trovata, sostituisco i valori e devo dire se la configurazione della matrice $V''$ è stabile. Per farlo guardo traccia e determinante, se sono positivi allora la configurazione di equilibrio è stabile per Lagrange Dirichlet

- Se dovesse essere una matrice $3 \times 3$ posso usare il criterio di Sylvester e controllare i tre minori principali della matrice.

## FREQUENZE PROPRIE E MODI NORMALI PER PICCOLE OSCILLAZIONI

Consideriamo un sistema con coordinate lagrangiane $s_1, s_2$, le frequenze proprie sono

$$ \omega_1 = \sqrt{\lambda_1} \qquad \omega_2 = \sqrt{\lambda_2}$$

soluzioni dell'equazione secolare

$$ det(V''(s_1, s_2) - \lambda A(s_1, s_2)) = 0 $$

altrimenti trovando gli autovalori della matrice

$$ A^{-1} V''(s_1, s_2) $$

Dove $A$ è la matrice cinetica. Assumendo che l'energia cinetica sia una funzione delle due variabili $x$ e $y$ e delle loro derivate rispetto al tempo $t$, la matrice cinetica $K$ può essere scritta in notazione matriciale come:

$$K =
\begin{bmatrix}
\frac{\partial^2 T}{\partial \dot{x}^2} & \frac{\partial^2 T}{\partial \dot{x} \partial \dot{y}}\\
\frac{\partial^2 T}{\partial \dot{y} \partial \dot{x}} & \frac{\partial^2 T}{\partial \dot{y}^2}
\end{bmatrix}$$

dove $T$ rappresenta l'energia cinetica del sistema e $\dot{x}$ e $\dot{y}$ sono le derivate rispetto al tempo delle variabili $x$ e $y$, rispettivamente.

Si noti che la matrice cinetica è simmetrica, il che significa che $\frac{\partial^2 T}{\partial \dot{x} \partial \dot{y}} = \frac{\partial^2 T}{\partial \dot{y} \partial \dot{x}}$. Inoltre, gli elementi diagonali sono positivi, ovvero $\frac{\partial^2 T}{\partial \dot{x}^2} > 0$ e $\frac{\partial^2 T}{\partial \dot{y}^2} > 0$.

I modi normali di oscillazione sono le famiglie di funzioni vettoriali

$$ c_1 \cos(\omega_1 t + \Phi_1)u_1 \qquad c_2 \cos(\omega_2 t + \Phi_2)u_2 $$

dove, per $j=1,2$, $c_j \in \mathbb{R}^+, \Phi_j \in S^1$ ed $u_j$ un autovettore di $V''(s_1, s_2) - \lambda_j A(s_1, s_2)$.

# QUANDO TUTTO GIRA

## Leggi di trasformazione

Consideriamo un sistema di riferimento $\Sigma$ e consideriamo un sistema $\Sigma'$ che ruota rispetto a $\Sigma$ con una velocita angolare $\omega$ sappiamo che abbiamo delle leggi di trasformazione per le velocità ed accelerazioni

$$ a' = a - a_{trascinamento} - a_{coriolis} $$

Dove

$$ a_t = a_{O'} + a_{centrifuga} + derivata  $$
$$ = a_{O'} + \omega \times (\omega \times(P - O')) + \dot \omega \times(P - O') $$

Mentre

$$ a_{coriolis} = 2 \omega \times v' $$

---

Ci viene dato un sistema con un corpo. Parametrizziamo un punto su questo, ad esempio su un asta lunga $L$ prendo un punto $P \in [0,L]$

- L'energia cinetica resta invariata, si fa come nel caso normale
- L'energia potenziale si divide in forza peso, forza elastica (se esiste) e forze apparenti

$$ V = V_{peso} + V_{elastica} + V_{apparenti} $$

dove

$$ V_{app} = V_{coriolis} + V_{centrifuga} + V_{trascinamento} $$

**TRUCCO:** Se siamo in un piano $Oxy$ e giriamo attorno ad $y$ con $\omega$ costante, di norma sia $v_{cor}, V_{tra}$ sono nulle, quindi ci interessa solo quella centrifuga. In generale possiamo calcolarle come

$$ V_{cor} = - \int_0^L \lambda (\omega\times(P-O'))\cdot v'$$

$$ V_{centr} = - \frac{1}{2} \int_0^L \lambda | \omega \times (P-O')|^2 = - \frac{1}{2} \int_0^L \lambda \cdot \omega^2\cdot (x_P - x_{O'}) e_1 $$

$$ V_{tra} = \int \lambda a_{O'} \cdot (P-O') $$

Nel caso di un punto materiale abbiamo ad esempio

$$ V_{tra}= m \cdot a_{O'} \cdot (P - O') $$
