# Bones pràctiques de visualització.

## Introducció
En el món de l’analítica de dades, saber extreure informació útil no és suficient: cal també comunicar-la de manera clara, efectiva i responsable. Aquesta guia està pensada per ajudar-te a dominar els principis i les bones pràctiques de la visualització de dades, una competència fonamental per a qualsevol analista.

L’objectiu és doble: d’una banda, oferir-te eines per crear visualitzacions que facilitin la comprensió i la presa de decisions; de l’altra, acostar-te a un model estandarditzat que pot ser útil especialment en el context de les entitats públiques i locals, on la claredat i la transparència són essencials.

A més, aquesta guia promou valors com la qualitat, la simplicitat, la inclusió i l’ètica, perquè comunicar dades no és només una qüestió tècnica, sinó també una responsabilitat social. Aprendràs a fer servir els recursos visuals adequats, a evitar errors comuns i a dissenyar visualitzacions que realment comuniquin.

## Principis generals de visualització de dades

La visualització de dades ens ajuda a analitzar, entendre i comunicar missatges basats en dades. A diferència d’altres formes de comunicació, com poden ser el llenguatge escrit o la música, la visualització de dades no disposa de criteris ni regles universals de notació i representació semàntica.

Tot i això, hi ha una sèrie de principis àmpliament acceptats i formes de representar les dades que els usuaris reconeixen i poden percebre de manera efectiva i entenedora.

En aquest sentit, cal destacar les aportacions de l’International Business Communication Standards (IBCS), que treballa per unificar la visualització d’informació financera. Igualment, són molt rellevants les contribucions de diversos organismes públics —com l’Institut Nacional d’Estadística, la Generalitat de Catalunya o el portal datos.gob.es, entre d’altres—, que, a través de la publicació de guies i recursos propis, impulsen principis i bones pràctiques de visualització àmpliament reconegudes.

## Principis habituals en l’àmbit de la visualització

En la guia s’han seleccionat vuit principis habituals en l’àmbit de la visualització de dades, que es resumeixen a continuació:

1. Simplificació

2. Percepció fidel

3. Aproﬁtament de l’espai

4. Estructuració correcta

5. Objectivitat i compliment ètic i normatiu

6. Uniformitat

7. Ús adequat del color

8. Accessibilitat i disseny inclusiu

## 1. Principi de simplificació

Aquest principi, conegut com "Simplifica i evita el desordre" (Simplify and avoid clutter), planteja la necessitat que les visualitzacions siguin simples i clares, eliminant tots aquells elements superflus, decoratius, excessivament complexos o redundants que puguin dificultar la comprensió del missatge principal.

L’objectiu és millorar la claredat i l’eficiència comunicativa de la visualització, augmentant la proporció d’informació rellevant respecte a la quantitat de tinta utilitzada. En altres paraules, s’ha de prioritzar la informació essencial i evitar la saturació visual.

**S’han de seguir aquestes recomanacions bàsiques:**
- Evitar elements decoratius o innecessaris, com ara logotips, fotografies, animacions, fons amb trames o textures, efectes 3D, ombres, colors decoratius o tipografies ornamentals.
- Utilitzar colors només amb propòsit, per destacar o diferenciar. L’excés de color pot confondre.
- Preferir el contrast alt i net, com xifres negres sobre fons blanc.
- Reduir el soroll visual: eliminar línies de quadrícula, línies de separació innecessàries en taules, vores i etiquetes supèrflues.
- Simplificar el text: eliminar paraules redundants o evidents (com "gràfic", "taula", "suma", etc.).
- Ajustar les xifres mostrades, evitant decimals innecessaris i etiquetes en valors baixos; cal arrodonir si no es perd significat.

**Exemple d’aplicació del principi de simplificació: Els dos gràfics següents mostren exactament la mateixa sèrie de dades, però en el de la dreta, la comprensió de les dades és més ràpida, eficient i precisa.**

![Exemple del principi de simplificació](./images/limpios.jpg)

**Dèficits identificats en el gràfic de l’esquerra:**
- Els decimals i la repetició de "EUR" en les etiquetes de dades no aporten valor i dificulten la lectura. A més, el color blau de les etiquetes no facilita la percepció.

- Els títols inclouen paraules innecessàries, com ara “anys”, “totals” i “suma”.

- S’incorporen llegendes que no són útils per a la comprensió del gràfic.

- La rotulació de l’eix vertical és prescindible, i el fet que el rètol estigui en sentit vertical en dificulta la lectura.

- El degradat decoratiu i les línies de les barres són elements superflus que generen distracció.

- Es combinen un gràfic de barres i un de línies per a la mateixa sèrie de dades, la qual cosa és redundant i no aporta informació addicional.

- No s’incorporen etiquetes de valor a cada barra, cosa que obliga a l’usuari a fer una traslació visual des de l’eix fins a cada barra.

- Amb la inclusió de les etiquetes de valor, es pot eliminar l’eix Y, ja que en aquest cas no aporta gaire utilitat.

- Les línies horitzontals de projecció de valors (grid) són totalment prescindibles.

- El fons de color gris no és necessari i dificulta la visualització de les etiquetes.

## 2. Principio de percepción fidedigna
La representació de les dades ha d’oferir una imatge fidel de la realitat, que faciliti el coneixement objectiu i complet de les dades i eviti que la persona usuària pugui obtenir interpretacions esbiaixades o parcials.
Les regles associades a aquest principi són:

- Representar les etiquetes de valors i eixos sempre horitzontalment. Les etiquetes verticals o inclinades dificulten molt la lectura de les dades.

Figura 2. Exemple del principi de percepció fidel

![Ejemplo del principio de percepción fidedigna](./images/2.jpg)

- Evitar trams amb composicions desiguals. Agrupar els valors numèrics en categories permet convertir dades numèriques en qualitatives, però mostrar agrupacions amb segments desiguals pot generar interpretacions allunyades de la realitat. En cas que existeixi una categoria residual amb molt poca freqüència, es pot establir un tram més ampli, sempre que l’agrupació no alteri les conclusions de l’anàlisi i s’indiqui degudament com a “resta de valors”.


> **Exemple d’agrupacions desiguals:**  
> Els gràfics següents mostren les mateixes dades, però els missatges es poden interpretar com a contradictoris. En el primer cas, les agrupacions desiguals promouen una falsa acumulació en els grups de més edat. El segon gràfic, amb agrupacions iguals, permet visualitzar una major concentració de casos en les agrupacions d’edat inferiors.
>
> Aquesta falsa percepció es produeix per l’agrupació dels joves en intervals d’edat amb pocs anys de diferència i els de més edat en grups que incorporen un espectre d’edat més ampli.

Figura 3. Exemple d’agrupació de les dades en trams

![Exemple d’agrupació de les dades en trams](./images/3.jpg)

- Evitar truncar els eixos (que no comencin en zero). Els eixos truncats generen una percepció distorsionada de les proporcions, afavorint una interpretació errònia de les pendents de creixement i decreixement.
El truncament dels eixos és una pràctica habitual que s’aplica quan els gràfics mostren un gran espai buit entre el zero i els primers valors de les sèries. El truncament condensa les dimensions d’un gràfic modificant l’escala d’un eix perquè no comenci en zero, sinó en un valor més proper als valors de les sèries.


>**Exemple de truncament d’eixos:** 
>
>Els dos gràfics següents mostren exactament la mateixa sèrie de dades, però els missatges que comuniquen són molt diferents. El gràfic amb l’eix vertical truncat afavoreix una interpretació de decreixements pronunciats i un creixement remarcable que no corresponen al patró real de les dades.

Figura 6. Exemple de truncament d’eixos  

![Exemple de truncament d’eixos](./images/4.jpg)

Evitar les columnes trencades (broken bars). Les columnes trencades no aporten informació sobre la realitat de les proporcions i generen una percepció errònia a l’hora d’interpretar les dades.





>**Ejemplo de eje roto:**
>
>Los siguientes gráficos muestran los mismos datos, pero en el gráfico
con columnas rotas se obtiene una imagen poco exacta de la proporción visual de la diferencia.
Figura 7. Exemple de trencament dels eixos d’un gràfic

![Exemple de truncament d’eixos](./images/Exemple%20de%20trencament%20dels%20eixos%20d’un%20gràfic.jpg)

- Mostrar de manera exhaustiva la totalitat de les categories. Una visualització en què només aparegui una part de les categories pot portar a pensar que les dades mostrades corresponen a la totalitat del fenomen d’estudi. Per això, és més adequat mostrar els valors de totes les categories, indicant clarament el contingut obert o tancat de cada tram. En cas que algunes categories siguin poc nombroses, es poden agrupar en una categoria residual tipus “altres” o “resta”.

>**Ejemplo de categorías no exhaustivas:**
>
>Los siguientes gráficos muestran el número
de visitantes categorizado por grupos de edades. El primer gráfico no es exhaustivo y
muestra únicamente las tres categorías más numerosas. La suma de estos tramos es de
500, una cifra inferior a la real. Este dato no corresponde con la totalidad de asistentes,
tal y como se muestra en el segundo gráfico.

Figura 8. Exemple de categories exhaustives (No exhaustiu)

![Exemple de truncament d’eixos](./images/Exemple%20de%20categories%20exhaustives.jpg)

- Presentar les dades ordenades per valors (rànquing) en ordre descendent és una bona opció per facilitar l’anàlisi i identificar les categories més nombroses de manera ràpida.
- No presentar les dades ordenades per valors (rànquing) quan siguin ordinals (amb un ordre intern ja establert), dades temporals o, en definitiva, dades amb un ordre de presentació lògic. L’ordre de presentació que no sigui de rànquing s’ha de mantenir de manera uniforme en el temps.

>**Exemple d’ordenació de dades amb una seqüència lògica:**
>
>Les dades que tenen un ordre natural, com per exemple els dies de la setmana, s’han de presentar seguint aquesta lògica i no mitjançant un rànquing en ordre descendent.

Figura 9. Exemple de presentació de categories amb un ordre lògic

![Exemple de presentació de categories amb un ordre lògic](./images/Exemple%20de%20presentació%20de%20categories%20amb%20un%20ordre%20lògic.jpg)


- Verificar la qualitat i la fiabilitat de la font de dades i el seu tractament, així com valorar prèviament les limitacions i la idoneïtat de les dades.

- L’ordre dels valors als eixos ha de ser de menor a major: de baix a dalt a l’eix Y (vertical) i d’esquerra a dreta a l’eix X (horitzontal).

- No utilitzar el degradat de colors com a únic element per mostrar proporcions. A diferència de les formes geomètriques, el color és un recurs molt menys precís per visualitzar una proporció, ja que costa determinar quan un color blau representa el doble que un altre color blau. Tanmateix, és un recurs molt útil per separar grups o remarcar diferències.

>**Exemple de dificultat en la quantificació de valors a partir dels colors:**
>
>El següent gràfic mostra una quantificació de valors en funció d’aplicar un paràmetre quantitatiu a la intensitat de brillantor de cada color en la mateixa proporció que el valor. És molt més fàcil quantificar proporcions a partir de la longitud de les barres que a partir de les intensitats del color. Tanmateix, no sempre és possible respectar aquest principi. Per exemple, en mapes que inclouen molts polígons, és difícil posar una etiqueta de valor per a cadascuna de les divisions, ja que la mida de la font hauria de ser necessàriament molt petita. En aquest cas, sí que estaria justificat l’ús del color per quantificar diferències.

Figura 10. Exemple de dificultat en la quantificació a partir del color

![Exemple de dificultat en la quantificació a partir del color](./images/Exemple%20de%20dificultat%20en%20la%20quantificació%20a%20partir%20del%20color.jpg)

## 3. Principi d’aprofitament de l’espai

L’aprofitament òptim de l’espai disponible és fonamental per garantir que la visualització sigui clara i eficient. Un ús inadequat de l’espai pot provocar gràfics amb massa buits, elements amuntegats o informació poc llegible.

**Recomanacions per a un bon aprofitament de l’espai:**

La densitat de la informació mostrada ha de ser l’adequada, aprofitant l’espai de manera que faciliti l’atenció i la comprensió correcta del missatge.

- Els gràfics han d’aprofitar al màxim l’espai disponible per mostrar la màxima quantitat d’informació rellevant sense sobrecarregar.
- Una visualització ha de justificar l’espai que ocupa; no té sentit mostrar un gràfic gran amb només dues dades quan una taula o un indicador seria més clar i compacte.
- Incorporar elements visuals de petit format, aplicable tant a gràfics com a altres objectes, com ara filtres d’interacció, botons, etc.
- Incorporar un alt nivell d’informació. Cal evitar visualitzacions que ocupin molt espai i mostrin poques dades.

> **Exemple de visualització poc condensada:**
>
> La visualització de l’esquerra mostra un gràfic de sectors amb dues dades, que ocupa pràcticament mitja pàgina. Aquesta poca informació s’acompanya d’un altre gràfic de barres amb quatre dades addicionals que ocupen l’espai de manera molt ineficient.
> Per contra, la visualització de la dreta mostra la informació de manera més adequada, acompanyada de textos explicatius i aportant dades útils per a la comprensió, en un espai més reduït.

Figura 11. Exemple d’aprofitament de l’espai

![Exemple d’aprofitament de l’espai](./images/Exemple%20d’aprofitament%20de%20l’espai.jpg)

Altres regles a tenir en compte en aquest principi d’aprofitament de l’espai són:

- Evitar espais buits. Reduir els marges i la separació entre capçaleres i títols, i en general, els espais morts.

- Optar per visualitzacions compostes (overlay/multi tier charts), per exemple, combinant barres, línies o taules amb mini gràfics (mini bars i sparkline amb escala correcta), i evitar mostrar aquests quadres amb els mateixos gràfics de manera independent i ocupant més espai si no és necessari.

- Utilitzar text dins del mateix gràfic. Contribueix a la correcta comprensió de les dades que el text explicatiu estigui més a prop de l’element al qual es refereix. La lletra ha de ser petita (8-10 punts) i s’han d’aprofitar els espais que deixin els diferents objectes de visualització.


## 4. Principi d’estructuració correcta ##

Una bona visualització no depèn únicament de l’encert dels seus objectes individuals, sinó de la composició de tots aquests elements. Així, la manera com s’estructuren i maqueten els diferents elements no és indiferent.
Les regles per aconseguir una estructuració adequada de la visualització són les següents:

- Estructurar el producte visual exhaustivament i organitzar-lo jeràrquicament a partir d’elements principals que es relacionin amb els elements secundaris o auxiliars. El missatge transmès ha de ser clar i complet a partir d’una estructura lògica.

>**Exemple d’estructura jeràrquica i de contingut exhaustiu:**
>
>La visualització de l’esquerra presenta un dèficit de coherència jeràrquica perquè el titular del gràfic es refereix únicament a un dels dos objectes mostrats. El gràfic del nombre d’assistents no serà coherent amb el títol de tota la composició. D’altra banda, l’afirmació del titular de “nivell molt alt d’ingressos” no queda avalada per les dades, ja que no existeix cap referent de comparació que permeti determinar si els ingressos són molt alts o no ho són.
>Per contra, en la visualització de la dreta existeix coherència amb la jerarquia del títol, no es barregen temàtiques i la informació està avalada per les dades que es mostren.

Figura 12. Exemple d’estructuració jeràrquica

![Exemple d’estructuració jeràrquica](./images/Exemple%20d’estructuració%20jeràrquica.jpg)

- Dissenyar la pàgina o pantalla tenint en compte els patrons de percepció i atenció previstos dels usuaris per transmetre el missatge de manera òptima. Diversos estudis sobre lectura de pantalla i usabilitat web (patrons visuals F, patrons Z, esquema de Gutenberg, triangle d’or d’eye tracking de Google) conclouen que l’atenció dels usuaris segueix un recorregut visual determinat i que no totes les parts de la pantalla reben la mateixa atenció. Fins i tot, existeix el risc que una part rellevant no sigui llegida.

El patró en Z mostra un recorregut que va de la part superior esquerra a la superior dreta, després fa una diagonal ràpida i finalitza a la zona inferior de la pantalla.

En el patró en F, o en triangle, el recorregut inicial és igual, amb una atenció més intensa a la part superior esquerra, que decreix en intensitat i desplaçament cap a la dreta a mesura que la vista baixa per la pantalla.

Per tot això, és especialment important aprofitar el quadrant superior esquerre de la pàgina per transmetre el missatge i captar l’atenció dels usuaris.

>**Estudio Eye tracking de Google:**
>
>Como ejemplo de lo que se indica en este punto, en
la imagen adjunta se muestra un mapa de calor del tiempo de atención en cada zona
de la página. A pesar de que esta atención depende del propio diseño de la página,
el tamaño de la fuente y el contraste de los elementos que se muestran se puede
apreciar que de forma natural la zona más caliente de la pantalla está situada en el
cuadrante superior izquierdo de la página. Este patrón, como puede intuirse, seguiría un
patrón de tipo F o triángulo.

Figura 13. Exemple de mapa de calor d’atenció visual

![Exemple de mapa de calor d’atenció visual](./images/Exemple%20de%20mapa%20de%20calor%20d’atenció%20visual.jpg)


- Indexar jerárquicamente con enlaces y marcadores los productos visuales con
diferentes partes, capítulos o pestañas, de modo que el movimiento y la navegabilidad
entre los distintos apartados sea fácil.

- Evitar la superposición de conceptos y métricas en una misma visualización (overlapping),
de forma que se evite que algunos elementos queden tapados por otros.

- Indicar la fuente de datos, la actualización y, en su caso, la metodología de elaboración de
los datos en el pie de página.








