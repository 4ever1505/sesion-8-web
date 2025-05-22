<!DOCTYPE html>
<html lang="es">
    <head>
        <meta charset="UTF-8">
        <tittle>Dashboard con Bootstrap</tittle>
        <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/distcss/bootstrap.min.css"
                   rel="stylesheet">
    <style>
        body{
            font-family: Arial, Helvetica, sans-serif;
            background-color: #FFFBDE;
            margin: 0;
            padding: 20px;
            display: flex;/*organiza el contenido en formato de cajas flexsibles(horizontal)*/
        }
        *{
            box-sizing: border-box;/*borde y padding no aumenten su tamaño*/
        }
        /*estilos para el menú lateral*/
        .sidebar{
            width: 220px;/*ancho del menú*/
            background-color: blue;
            color: white;
            height: 100vb;/*altura completa de la ventana*/
            padding: 20px;
            position:fixed;/*mantiene fijo en su lugar al hacer scr*/
        }
        .sidebar h2{
            margin-top: 0;/*elimina el margen superior*/
            text-align: center;
        }
        .sidebar ul{
            list-style-type: none;/*elimine los puntos de la lista*/
            padding: 0;
        }
        .sidebar li{
            padding: 10px 0;
            border-bottom: 1px solid rgb(83, 149, 83);
            /*linea transparente divior*/
        }
        .sidebar ul li :hover {
            background-color: aqua /*color cuando pasa el mouse*/
            cursor pointer;/*cambiar el curso a mano*/
        }
        /*Contenedor principal del contenido a la derecha*/
        .main-content{
          margin-left: 220px;/*desplaza el contenido a la derecha*/
          padding: 20px;
          width: 100%;/*Ocupa el espacio de ancho disponible*/
        }
        h1{
            text-align: center;
            color: #90D1CA;
        }
        .dashboard{
            display: grid;/*Permite orgaizar los cards*/
            grid-template-columns: repeat(auto-fit, minmax(250px,1fr)),;/*ajustar columna como min, 250px*/
            gap: 20px;/*espacio entre tarjetas*/
            margin-top: 30px;/*espacio superior al titulo*/
        }
        .card {
            background-color: #129990;/*fondo blanco*/
            border-radius: 10px;/*dordes redondeados*/
            padding: 20px;
            box-shadow: 0 4px 8px rgb(73, 38, 38);/*efecto sombra*/
            text-align: center;
        }
        .card h2{
            margin: 10px 0;/*margen arriba y abajo*/
            color: #90D1CA;
        }
        .card p{
            font-size: 18px;
            color:chocolate
        }
    </style>
    </head>
    <body>
        <div class="sidebar">
        <h2>Menú Opciones</h2>
        <ul>
            <li>INICIO</li>
            <li>RESUMEN</li>
            <li>PRESTAMO</li>
            <li>SALIR</li>
        </ul>    
        </div>
        <!--Contenido principal-->
        <div class="main-content">
             <h1>Deshboard Financiero - Pestamo Bancario</h1>
        <div class="dashboard"><!--Contenedor general deshboard-->
            <div class="card"><!--Sustitulo de la tarjeta--> 
                 <h2>Cuota Inicial</h2>
                 <p>s./32,550</p>
            </div>
        <div class="card">
            <h2>Monto Financiero</h2>
            <p>s./122.450</p>
        </div>
        <div class="card">
            <h2>CUOTA MENSUAL</h2>
            <p>S./3,302.47</p>
        </div>
        </div>
        </div>
    </body>
</html>
