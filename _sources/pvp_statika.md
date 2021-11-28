# Princip virtuálních prací (PVP) (☕☕☕)

PVP je zcela odlišný způsob jak dojít k rovnovážnému stavu tělesa. Výchází z předpokladu, že těleso v rovnováze zůstane v rovnováze i po malém (nekonečně malém vychýlení) a že práce vykonaná silami po tomto malém (virtuálním) posunutí je nulová. PVP princip je univerzální a vzhledem k tomu, že práce (energie) je nezávislá na souřadnicovém systému, je i méně pracný než uvolňovací metoda.

## Princip virtuální práce hmotného bodu
Hmotný bod (HB) je v rovnováze tehdy, pokud platí, že výslednice sil je rovna nule:

$$
\begin{equation}
    F = 0
\end{equation}
$$

Nyní HB přesuneme "virtuálně" o libovolný malý úsek $\delta r$. HB vykoná virtuální práci:

$$
\begin{equation}
	\delta W = F\cdot\delta r = 0
\end{equation}
$$

Vztah říká, že je-li HB v rovnováze, virtuální práce sil působcích na HB je 0 pro libovolné virtuální posunutí $\delta r$. Pokud je virtuální práce 0, musí platit i obráceně, že HB je v rovnováze. Zvolme například $\delta r = {\delta x, 0, 0}$, vidíme, že:

$$
\begin{equation}
	\delta W = 0 = F_x \delta x + F_y 0  + F_z 0 \rightarrow F_x = 0
\end{equation}
$$

## Princip virtuální práce pro soustavu hmotných bodů

Soustava $N$ HB je v rovnováze jestliže každý HB je v rovnováze, tedy výslednice sil $F_i=0, i=1, ..., N$.

<p align="center">
    <img src="obrazky/prednaska08/PVP_soustava_hmotnych_bodu.png" alt="soustava hmotných bodů" width="130"/>
</p>

Pokud každý bod posuneme o $\delta r_i$, můžeme napsat podle PVP:

$$
\begin{equation}
	\delta W = \sum_{i}^{N} F_i \cdot \delta r_{i}=0
\end{equation}
$$

Obráceně platí, že pokud je $\delta W=0$, musí být soustava HB v rovnováze (stejná úvaha jako pro jeden HB.)

## Virtuální práce reakčních sil

Reakční síla $R$ je dána geometrickou vazbou $z\geq 0$.

<p align="center">
    <img src="obrazky/prednaska08/PVP_prace_vazeb.png" alt="práce vazeb" width="90"/>
</p>

Vidíme, že virtuální posunutí nemůže být libovolné, tj. musí být takové, které neporušuje vazbu (HB nemůžeme zatlačit do stolu) a musí platit, že podmínka vazby je splněna pro $\pm \delta r$.

```{admonition} Poznámka
    Virtuální práce reakčních sil při vratných posunutích slučitelných s vazbami je rovna nule.
```

## Zobecněný PVP
Výslednice sil působící na itý HB je dána:

$
\begin{equation}
    F_i = F_i + R_i
\end{equation}
$


Podle PVP musí platit, že soustava je v rovnováze tehdy:

$$
\begin{equation}
	\sum_{i}^{N} = F_i\cdot \delta r_i=0
\end{equation}
$$

Dosadíme-li, 5 do 6:

$$
\begin{equation}
	\delta W = \sum_{i}^{N} (F_i + R_i)\cdot\delta r_i = \sum_{i}^{N}F_i\cdot\delta r_i + \sum_{i}^{N}R_i\cdot\delta r_i = \sum_{i}^{N}F_i\cdot\delta r_i
\end{equation}
$$

Víme, že virtuální práce vykonaná reakcemi je 0.

## Příklad 01: Kyvadlo

Uvažujme kyvadlo v homogenním gravitačním poli. Nalezněte polohu, kdy je kyvadlo ve statické rovnováze.

<p align="center">
    <img src="obrazky/prednaska08/prednaska_priklad01.png" alt="kyvadlo" width="110"/>
</p>

Kyvadlo obsahuje geometrickou vazbu, která je dána:

$$
\begin{equation}
    \bar{x}^2 + \bar{y}^2 = l^2 = konst.
\end{equation}
$$

Virtuální posunutí spočítáme jako diferenciál (nekonečně malá):

$$
\begin{equation}
    2\bar{x}\delta{\bar{x}} + 2\bar{y}\delta{\bar{y}} = 0
\end{equation}
$$

Podle PVP platí:

$$
\begin{equation}
    \delta W = F\cdot\delta r = 0\delta x + mg\delta y = -\frac{mg}{y}x\delta x = 0
\end{equation}
$$

Pro libovolné $\delta r$, splňující (8), plyne $x=0$! Pro PVP s reakcemi neplyne, že síly $F$ jsou nulové. Nulový je součet $F + R$!

## Příklad 02: Rovnováha na kladce
Uvažujme buben zatížený závažím $m$ v grav. poli. Nalezněte sílu $F$ tak aby byla soustava v rovnováze.

<p align="center">
    <img src="obrazky/prednaska08/prednaska_priklad02.png" alt="kladka" width="130"/>
</p>

Podle PVP platí:

$$
\begin{equation}
    \delta W = -mg\delta u_1 + F\delta u_2 = 0
\end{equation}
$$
Geometrická podmínka je:

$$
\begin{equation}
    \frac{\delta u_1}{r_1} = \frac{\delta u_2}{r_2}
\end{equation}
$$

Dosazením 12 do 11:

$$
\begin{equation}
    \delta W = (-mg\frac{r_1}{r_2} + F)\delta u_2=0
\end{equation}
$$

Nebo:

$$
\begin{equation}
    \delta W = (-mg r_1 + F r_2)\delta\alpha=0
\end{equation}
$$
## Příklad 03: Podepřený hranol

Uvažujte podepřený hranol, který je zatížení vlastní vahou. Nalezněte sílu $F$, tak aby byl hranol v rovnováze.

<p align="center">
    <img src="obrazky/prednaska08/cviceni_priklad01.png" alt="hranol" width="600"/>
</p>


zaveďme: $L = a + b$, $x_B$=c + d, $y_A=\sqrt{\mathrm{L}^2 - x_B^2}$
Napišme rovnici vazby mezi pohybem bodu A a B:

$$
\begin{equation}
    (x_B - \delta x_B)^2 + (y_A + \delta y_A)^2 = L^2 = x_B^2 + y_A^2
\end{equation}
$$

$\delta x_B,\delta y_A$ jsou virtuální posunutí, která jsou na sobě závislá.
Rozepsáním získáme:

$$
\begin{equation}
    x_B^2 - 2x_B\delta x_B + \delta x_B^2 + y_A^2 + 2y_A\delta y_A + \delta y_A^2 = x_B^2 + y_A^2
\end{equation}
$$

členy $\delta x_B^2, \delta y_A^2$ jsou velmi malé a tak je zanedbáme, pak platí, že:

$$
\begin{equation}
    \delta y_A = \frac{x_B}{y_A} \delta x_B
\end{equation}
$$

Podobně platí, že:

$$
\begin{equation}
	\delta y_G = \frac{1}{2}(y_A + \delta y_A) - \frac{1}{2}y_A = \frac{1}{2}\delta y_A
\end{equation}
$$

S uvažováním (18) pak platí:

$$
\begin{equation}
	\delta y_G = \frac{1}{2}\frac{x_B}{y_A}\delta x_B
\end{equation}
$$

Virtuální práce musí být nula aby byla tyč v rovnováze:

$$
\begin{equation}
	\delta W = F_G \delta y_G \cos(180) + F \delta x_B \cos(0) = 0
\end{equation}
$$

Musíme sjednotit virtuální posuv...tedy dosaďme z (20):

$$
\begin{equation}
	\delta W = (-F_G \frac{1}{2}\frac{x_B}{y_A} + F)\delta x_B = 0
\end{equation}
$$

Pro libovolné nenulové $\delta x_B$ musí platit, že výraz v závorce je nula!
Dosadíme za $L = a + b, x_B = c + d, y_A = \sqrt{L^2 - x_B^2}$:

$$
\begin{equation}
\delta W = (-F_G \frac{1}{2}\frac{c + d}{\sqrt{(a + b)^2 - (c + d)^2}} + F)\delta x_B = 0
\end{equation}
$$

Výraz v závorce je rovnice rovnováhy, tedy:

$$
\begin{equation}
    -F_G \frac{1}{2}\frac{c + d}{\sqrt{(a + b)^2 - (c + d)^2}} + F = 0
\end{equation}
$$
