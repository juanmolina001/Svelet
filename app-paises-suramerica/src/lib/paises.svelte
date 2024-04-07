<script>
  export let pais;
  let p;
  /*[0]-Nombre_pais [1]-capital [2]-poblacion [3]-moneda [4]-area [5]-bandera*/
  const paises= {
    "colombia":["colombia", "Bogotá", "51.52 millones", "Peso colombiano", "1.142 millones km²", "Flag_of_Colombia.svg"],
    "venezuela":["venezuela", "Caracas", "28.2 millones", "Bolívar", "916.445 km²", "Flag_of_Venezuela.svg"],
    "ecuador":["ecuador", "Quito", "17.8 millones", "Dólar estadounidense", "256.370 km²", "flag_of_Ecuador.svg"],
    "peru":["peru", "Lima", "32.7 millones", "Sol peruano", "1_285_216_km²", "268px_Flag_of_Peru_(state).svg.webp"],
    "brasil":["brasil", "Brasilia", "214.3 millones", "Real brasileño", "8.51 millones km²", "flag_of_Brazil.svg"]
  }
  p = paises[pais];
</script>

<div class="main">
    <div class="col1">
        <img src="../src/assets/{p[5]}" alt="" width="300" height="200">
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