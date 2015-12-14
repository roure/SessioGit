# SessioGit
Sessió per explicar la meva experiència d'ús de Git i GitHub a l'assignatura de "Programació de dispositius mòbils". El públic destinatari són els professors d'informàtica del Tecnocamp

#Git i GitHub al Grau d’Enginyeria Informàtica del Tecnocampus

## Raons per usar Git a la titulació

1. **Git com a eina professional:**

    1. El control de versions s’usa MOLT al món professional. Està molt relacionada amb el desenvolupament àgil (però no únicament)

    2. Una forma que tenen els nostres estudiants de fer un portfoli

2. **Git com a eina docent**

    3. Permet jugar amb el codi sense por a fer-lo malbé

    4. Preparació d’exemples pas a pas. Permet veure l’evolució del codi pas a pas -> mostrar-ho en un cas concret

    5. Permet donar un codi base on treballar

    6. Permet donar feedback als estudiants

3. **Git com a eina treball en equip**

    7. Facilita molt la col·laboració

    8. S’han de fer molts commits i molt petits (pocs canvis) així es veu l’evolució

    9. S’han d’establir unes normes d’ús que respectin tots els usuaris

    10. El codi no és propietat de ningú en concret de l’equip

4. **Git com a eina de desenvolupament "Hand Solo" (individual)**

    11. Error de Intellij al compilar. Impossible de trobar. Al fer un diff vaig veure q havia canviat la versió d’unes llibreries la qual no tenia instal·lada

    12. Merdejar el codi. Al final no saps q has fet ni que has tocat. Marxa enrera molt fàcil

    13. Implementar una funcionalitat i comparar amb versió anterior x documentar

    14. Molt fàcil treballar des de diversos ordinadors. Sincronitzar amb el GitHub

    15. Elaborar un exemple pas a pas. 

## GitHub

El GitHub és un servei Git al núvol. Permet emmagatzemar els repositoris locals a un centralitzat i, el que és més important, permet compartir-los. Al final el GitHub és una xarxa social de programadors.

1. Font infinita d’exemples i de llibreries. Exemples: [https://github.com/lgvalle/Material-Animations](https://github.com/lgvalle/Material-Animations)

    1. Anar a graphs - members i veure qui ha fet els forks. Buscar-me a mi mateix 

    2. Anar a graphs - network i veiem tots els commits i les posteriors contribucions del fork. Realment fa xarxa i jo puc veure el que han fet la resta

    3. Anar a Code - commits i veiem qui ha fet cada commit, data i hora, el diff

2. GitHub education [https://education.github.com/](https://education.github.com/)

    4. Veure la pàgina i el student pack

    5. Veiem com demanar el pack

    6. Fem un upgrade de l’organització

    7. Mostrem els missatges que envien

3. GitHub education: mostrar la pestanya "Classroom Guide"

## Ús GitHub a Programació de Dispositius Mòbils (1era edició)

### Organization

1. El GitHub usa les organitzacions com a forma d’organitzar repositoris i usuaris.

2. Haurem de crear una organització per cada impartició de cada assignatura. Per tant el nom pot ser ProgramacióMobilsT15. Una organització es crea a partir del símbol "+" a la part de dalt

3. Demanem el upgrade d’una "organization account" i indicar la nostra organització. Al fer-ho pensar bé quants repositoris usarem ja que depenent de quants en demanem ens donaran un tipus d’upgrade o un altre

4. Hem de convidar els estudiants a participar de l’organització. Un cop convidats reben un correu i han de confirmar que hi volen ser inclosos. Jo ho he fet a ma però hi ha eines per automatitzar-ho (no ho he fet mai)

5. Un cop tenim els estudiants podem crear grups de pràctiques. En el meu cas he creat un sol grup amb tots els estudiants. 

6. Creem repositoris privats i els donem privilegis de només lectura. D’aquesta manera poden fer "**fork**" i “**clone**” de l’assignatura però no poden fer “push” (afegir nou codi). També podran fer “**pull request**” 

### L’assignatura

En aquest cas uso una "organization" que es diu TecnocampusMobils: [https://github.com/TecnocampusMobils](https://github.com/TecnocampusMobils)

1. Es pot posar un repositori públic que expliqui l’assignatura: [https://github.com/TecnocampusMobils/Android-Mobile-Programming-Syllabus](https://github.com/TecnocampusMobils/Android-Mobile-Programming-Syllabus)
Jo he afegit una llista amb tots els repositoris que hi poden trobar per tal d’organitzar-los una mica i fer una breu explicació

2. Cada repositori té un read.me file on es poden explicar coses vàries. Aquest fitxer usa un llenguatge de marques que és força senzill. [https://help.github.com/articles/markdown-basics/](https://help.github.com/articles/markdown-basics/)

### Repositoris pròpis com a exemple de codi 

Va molt bé per organitzar el codi i anar veient com va creixent l’aplicació. En aquest cas vaig fer un exemple d’una aplicació que serveix per crear notes al mòbil. De forma incremental vaig anar afegint funcionalitats:

1. Cada funcionalitat l’he fet en una branca nova. Veure com canvia el codi al fer un **checkout **de la branca o commit.

2. El proper cop faré una branca per cada funcionalitat a afegir i a l’acabar fer un merge al master

3. Un cop implementada la funcionalitat es pot plantejar com a pràctica: 

    1. Es crea branca nova: assigmentX

    2. Es fa un diff x veure tot el codi nou: fer l’exemple amb el NoteOne comparant la branca TwoPaneMode i la branca BBDD. Es veu diferències en fitxers ja exitents i fitxers completament nous

    3. Es posen comentaris tipus TODO i es fa un commit. Representa la pràctica resolta

    4. S’esborra el codi i commit. Representa l’enunciat de la pràctica

    5. Es crea un repositori privat nou i es publica la darrera versió esborrant tots els commits anteriors (detalls tècnics disponibles)

    6. En el meu cas una pràctica té la solució de la pràctica anterior: veure BBDD_1, assigment i multiple deletion

    7. Un repositori local pot tenir definits més d’un repositori remot. Facilita tenir-ne un pel professor i d’altres pels estudiants

4. Els exemples els tinc com a privats però penso un cop ben elaborats es poden posar públics. En el meu cas falta posar les explicacions i anar-les elaborant. Pot ser una forma de fe que els estudiants vagin corregint coses.

### Repositoris d’altri com a exemple de codi 

1. GitHub és una font interminable d’exemples. Es pot veure com n’hi ha un que no és meu: [https://github.com/TecnocampusMobils/android-material-travellist](https://github.com/TecnocampusMobils/android-material-travellist)

2. Hi he afegit una explicació. En els altres repositoris l’explicació és al moodle. És una cosa que aniré canviat. L’explicació està molt millor al GitHub que amagada en una intranet

### Lliurament de les pràctiques

Es pot organitzar de vàries maneres

1. Un únic repositori per tots els alumnes amb només permisos de lectura. 

    1. Estudiants fan un fork (al seu compte remot)

    2. fan un clon al repositori local, 

    3. resolen la pràctica i fan commits

    4. push al seu repositori remot, 

    5. fan un pull-request a l’original

    6. El darrer pas no és esrrictament necessàri ja q queda registrat els forks fets i com a propietaris originals tenim permisos de lectura

2. També podem tenir un repositori diferent per cada estudiant o grup d’estudiants i donar permisos d’escriptura. D’aquesta forma treballen en un únic repositori remot

### Correcció de les pràctiques

GitHub ens ofereix un munt d’eines per corregir les pràctiques: mostrar exemple Dylan: Assagment_Volley

1. Veure data i hora del pull request i de tots els commits

2. Veure tots els commits: propietari i hora

3. Fer diff amb el codi base i veiem tot el que ha fet de nou

4. Fer diff entre els commits del codi lliurat. Podem veure què ha fet cada estudiant

5. Fer diff entre pràctiques/pull request que sospitem còpia: anem al pull request, codi i a la part just a sobre del codi hi ha un botó petit que diu compare. Podem escollir l’origen i el destí: fork i branch/commit origen, fork i branch/commit destí

6. Podem fer comentaris al codi. Tant generals com dins del codi en línies concretes

7. Podem afegir **issues **per suggerir millores als estudiants

