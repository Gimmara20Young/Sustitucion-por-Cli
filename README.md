# Sustitucion-por-Cli
En base a la aplicación desarrollada(Diccionario) en la Sustitución de MongoDB por Redis, debe sustituir la arquitectura de ser una aplicación de línea de comandos a una aplicación web, basada en Flask
#Primer archivo lo llamaremos Formulario, el cual contendra el siguiente codigo
<!DOCTYPE html>
<html lang="es">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <meta http-equiv="X-UA-Compatible" content="ie=edge">
        <title>Formulario con Flask</title>
    </head>
    <body>
        <form method="POST" action="{{url_for('procesar')}}">
            <input name="palabra" required type="text" placeholder="Palabra">
            <br><br>
            <input name="significado" required type="text" placeholder="Significado">
            <br><br>
            <input type="submit" value="Enviar">
        </form>
    </body>
</html>

#nuestro segundo archivo se llamara mostrar, con el siguiente codigo.
<!DOCTYPE html>
<html lang="es">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <meta http-equiv="X-UA-Compatible" content="ie=edge">
        <title>Mostrar resultados</title>
    </head>
    <body>
        <strong>Palabra: </strong>{{palabra}}
        <br>
        <strong>Significado: </strong>{{significado}}
    </body>
</html>
