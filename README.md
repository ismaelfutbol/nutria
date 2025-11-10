# nutriaC:\Users\SALA2-PC2\Desktop\nutriapp\regisro.html
<!DOCTYPE html>
<html lang="es_mx">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-sRIl4kxILFvY47J16cr9ZwB07vP4J8+LH7qKQnuqkuIAvNWLzeN8tE5YBujZqJLB" crossorigin="anonymous">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aplicación de Nutrición</title>
    <link rel="stylesheet" href="{{ url_for('static', filename='css/estilo.css') }}">
</head>
<body>
    <h1>Bienvenido a la Aplicación de Nutrición</h1>
    <a href="{{ url_for('register') }}">Registrarse</a>
    <a href="{{ url_for('profile') }}">Perfil de usuario</a>
</body>
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/js/bootstrap.bundle.min.js" integrity="sha384-FKyoEForCGlyvwx9Hj09JcYn3nv7wiPVlz7YYwJrWVcXK/BmnVDxM+D2scQbITxI" crossorigin="anonymous"></script>
</html>

<!DOCTYPE html>
<html lang="es_mx">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-sRIl4kxILFvY47J16cr9ZwB07vP4J8+LH7qKQnuqkuIAvNWLzeN8tE5YBujZqJLB" crossorigin="anonymous">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Registro de Usuario</title>
    <link rel="stylesheet" href="{{ url_for('static', filename='css/estilo.css') }}">
</head>
<body>
    <h1>Registro de Usuario</h1>
    <form method="POST">
        {{ form.hidden_tag() }}
        <div>{{ form.nombre.label }} {{ form.nombre() }}</div>
        <div>{{ form.email.label }} {{ form.email() }}</div>
        <div>{{ form.contrasena.label }} {{ form.contrasena() }}</div>
        <div>{{ form.confirmar_contrasena.label }} {{ form.confirmar_contrasena() }}</div>
        <div>{{ form.telefono.label }} {{ form.telefono() }}</div>
        <div>{{ form.fecha_nacimiento.label }} {{ form.fecha_nacimiento() }}</div>
        <div>{{ form.genero.label }} {{ form.genero() }}</div>
        <button type="submit">Registrarse</button>
    </form>
    <a href="{{ url_for('home') }}">Volver al inicio</a>
</body>
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/js/bootstrap.bundle.min.js" integrity="sha384-FKyoEForCGlyvwx9Hj09JcYn3nv7wiPVlz7YYwJrWVcXK/BmnVDxM+D2scQbITxI" crossorigin="anonymous"></script>
</html>
