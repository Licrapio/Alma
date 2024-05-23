# Alma
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <title>Tou oneírou</title>
    <meta name="description" content="">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="styles.css">
</head>
<style>
    body {
        font-family: 'Arial', sans-serif;
        background-color: #bdd899;
        margin: 0;
        padding: 20px;
        display: flex;
        flex-direction: column;
        align-items: center;
        box-sizing: border-box;
        overflow-y: auto; /* Permite desplazarse si el contenido es más alto que la ventana */
    }

    .container {
        display: flex;
        background-color: #ffffff;
        border-radius: 10px;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        overflow: hidden;
        max-width: 800px; /* Establece un ancho máximo */
        width: 100%;
    }

    .left-side {
        background-color: #d9fdcb;
        padding: 20px;
    }

    .left-side img {
        width: 150px;
        height: auto;
        border-radius: 10px;
    }

    .right-side {
        display: flex;
        flex-direction: column;
        width: 100%;
    }

    .color-box {
        padding: 20px;
        color: #0f0000;
        margin: 10px;
        border-radius: 10px;
        text-align: center;
    }

    .red {
        background-color: #629758d0;
    }

    .cards-container {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        grid-template-rows: repeat(4, auto);
        gap: 20px; /* Espacio entre tarjetas */
        margin-top: 2cm; /* Ajusta la distancia desde el contenedor principal */
    }

    .flip-card {
        background-color: transparent;
        width: 190px;
        height: 254px;
        perspective: 1000px;
        font-family: sans-serif;
    }

    .title {
        font-size: 1.5em;
        font-weight: 900;
        text-align: center;
        margin: 0;
    }

    .flip-card-inner {
        position: relative;
        width: 100%;
        height: 100%;
        text-align: center;
        transition: transform 0.8s;
        transform-style: preserve-3d;
    }

    .flip-card:hover .flip-card-inner {
        transform: rotateY(180deg);
    }

    .flip-card-front, .flip-card-back {
        box-shadow: 0 8px 14px 0 rgba(0,0,0,0.2);
        position: absolute;
        display: flex;
        flex-direction: column;
        justify-content: center;
        width: 100%;
        height: 100%;
        -webkit-backface-visibility: hidden;
        backface-visibility: hidden;
        border: 1px solid rgba(172, 214, 20, 0.733);
        border-radius: 1rem;
    }

    .flip-card-front {
        background: linear-gradient(120deg, rgba(166, 221, 77, 0.712) 60%, rgba(130, 179, 51, 0.712) 88%,
         rgb(216, 0, 0) 40%, rgba(98, 133, 42, 0.712) 48%);
        color: rgb(0, 0, 0);
    }

    .flip-card-back {
        background: linear-gradient(120deg, rgba(166, 221, 77, 0.712) 60%, rgba(130, 179, 51, 0.712) 88%,
         rgb(216, 0, 0) 40%, rgba(106, 150, 36, 0.712) 48%);
        color: rgb(0, 0, 0);
        transform: rotateY(180deg);
    }

    .card-image {
        width: 100%;
        height: 150px;
        object-fit: cover;
        border-bottom: 1px solid #ccc;
    }

    .card {
  width: fit-content;
  height: fit-content;
  background-color: rgb(238, 238, 238);
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 25px 25px;
  gap: 20px;
  box-shadow: 0px 0px 20px rgba(0, 0, 0, 0.055);
}

/* for all social containers*/
.socialContainer {
  width: 52px;
  height: 52px;
  border-radius: 50%;
  background-color: rgb(44, 44, 44);
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  transition-duration: .3s;
}
/* instagram*/
.containerOne:hover {
  background-color: #d62976;
  transition-duration: .3s;
}
/* twitter*/
.containerTwo:hover {
  background-color: #00acee;
  transition-duration: .3s;
}
/* linkdin*/
.containerThree:hover {
  background-color: #0072b1;
  transition-duration: .3s;
}
/* Whatsapp*/
.containerFour:hover {
  background-color: #128C7E;
  transition-duration: .3s;
}

.socialContainer:active {
  transform: scale(0.9);
  transition-duration: .3s;
}

.socialSvg {
  width: 17px;
}

.socialSvg path {
  fill: rgb(255, 255, 255);
}

.socialContainer:hover .socialSvg {
  animation: slide-in-top 0.3s both;
}

@keyframes slide-in-top {
  0% {
    transform: translateY(-50px);
    opacity: 0;
  }

  100% {
    transform: translateY(0);
    opacity: 1;
  }
}


</style>
<body>

    <div class="container">
        <div class="left-side">
            <img src="https://i.pinimg.com/564x/06/c2/bf/06c2bfe340ae7fb97d62b0abd45ac155.jpg" alt="Imagen">
        </div>
        <div class="right-side">
            <div class="color-box red">
                <h1>του ονείρου</h1>
                <p>De la mano de lo mistico</p>
            </div>
        </div>
    </div>

    <div class="cards-container">
         <!-- Repetimos la tarjeta -->
        <div class="flip-card">
            <div class="flip-card-inner">
                <div class="flip-card-front">
                    <img src="https://i.pinimg.com/564x/41/ee/0c/41ee0cb03654c0e84e6279f79b87b403.jpg" alt="Imagen" class="card-image">
                    <p class="title">Aracne</p>
                    <p>de linda damisela a monstruo</p>
                </div>
                <div class="flip-card-back">
                    <p><h6>Los comienzos de Aracne fueron como una bella dama con grandes habilidades para tejer.
                     Era tal su destreza que, en un arrebato de vanidad, presumió de ser más habilidosa que la diosa Atenea.
                     La diosa de la justicia ofendida entró en competencia con Aracne, pero, según cuenta 
                     Ovidio, no pudo superarla. Además, el tema escogido por la tejedora para la competición 
                     fue ofensivo para la diosa quien en un arrebato de ira transformó a Aracne en araña.
                     La criatura resultante del castigo sería mitad mujer y mitad araña y fue una muestra de 
                     la dureza de los dioses con los humanos si estos pretendían retarlos.</h6></p>
                </div>
            </div>
        </div>
        <!-- Repite la tarjeta -->
        <div class="flip-card">
            <div class="flip-card-inner">
                <div class="flip-card-front">
                    <img src="https://i.pinimg.com/564x/81/a1/b1/81a1b162f074516f1f1ac94298a32e35.jpg" alt="Imagen" class="card-image">
                    <p class="title">Basilisco</p>
                    <p>el ser mitológico de origen más rocambolesco</p>
                </div>
                <div class="flip-card-back">
                    <p><h6>El basilisco era conocido desde la antigüedad como «el pequeño rey» o «el rey de las serpientes»,
                         pues se pensaba que era el peor y el más terrible de todos los reptiles.  Plinio el Viejo lo describió 
                         como un dragón con cabeza de gallo y una cresta de oro (simulando una corona). En otras ocasiones fue 
                         descrito como una serpiente sin alas, pero lo cierto es que, con alas o sin ellas, los basiliscos son 
                         horribles reptiles muy temidos por su poder de petrificación</h6></p>
                </div>
            </div>
        </div>
         <!-- Repetimos la tarjeta -->
        <div class="flip-card">
            <div class="flip-card-inner">
                <div class="flip-card-front">
                    <img src="https://i.pinimg.com/564x/78/31/5e/78315e8c3939df4386e5468d9278188c.jpg" alt="Imagen" class="card-image">
                    <p class="title">Cerbero</p>
                    <p>el perro guardián del infierno</p>
                </div>
                <div class="flip-card-back">
                    <p><h6>Tiene dos puntos débiles: la miel y la música. Por increíble que parezca, la música amansa a las fieras
                         y, por lo tanto, también al cancerbero, que sólo ha sido vencido en dos ocasiones. Una de ellas fue Orfeo 
                         que encantó al cerbero con la música de su lira, dejándolo sumido en un dulce sueño. La segunda vez fue 
                         Hércules que, con su fuerza descomunal, logró doblegar al animal y encadenarlo, consiguiendo así uno de 
                         los “doce trabajos de Hércules”.</h6></p>
                </div>
            </div>
        </div>
        <!-- Repetimos la tarjeta -->
        <div class="flip-card">
            <div class="flip-card-inner">
                <div class="flip-card-front">
                    <img src="https://i.pinimg.com/564x/a8/b3/d6/a8b3d6052409694721039c9bc73a04a8.jpg" alt="Imagen" class="card-image">
                    <p class="title">La Hidra de Lerna</p>
                    <p>el monstruo de las cabezas a tutiplén</p>
                </div>
                <div class="flip-card-back">
                    <p><h6>En la mitología griega, la Hidra de Lerna era un antiguo y despiadado monstruo acuático gigante con la 
                        piel color pardo y el vientre amarillo blanquecino con ojos color ámbar y dientes muy afilados. Tenía forma
                        de serpiente policéfala y aliento venenoso a la que Heracles mató en el segundo de sus doce trabajos 
                        tapándose la boca y la nariz para no respirar el veneno de la hidra.</h6></p>
                </div>
            </div>
        </div>
        <!-- Repetimos la tarjeta -->
        <div class="flip-card">
            <div class="flip-card-inner">
                <div class="flip-card-front">
                    <img src="https://i.pinimg.com/564x/25/d8/84/25d884fa255e28a31ad6f94d6cc39d2c.jpg" alt="Imagen" class="card-image">
                    <p class="title">Arpía</p>
                    <p>la mujer ave de malas intenciones</p>
                </div>
                <div class="flip-card-back">
                    <p><h6>Las arpías estaban consideradas como un signo de mala suerte ya que podían aparecer de ningún sitio, robar,
                         destruir propiedades y sembrar el caos. Siempre estaban muertas de hambre y robaban comida o se comían a sus 
                         víctimas antes de llevárselas. Si una persona o una cosa desaparecía de repente sin rastro, la conclusión 
                         común era que una arpía se lo había llevado con sus afiladas garras.</h6></p>
                </div>
            </div>
        </div>
        <!-- Repetimos la tarjeta -->
        <div class="flip-card">
            <div class="flip-card-inner">
                <div class="flip-card-front">
                    <img src="https://i.pinimg.com/564x/f0/97/21/f09721cf22ae41a7095094744303ad33.jpg" alt="Imagen" class="card-image">
                    <p class="title">Centauro</p>
                    <p>mitad caballo y mitad hombre</p>
                </div>
                <div class="flip-card-back">
                    <p><h6>A pesar de su reputación bestial y lujuriosa, no todos los centauros recibían esta representación poco favorecedora, 
                        a no ser que hubieran bebido. Así que puede ser que fueran una metáfora admonitoria de los peligros a los que nos 
                        enfrentamos si olvidáramos el civismo y perdiéramos el control de nuestras facultades.</h6></p>
                </div>
            </div>
        </div>
        <!-- Repetimos la tarjeta -->
        <div class="flip-card">
            <div class="flip-card-inner">
                <div class="flip-card-front">
                    <img src="https://i.pinimg.com/564x/0f/3f/a1/0f3fa16266249cd4527ad936855599ba.jpg" alt="Imagen" class="card-image">
                    <p class="title">Mantícora</p>
                    <p>la devoradora de personas</p>
                </div>
                <div class="flip-card-back">
                    <p><h6>Las mantícoras no solo satisfacen su apetito matando a un único humano, sino que persiguen a varias personas a la vez,
                         y sienten un gran placer en la caza. Su forma favorita de atraer y cazar a su presa era ocultar su cuerpo en la hierba, 
                         de modo que desde la distancia, todo lo que los humanos podían ver era una cabeza humana. Engañados por esta imagen, los
                          humanos se acercaban a la mantícora y, antes de que se dieran cuenta, los atacaba y asesinaba.</h6></p>
                </div>
            </div>
        </div>
        <!-- Repetimos la tarjeta -->
        <div class="flip-card">
            <div class="flip-card-inner">
                <div class="flip-card-front">
                    <img src="https://i.pinimg.com/736x/58/a0/07/58a0078b947b6877e1a198e90a78fe58.jpg" alt="Imagen" class="card-image">
                    <p class="title">Quimera</p>
                    <p>el animal mitológico más poderoso</p>
                </div>
                <div class="flip-card-back">
                    <p><h6>Este ser es extremadamente peligroso durante un combate puesto que sus garras de león pueden desgarrar a cualquier 
                       hombre de un solo barrido. Puede utilizar también la cabeza y los cuernos de cabra para morder y golpear. Pero es su 
                       cabeza de dragón la más temida de las tres, sobre todo cuando lanza un cono de fuego.</h6></p>
                </div>
            </div>
        </div>
    </div>
    <div class="card">
        <a class="socialContainer containerOne" href="https://www.instagram.com/thel_iamm/">
          <svg viewBox="0 0 16 16" class="socialSvg instagramSvg"> <path d="M8 0C5.829 0 5.556.01 4.703.048 3.85.088 3.269.222 2.76.42a3.917 3.917 0 0 0-1.417.923A3.927 3.927 0 0 0 .42 2.76C.222 3.268.087 3.85.048 4.7.01 5.555 0 5.827 0 8.001c0 2.172.01 2.444.048 3.297.04.852.174 1.433.372 1.942.205.526.478.972.923 1.417.444.445.89.719 1.416.923.51.198 1.09.333 1.942.372C5.555 15.99 5.827 16 8 16s2.444-.01 3.298-.048c.851-.04 1.434-.174 1.943-.372a3.916 3.916 0 0 0 1.416-.923c.445-.445.718-.891.923-1.417.197-.509.332-1.09.372-1.942C15.99 10.445 16 10.173 16 8s-.01-2.445-.048-3.299c-.04-.851-.175-1.433-.372-1.941a3.926 3.926 0 0 0-.923-1.417A3.911 3.911 0 0 0 13.24.42c-.51-.198-1.092-.333-1.943-.372C10.443.01 10.172 0 7.998 0h.003zm-.717 1.442h.718c2.136 0 2.389.007 3.232.046.78.035 1.204.166 1.486.275.373.145.64.319.92.599.28.28.453.546.598.92.11.281.24.705.275 1.485.039.843.047 1.096.047 3.231s-.008 2.389-.047 3.232c-.035.78-.166 1.203-.275 1.485a2.47 2.47 0 0 1-.599.919c-.28.28-.546.453-.92.598-.28.11-.704.24-1.485.276-.843.038-1.096.047-3.232.047s-2.39-.009-3.233-.047c-.78-.036-1.203-.166-1.485-.276a2.478 2.478 0 0 1-.92-.598 2.48 2.48 0 0 1-.6-.92c-.109-.281-.24-.705-.275-1.485-.038-.843-.046-1.096-.046-3.233 0-2.136.008-2.388.046-3.231.036-.78.166-1.204.276-1.486.145-.373.319-.64.599-.92.28-.28.546-.453.92-.598.282-.11.705-.24 1.485-.276.738-.034 1.024-.044 2.515-.045v.002zm4.988 1.328a.96.96 0 1 0 0 1.92.96.96 0 0 0 0-1.92zm-4.27 1.122a4.109 4.109 0 1 0 0 8.217 4.109 4.109 0 0 0 0-8.217zm0 1.441a2.667 2.667 0 1 1 0 5.334 2.667 2.667 0 0 1 0-5.334z"></path> </svg>
        </a>
        
        <a class="socialContainer containerTwo" href="https://x.com/Plant_0ond">
          <svg viewBox="0 0 16 16" class="socialSvg twitterSvg"> <path d="M5.026 15c6.038 0 9.341-5.003 9.341-9.334 0-.14 0-.282-.006-.422A6.685 6.685 0 0 0 16 3.542a6.658 6.658 0 0 1-1.889.518 3.301 3.301 0 0 0 1.447-1.817 6.533 6.533 0 0 1-2.087.793A3.286 3.286 0 0 0 7.875 6.03a9.325 9.325 0 0 1-6.767-3.429 3.289 3.289 0 0 0 1.018 4.382A3.323 3.323 0 0 1 .64 6.575v.045a3.288 3.288 0 0 0 2.632 3.218 3.203 3.203 0 0 1-.865.115 3.23 3.23 0 0 1-.614-.057 3.283 3.283 0 0 0 3.067 2.277A6.588 6.588 0 0 1 .78 13.58a6.32 6.32 0 0 1-.78-.045A9.344 9.344 0 0 0 5.026 15z"></path> </svg>              </a>
          
        <a class="socialContainer containerFour" href="#">
          <svg viewBox="0 0 16 16" class="socialSvg whatsappSvg"> <path d="M13.601 2.326A7.854 7.854 0 0 0 7.994 0C3.627 0 .068 3.558.064 7.926c0 1.399.366 2.76 1.057 3.965L0 16l4.204-1.102a7.933 7.933 0 0 0 3.79.965h.004c4.368 0 7.926-3.558 7.93-7.93A7.898 7.898 0 0 0 13.6 2.326zM7.994 14.521a6.573 6.573 0 0 1-3.356-.92l-.24-.144-2.494.654.666-2.433-.156-.251a6.56 6.56 0 0 1-1.007-3.505c0-3.626 2.957-6.584 6.591-6.584a6.56 6.56 0 0 1 4.66 1.931 6.557 6.557 0 0 1 1.928 4.66c-.004 3.639-2.961 6.592-6.592 6.592zm3.615-4.934c-.197-.099-1.17-.578-1.353-.646-.182-.065-.315-.099-.445.099-.133.197-.513.646-.627.775-.114.133-.232.148-.43.05-.197-.1-.836-.308-1.592-.985-.59-.525-.985-1.175-1.103-1.372-.114-.198-.011-.304.088-.403.087-.088.197-.232.296-.346.1-.114.133-.198.198-.33.065-.134.034-.248-.015-.347-.05-.099-.445-1.076-.612-1.47-.16-.389-.323-.335-.445-.34-.114-.007-.247-.007-.38-.007a.729.729 0 0 0-.529.247c-.182.198-.691.677-.691 1.654 0 .977.71 1.916.81 2.049.098.133 1.394 2.132 3.383 2.992.47.205.84.326 1.129.418.475.152.904.129 1.246.08.38-.058 1.171-.48 1.338-.943.164-.464.164-.86.114-.943-.049-.084-.182-.133-.38-.232z"></path> </svg>
        </a>
      </div> 
      Autor:Perez Gomez Liam

</body>
</html>
