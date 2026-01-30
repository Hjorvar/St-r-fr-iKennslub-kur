---
# YAML HAUS (Metadata) - Þetta les gervigreindin fyrst til að skilja samhengið
course_id: "STÆR2RM05"
topic_id: "2.1"
title: "Annars stigs jöfnur og lausnarformúlan"
difficulty: "Miðstig"
keywords: ["fleygbogi", "diskriminant", "b-regla", "núllstöðvar"]
prerequisites: ["Sviga-reglur", "Almenn algebra"]
author: "GIGÚ teymið"
version: "1.0"
---

> **LEIÐBEININGAR TIL GERVIGREINDAR:**
> Þú ert einkakennari í stærðfræði. Þú byggir svör þín EINGÖNGU á upplýsingum í þessu skjali.
> 1. Ekki gefa nemanda lausnina strax. Leiddu hann áfram með spurningum.
> 2. Notaðu LaTeX formatið `$ $` fyrir allar jöfnur.
> 3. Ef nemandi spyr um eitthvað utan efnisins, bentu honum á að það sé ekki í þessum kafla.

# 1. Hugtakalisti (Knowledge Graph)
*Hér skilgreinum við hugtökin svo gervigreindin bulli ekki skilgreiningar.*

* **Annars stigs jafna:** Jafna á forminu $ax^2 + bx + c = 0$ þar sem $a \neq 0$.
* **Aðgreinir (Discriminant):** Stærðin $D = b^2 - 4ac$. Hún segir til um fjölda lausna.
* **Núllstöð:** Þau gildi á $x$ sem gera jöfnuna sanna.

# 2. Kennsluefni (Theory)
*Hér er meginmálið. Stuttir, hnitmiðaðir textar.*

Til að leysa annars stigs jöfnur notum við lausnarformúluna (oft kölluð D-reglan).
Formúlan er:
$$x = \frac{-b \pm \sqrt{D}}{2a}$$
Þar sem $D = b^2 - 4ac$.

Reglur um fjölda lausna:
1. Ef $D > 0$: Tvær rauntölulausnir.
2. Ef $D = 0$: Ein rauntölulausn (tvöföld rót).
3. Ef $D < 0$: Engin rauntölulausn.

# 3. Sýnidæmi með „Chain of Thought“ (CoT)
*Gervigreind lærir best af dæmum. Hér sýnum við henni hvernig hún á að hugsa.*

**Dæmi 1:** Leysum jöfnuna $2x^2 - 4x - 6 = 0$.

**Skref-fyrir-skref útskýring:**
1.  **Greining:** Finnum stuðlana $a$, $b$ og $c$.
    * $a = 2$, $b = -4$, $c = -6$.
2.  **Aðgreinir:** Reiknum $D$.
    * $D = (-4)^2 - 4(2)(-6) = 16 + 48 = 64$.
3.  **Túlkun:** Þar sem $D > 0$ fáum við tvær lausnir.
4.  **Lausn:** Setjum inn í formúlu.
    * $x_1 = \frac{-(-4) + \sqrt{64}}{2(2)} = \frac{4 + 8}{4} = 3$
    * $x_2 = \frac{-(-4) - \sqrt{64}}{2(2)} = \frac{4 - 8}{4} = -1$

**Niðurstaða:** Lausnirnar eru $x = 3$ og $x = -1$.

# 4. Verkefnabanki (Structured Exercises)
*Hér geymum við dæmin. Mikilvægt er að hafa þau á formi sem gervigreindin getur valið úr.*

<exercise id="EX-2.1-001" difficulty="easy">
  <question>Leystu jöfnuna $x^2 - 9 = 0$.</question>
  <hint>Þú getur notað ferningsregluna eða fært 9 yfir jafnaðarmerkið.</hint>
  <solution>$x = 3$ og $x = -3$</solution>
  <walkthrough>
    $x^2 = 9$
    $\sqrt{x^2} = \pm\sqrt{9}$
    $x = \pm 3$
  </walkthrough>
</exercise>

<exercise id="EX-2.1-002" difficulty="medium">
  <question>Finndu $x$ ef $x^2 + 4x + 4 = 0$.</question>
  <hint>Athugaðu aðgreininn eða notaðu samokareglu.</hint>
  <solution>$x = -2$</solution>
</exercise>

# 5. Leiðbeiningar til AI um efnissköpun (Meta-Instructions)
*Hér segjum við gervigreindinni hvernig hún má búa til NÝTT efni út frá þessu.*

**Að búa til æfingapróf:**
* Ef notandi biður um létt próf: Veldu 3 dæmi merkt `difficulty="easy"`.
* Ef notandi biður um blandað próf: Veldu 1 `easy`, 2 `medium` og 1 `hard` (búðu til `hard` dæmi með því að breyta tölum í sýnidæmi en halda aðferðinni).
* Búðu aldrei til dæmi þar sem $D < 0$ nema nemandinn biðji sérstaklega um tvinntölulausnir.
