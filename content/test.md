---
Title: Test page
Description: This is our test page
Template: test
---

The source for this page is in `content/test.md`.

Test page
==========================

<div class="first-box">
First box
</div>

<div class="second-box">
Second box
</div>

<div class="third-box">
Third box
</div>

<div class="fourth-box">
Fourth box
</div>

<p class="old-fashioned">
Hör nu på, govänner, så ska jag för er berätta vad en gosse gjorde, det är nu längesen, men nog lever minnet kvar i Smålands sköna dalar, Katthult Lönneberga, det var den gossens hem. Hujedamej, sånt barn han var, Ej värre tänkas kan, Och Emil var det namn han bar, Ja, Emil hette han.
</p>

<p class="modern">
Hör nu på, goävanner, så ska jag för er berätta vad vår Emil gjorde en dag i sköna maj. Upp i Katthults flaggsång hissa han sin lille syster, stod sen lugnt og såg henne hänga där på svaj. Hujedamej, sånt barn han var,fast Ida var rätt nöjd, ty ingen annan svävat har på denne höga höjd.
</p>

<p class="worst-ever">
Nästa hyss han gjorde var när han i grönsakssoppan dök på huvet ner og sen satt där stenhårt fast uti mor sins soppskål, ty hans öron var för stora, så det blev att fara till doktorn det med hast. Hujedamej, sånt barn han var, tror inte också ni, att den som blott en soppskål har vill ej ha gossar i?
</p>

<div class="wrapper1"> 
  <div class="bar one1"></div> 
</div>


assets/img:
[![Leaf](%assets_url%/img/leaf_256x256.png)](%assets_url%/img/leaf_256x256.png)
cimage:
[![Leaf](image/leaf_256x256.png?w=1072)](image/leaf_256x256.png)

Hur stretch och crop-to-fit kan se ut:
![Leaf](image/leaf_256x256.png?h=250&w=50&stretch)
![Leaf](image/leaf_256x256.png?h=250&w=50&crop-to-fit)

50% av dess originalbredd:
![Leaf](image/header.jpg?width=50%)

 Som exempel kan vi hämta ut halva dbwebb-lövet på följande sätt:
![Leaf](image/leaf_256x256.png?area=50,0,0,0)
![Leaf](image/leaf_256x256.png?area=0,50,0,0)
![Leaf](image/leaf_256x256.png?area=0,0,50,0)
![Leaf](image/leaf_256x256.png?area=0,0,0,50)

Beskära de mittersta 50x50 på lövet:
![Leaf](image/leaf_256x256.png?crop=50,50,100,100)

Konvertera bilder mellan olika format:
png funkar också men leaf är idag i png.
![Leaf](image/leaf_256x256.png?width=50%&save-as=jpg)
![Leaf](image/leaf_256x256.png?width=50%&save-as=gif)

Skala kvalite:
Testa och verifiera när du gör det.

![Leaf](image/leaf_256x256.png?width=50%)
![Leaf](image/leaf_256x256.png?width=50%&q=50)

Filter:
![Leaf](image/leaf_256x256.png?convolve=lighten)
![Leaf](image/leaf_256x256.png?convolve=darken)
![Leaf](image/leaf_256x256.png?blur)
![Leaf](image/leaf_256x256.png?f=grayscale)
![Leaf](image/leaf_256x256.png?f=brightness,50)
![Leaf](image/leaf_256x256.png?f=contrast,50)