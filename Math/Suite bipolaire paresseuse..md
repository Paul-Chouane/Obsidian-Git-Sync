# Définition
On dit que $(u_n)$ est une suite bipolaire paresseuse si et seulement si :
$$
\begin{align}
&\lim\limits_{n\rightarrow+\infty} \frac{u_{n+1}}{u_n} = 1 &&\rightarrow\text{On parle de suite paresseuse}\\
&(u_n)\text{ n'admet pas de limite}&&\rightarrow\text{On parle de suite bipolaire}
\end{align}
$$
On suppose implicitement qu'il existe un rang $n_0$ à partir du quel $\forall n\geq n_0, (u_n)\neq0$ pour que la limite $\lim\limits_{n\rightarrow+\infty} \frac{u_{n+1}}{u_n} = 1$ est un sens.

# Existence
### Recherche...

On propose alors de trouver une tel suite.
Pour qu'elle soit bipolaire nous allons la faire osciller entre 1 et 2.

On pose alors $u_0 = 1$ puis $u_1 = 2$.

Nous allons maintenant la diviser $2$ fois par un facteur $m_1$ pour la faire repasser à $1$
ce facteur vérifie : $(m_1)^2 = 2 \Rightarrow m_1 = \sqrt{2}$ 
ainsi $u_2=\sqrt{2}$ et $u_3 = 1$

Faisons la même chose avec $3$ étapes en multipliant et un facteur $m_2 = 2^{1/3}$.

### Définition de la suite

De manière générale on pose $m_p = 2^{1/(p+1)}$
On remarquera que $n\in\mathbb N$ s'écrit de manière unique avec $(p,r)\in\mathbb N^2$ tel que $r\leq p$, sous la forme :
$$n=\sum_{i=0}^{p}{i}+r$$
Et avec cette notation on pose :
$u_{n+1} = m_p\cdot u_n$              si $p$ pair.
$u_{n+1} = \frac{u_n}{m_p}$                    si $p$ impair.

### Bipolarité de la suite

Ainsi on remarque que pour $p$ pair, et $r = 0$
$u_n = 1$
Et pour $p$ impair, et $r = 0$
$u_n=2$
(Démontrable par récurrence en remarquant que si $u_n = 1$ on aura $u_{n+p+1}= (m_p)^{p+1}\cdot 1 = 2$ et vis versa)
Autrement dit $(u_n)$ oscille entre 1 et 2 elle n'admet pas de limite et est donc bipolaire.

### Paresse de la suite

On a selon la définition :

$\frac{u_{n+1}}{u_n} = m_p$ ou $\frac{u_{n+1}}{u_n} = \frac1{m_p}$ 

**or :** 

$\lim\limits_{p\rightarrow+\infty} m_p = \lim\limits_{p\rightarrow+\infty} 2^{1/(p+1)} = 2^0 = 1$ et donc $\lim\limits_{p\rightarrow+\infty} \frac1{m_p} = 1$

Finalement en remarquant que si $n\rightarrow +\infty$ alors $p\rightarrow +\infty$

On a bien : 
$\lim\limits_{n\rightarrow+\infty} \frac{u_{n+1}}{u_n} = 1$

$(u_n)$ est donc bien paresseuse bipolaire.

### Être heureux d'avoir trouvé

Chouette !