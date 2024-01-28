# Bil

## Fråga

Victoria kör uppför en brant backe (35°) med sin bil i hastigheten 60 km/h. Plötsligt tappar bilen greppet och börjar glida med låsta hjul. 2,0 s efter att Victoria har börjat glida har hon hastigheten 13 km/h uppför backen.

Vilket är friktionstalet mellan bilen och underlaget när hon glider? Utgå ifrån konstant friktionstal. 

## Lösning

Detta problem går att lösas på många sätt. Nedan används energiprincipen.

Energin innan (läge 1):
- Kinetisk energi, $E_{k1}$

Energin efter (läge 2):
- Kinetisk energi, $E_{k2}$
- Potentiell energi, $E_p$
- Friktionsarbete, $W$

Energin innan ska vara lika med energin efter (energiprincipen):

$$E_{k1}=E_{k2}+E_p+W$$

Kinetisk energi innan ($n=1$) och efter ($n=2$), där $v_n$ är hastigheten i läge $n$:

$$E_{kn}=\frac{1}{2}mv_n^2$$

Potentiell energi för höjdskillnaden $h$ mellan läge 1 och läge 2:

$$E_p=mgh=mgs\sin{35°}$$

där $s=\frac{h}{\sin{35°}}$ är den tillryggalagda sträckan upp längst rampen mellan läge 1 och läge 2, som ges av trigonometri. Eftersom friktionstalet antas vara konstant och alla andra krafter inblandade är konstanta har vi likformig acceleration, och sträckan $s$ ges av

$$s=\frac{(v_2+v_1)}{2}t$$

Friktionsarbetet ges av friktionskraften $F_f$ och sträckasn $s$:

$$W=F_fs$$

Friktionskraften ges av friktionstalet (friktionskoefficienten) $\mu$ och normalkraften $F_N$:

$$F_f=\mu F_N$$

Normalkraften är lika stor till beloppet som den komposant av gravitationskraften som verkar vinkelrätt mot rampens yta, det vill säga:

$$F_N=mg\cos{35°}$$

Insättning i energiprincipen ger

$$\frac{1}{2}mv_1^2 = \frac{1}{2}mv_2^2+mgs\sin{35°}+\mu s mg \cos{35°}$$

Massan $m$ återfinns i samtliga termer, vilket gör att den kan strykas. Omskrivning ger friktionstalet $\mu$:

$$\mu=\frac{v_1^2 - v_2^2-2gs\sin{35°}}{2 s g \cos{35°}}$$

Insättning av samtliga värden, med hastigheterna omräknade till enheten $m/s$, ger värdet

$$\mu\approx0.78$$
