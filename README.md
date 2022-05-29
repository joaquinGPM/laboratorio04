<div align="center">
<table>
    <theader>
        <tr>
            <td><img src="https://github.com/rescobedoq/pw2/blob/main/epis.png?raw=true" alt="EPIS" style="width:50%; height:auto"/></td>
            <th>
                <span style="font-weight:bold;">UNIVERSIDAD NACIONAL DE SAN AGUSTIN</span><br />
                <span style="font-weight:bold;">FACULTAD DE INGENIERÍA DE PRODUCCIÓN Y SERVICIOS</span><br />
                <span style="font-weight:bold;">ESCUELA PROFESIONAL DE INGENIERÍA DE SISTEMAS</span>
            </th>
            <td><img src="https://github.com/rescobedoq/pw2/blob/main/abet.png?raw=true" alt="ABET" style="width:50%; height:auto"/></td>
        </tr>
    </theader>
    <tbody>
        <tr><td colspan="3"><span style="font-weight:bold;">Formato</span>: Guía de Práctica de Laboratorio / Talleres / Centros de Simulación</td></tr>
        <tr><td><span style="font-weight:bold;">Aprobación</span>:  2022/03/01</td><td><span style="font-weight:bold;">Código</span>: GUIA-PRLD-001</td><td><span style="font-weight:bold;">Página</span>: 1</td></tr>
    </tbody>
</table>
</div>

<div align="center">
<span style="font-weight:bold;">INFORME DE LABORATORIO</span><br />
<span>(formato estudiante)</span>
</div>


<table>
<theader>
<tr><th colspan="6">INFORMACIÓN BÁSICA</th></tr>
</theader>
<tbody>
<tr><td>ASIGNATURA:</td><td colspan="5">Programación Web 2</td></tr>
<tr><td>TÍTULO DE LA PRÁCTICA:</td><td colspan="5">Python</td></tr>
<tr>
<td>NÚMERO DE PRÁCTICA:</td><td>04</td><td>AÑO LECTIVO:</td><td>2022 A</td><td>NRO. SEMESTRE:</td><td>III</td>
</tr>
<tr>
<td>FECHA DE PRESENTACION:</td><td>29-May-2022</td><td>HORA DE PRESENTACION:</td><td colspan="3">21:00</td>
</tr>
<tr><td colspan="3">Integrantes:
<ul>
<li>Joaquín Gonzalo Paredes Mescco</li>
</ul>
</td>
<td>NOTA:</td><td colspan="2"></td>
</tr>
<tr><td colspan="6">DOCENTES:
<ul>
<li>Richart Smith Escobedo Quispe (rescobedoq@unsa.edu.pe)</li>
</ul>
</td>
</<tr>
</tdbody>
</table>


# Solución y resultados
## EJERCICIOS PROPUESTOS
-   En esta tarea usted pondrá en práctica sus conocimientos de programación en Python para dibujar un tablero de Ajedrez. 
-   La parte gráfica ya está programada, usted sólo tendrá que concentrarse en las estructuras de datos subyacentes.
-   Con el código proporcionado usted dispondrá de varios objetos de tipo Picture para poder realizar su tarea:
    ![Fichas de ajedrez](imagenes/picture.png)
-   Estos objetos estarán disponibles importando la biblioteca: [chessPictures](Tarea-del-Ajedrez/chessPictures.py) y estarán internamente representados con arreglos de strings que podrá revisar en el archivo [pieces.py](Tarea-del-Ajedrez/pieces.py)
-   La clase [Picture](Tarea-del-Ajedrez/picture.py) tiene un sólo atributo: el arreglo de strings img, el cual contendrá la representación en caracteres de la figura que se desea dibujar. 
-   La clase [Picture](Tarea-del-Ajedrez/picture.py) ya cuenta con una función implementada, no debe modificarla, pero si puede usarla para implementar sus otras funciones:
    -   _invColor: recibe un color como un caracter de texto y devuelve su color negativo, también como texto, deberá revisar el archivo [colors.py](Tarea-del-Ajedrez/colors.py) para conocer los valores negativos de cada caracter.

-   La clase [Picture](Tarea-del-Ajedrez/picture.py) contará además con varios métodos que usted deberá implementar:
    1.  verticalMirror: Devuelve el espejo vertical de la imagen
    2.  horizontalMirror: Devuelve el espejo horizontal de la imagen
    3.  negative: Devuelve un negativo de la imagen
    4.  join: Devuelve una nueva figura poniendo la figura del argumento al lado derecho de la figura actual
    5.  up: Devuelve una nueva figura poniendo la figura recibida como argumento, encima de la figura actual
    6.  under: Devuelve una nueva figura poniendo la figura recibida como argumento, sobre la figura actual
    7.  horizontalRepeat, Devuelve una nueva figura repitiendo la figura actual al costado la cantidad de veces que indique el valor de n
    8.  verticalRepeat Devuelve una nueva figura repitiendo la figura actual debajo, la cantidad de veces que indique el valor de n

-   Tenga en cuenta que para implementar todos estos métodos, sólo deberá trabajar sobre la representación interna de un Picture, es decir su atributo img.

-   Para dibujar una objeto Picture bastará importar el método draw de la biblioteca interpreter y usarlo de la siguiente manera:
    ```sh
    $ python3
    Python 3.9.2 (default, Feb 28 2021, 17:03:44) 
    [GCC 10.2.1 20210110] on linux
    Type "help", "copyright", "credits" or "license" for more information.
    ```
    ```sh
    >>> from chessPictures import *
    >>> from interpreter import draw
    pygame 1.9.6
    Hello from the pygame community. https://www.pygame.org/contribute.html
    >>> draw(rock)
    ```
    ![PyGame](imagenes/pygame_rock.png)

-   Ejercicios:

    -   Para resolver los siguientes ejercicios sólo está permitido usar ciclos, condicionales, definición de listas por comprensión, sublistas, map, join, (+), lambda, zip, append, pop, range.

        1.  Implemente los métodos de la clase Picture. Se recomienda que implemente la clase picture por etapas, probando realizar los dibujos que se muestran en la siguiente preguntas.
        2.  Usando únicamente los métodos de los objetos de la clase Picture dibuje las siguientes figuras (invoque a draw):

            *    (a) ![(a)](imagenes/ejercicio_02_a.png)

            *    (b) ![(b)](imagenes/ejercicio_02_b.png)

            *    (c) ![(c)](imagenes/ejercicio_02_c.png)

            *    (d) ![(d)](imagenes/ejercicio_02_d.png)

            *    (e) ![(e)](imagenes/ejercicio_02_e.png)

            *    (f) ![(f)](imagenes/ejercicio_02_f.png)

            *    (g) ![(g)](imagenes/ejercicio_02_g.png)

#



## II.	SOLUCIÓN DE CUESTIONARIO

-   ¿Qué son los archivos *.pyc?
-   ¿Para qué sirve el directorio __pycache__?
-   ¿Cuáles son los usos y lo que representa el subguión en Python?

## REFERENCIAS Y BIBLIOGRÁFIA RECOMENDADAS
-   
