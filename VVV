<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Gráfico de Barras Dinámico</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
        }

        #contenedor {
            display: flex;
            justify-content: center;
            align-items: flex-end;
            height: 300px;
            width: 400px;
            margin: 50px auto;
            border: 2px solid #333;
        }

        .barra {
            width: 50px;
            margin: 5px;
            background-color: steelblue;
            transition: height 0.5s;
        }
    </style>
</head>
<body>

<h2>Gráfico de Barras Dinámico</h2>
<h2>HECHO POR: LUIS EDWIN FUENTES MARIN</h2>

<div id="contenedor"></div>

<script>
    const contenedor = document.getElementById("contenedor");
    const cantidadBarras = 5;
    let valores = [];

    // Crear barras
    for (let i = 0; i < cantidadBarras; i++) {
        const barra = document.createElement("div");
        barra.classList.add("barra");
        contenedor.appendChild(barra);
    }

    const barras = document.querySelectorAll(".barra");

    // Función para generar valores aleatorios
    function generarValores() {
        valores = [];
        for (let i = 0; i < cantidadBarras; i++) {
            valores.push(Math.floor(Math.random() * 91) + 10); // entre 10 y 100
        }
    }

    // Función para actualizar gráfico
    function actualizarGrafico() {
        generarValores();

        barras.forEach((barra, index) => {
            barra.style.height = valores[index] * 2 + "px"; // escala visual
        });
    }

    // Actualizar cada segundo
    setInterval(actualizarGrafico, 1000);

    // Primera carga
    actualizarGrafico();
</script>

</body>
</html>
