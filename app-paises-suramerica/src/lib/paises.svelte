<script>
  export let pais;
  let p;
  /*[0]-Nombre_pais [1]-capital [2]-poblacion [3]-moneda [4]-area [5]-bandera*/
  const paises= {
    "colombia":["colombia", "Bogotá", "51.52 millones", "Peso colombiano", "1.142 millones km²", "bandera-colombia.jpg"],
    "venezuela":["venezuela", "Caracas", "28.2 millones", "Bolívar", "916.445 km²", "bandera-venezuela.jpg"],
    "ecuador":["ecuador", "Quito", "17.8 millones", "Dólar estadounidense", "256.370 km²", "bandera-ecuador.jpg"],
    "peru":["peru", "Lima", "32.7 millones", "Sol peruano", "1.285.216 km²", "bandera-peru.jpg"],
    "brasil":["brasil", "Brasilia", "214.3 millones", "Real brasileño", "8.51 millones km²", "bandera-brazil.jpg"],
    "argentina":["argentina", "Buenos aires", "46,23 millones", "peso argentino", "2 780 400 km²", "bandera-argentina.jpg"],
    "chile":["chile", "santiago de chile", "19,6 millones", "peso chileno", "756.626 km²", "bandera-chile.jpg"],
    "uruguay":["uruguay", "monte video", "3,423 millones", "peso uruguayo", "176.215 km²", "bandera-uruguay.jpg"],
    "bolivia":["bolivia", "sucre", "12,22 millones", "bolivano", "1,099 millones km²", "bandera-bolivia.jpg"],
    "paraguay":["paraguay", "asuncion", "6,781 millones", "Guaraní paraguayo", "406.752 km²", "bandera-paraguay.jpg"],

  }
  p = paises[pais];
</script>

<div class="main">
    <div class="col1">
        <img src="../src/assets/{p[5]}" alt="bandera_colombia" width="284" height="200">
    </div>
    <div class="col2">
        <div class="linea"><strong>Pais:</strong> {p[0]}</div>
        <div class="linea"><strong>Capital:</strong> {p[1]}</div>
        <div class="linea"><strong>Población:</strong> {p[2]}</div>
        <div class="linea"><strong>Moneda:</strong> {p[3]}</div>
        <div class="linea"><strong>extencion:</strong> {p[4]}</div>
    </div>
</div>  
<style>
    .main {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        grid-gap: 5px;
        grid-auto-flow: minmax(100px, auto);
        border-radius: 10px;
        border-style: solid;
        border-color: rgb(186, 190, 182);
        border-width: 2px;
        margin: left;
        width: 600px;
        box-shadow: 5px 5px 5px black;
        margin-right: 5px;
        margin-bottom: 10px;
    }
    .col1{
        grid-column: 1;
        grid-row: 1;
        margin: 5px;
        padding: 5px;
    }
    .col2{
        grid-column: 2;
        grid-row: 1;
        margin: 5px;
        padding: 5px;
        border-color: black;
        width: max-content;
    }
    strong{
        color: blue;
        font-weight: bolder;
    }
    .linea{
        font-size: 20px;
        margin-bottom: 18px;
    }
</style>