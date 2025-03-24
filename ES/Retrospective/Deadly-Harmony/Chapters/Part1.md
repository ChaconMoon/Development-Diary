## Parte 1 - Bases del proyecto (Moviniento)

Cuando empezamos con el desarrollo del proyecto lo primero que se decidió era el aspecto que tendría, optamos por un aspecto típico de juegos de rol como Earthbound o Undertale y que el movimiento consistiría en 2 personajes de los cuales el jugador controla a uno y el otro le seguiría automáticamente como ocurre en juegos como Inazuma Eleven o Mario y Luigi

Afortunadamente aún tengo algunas imágenes de como fue el desarrollo del proyecto, aunque no son muy nítidas.

En ese primer día de desarrollo el juego se veia asi:


![Moviniento de los persoanjes](./Part1%20Media/Deadly%20Harmony%20Day%201.gif)

En este momento el movimiento era algo bastante tosco pero servía para hacerse a la idea de lo que queríamos.

Tras esto estuvimos un periodo de tiempo debatiendo sobre cómo sería el aspecto de los personajes, al final decidimos que usaremos como base sprites al estilo de Danganronpa y el resultado se quedo asi:

<div>
<img src="./Part1 Media/Character Desing.png" style="width:40%">
</div>

Una vez ya mejore el movimiento y creamos las animaciones el resultado fue este:

<div>
<img src="./Part1 Media/Moviniento final.gif" style="width:60%">
</div>

Ahora el movimiento queda mucho más orgánico, aunque aún hay algunos errores en las animaciones que se arreglaron durante el desarrollo

Las animaciones están hechas de forma que las animaciones no son un ciclo si que el juego "establece" hacia dónde te has quedado mirando y se deja en esa posición así conseguimos que la posición a la que mira los personajes se corresponda con el punto de interacción.

<div>
<img src="./Part1 Media/Dirección mirada.png" style="width:60%">
</div>

El diagrama que siguen las animaciones es este, cada dirección del flujo representa una dirección y estas siempre empiezan desde un poco común.

<div>
<img src="./Part1 Media/Animaciones base.png" style="width:80%">
</div>

El movimiento del personaje principal, al que controlas fue fácil de hacer, hacer el movimiento del compañero si fue más complicado ya que fue difícil hacer que se siga de forma que se sienta natural.

La solución por la que opté es que calculé si se encontraba en los mismos ejes que el personaje principal y en base a ellos se moviera si veía que se encontraba en un eje diferente.

<div>
<img src="./Part1 Media/Calculo de moviniento.png" style="width:60%">
</div>

Adicionalmente añadimos una opción de separarlos permitiendo que el segundo se quede parado donde está, pensamos que sería útil para algún momento de la historia pero finalmente nunca se usó.

<div>
<img src="./Part1 Media/Separación de personajes.png" style="width:60%">
</div>

Una vez se vuelve ha habilitar para que le siga al otro personaje una vez tu empieces el otro personaje se pondrá a seguirte hasta que vuelva a su posición.

<div>
<img src="./Part1 Media/Volver a seguir.gif" style="width:80%">
</div>

El cuadro blanco que se ve es lo que llamamos "Punto de interacción" representa el área en la que tiene que estar algo para que el personaje pueda interactuar con eso.

<div>
<img src="./Part1 Media/Punto de interacción.png" style="width:60%">
</div>

Cuando hable mas del desarrollo de la construcción del comportamiento del juego hablaré de cómo funcionan las interacciones, en el juego normal es invisible pero durante el desarrollo es útil verlo, este se posiciona siempre hacia donde esta la vista del personaje.

Ya he hablado de todo lo que fue hacer el movimiento base del juego, lo más básico del proyecto, pero esto es una visual novel, lo importante es la historia, el texto el próximo capítulo de este.