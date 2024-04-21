# mandingo
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>gei</title>
<style>
    /* Estilo para el cuadro de diálogo emergente */
    .popup {
        display: none;
        position: fixed;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        background-color: #c780c1;
        padding: 20px;
        border: 2px solid #333;
        border-radius: 5px;
        z-index: 1000;
    }
</style>
</head>
<body>

<!-- Botón -->
<button id="mostrarBoton">piquele aqui</button>

<!-- Cuadro de Diálogo -->
<div id="miCuadroDialogo" class="popup">
    <p>puto el que lo lea :D</p>
    <button id="cerrarBoton">cerrar</button>
</div>

<script>
    // Función para mostrar el cuadro de diálogo
    function mostrarDialogo() {
        var cuadroDialogo = document.getElementById("miCuadroDialogo");
        cuadroDialogo.style.display = "block";
    }

    // Función para cerrar el cuadro de diálogo
    function cerrarDialogo() {
        var cuadroDialogo = document.getElementById("miCuadroDialogo");
        cuadroDialogo.style.display = "none";
    }

    // Evento al hacer clic en el botón para mostrar el cuadro de diálogo
    document.getElementById("mostrarBoton").addEventListener("click", mostrarDialogo);

    // Evento al hacer clic en el botón de cerrar dentro del cuadro de diálogo
    document.getElementById("cerrarBoton").addEventListener("click", cerrarDialogo);
</script>

</body>
</html>
