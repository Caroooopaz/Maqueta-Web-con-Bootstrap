# 🧩 Desafío Maqueta Web con Bootstrap (Versión Cliente Exigente)

## 📌 Instrucciones Generales

Tu equipo ha sido asignado para construir una **sección específica** de una maqueta web. Esta maqueta **NO FUNCIONARÁ** si no respetas al pie de la letra los siguientes puntos:

1. **NO CAMBIES LOS NOMBRES DE LOS ARCHIVOS**: Si tu sección se llama `login.html`, ese es el nombre exacto que debes usar.
2. **NO MODIFIQUES EL NAVBAR NI EL FOOTER**: Solo debes preocuparte del **contenido central de tu sección**, como si fueras un diseñador contratado por un cliente con requerimientos estrictos.
3. **NO USES JS PERSONALIZADO**: Usa solamente el JavaScript incorporado en Bootstrap si lo necesitas.
4. Todo se ensamblará en un archivo `index.html`, el cual ya tiene definidos el **navbar**, el **footer**, y el **espacio central** para insertar cada una de las secciones.

---

## 🧱 Estructura base (la ve el grupo 1 y se replica en todos los archivos)

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Grupo X - Sección</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.7/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <!-- AQUI VA EL CONTENIDO DE TU SECCIÓN -->

</body>
</html>
```

---

## 🔗 Navbar (NO MODIFICABLE)

Todos los archivos usan el mismo `navbar`. Debe tener los siguientes enlaces en este orden y con **estos nombres exactos**:

```html
<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <div class="container">
    <a class="navbar-brand" href="#">MaquetaWeb</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav ms-auto">
        <li class="nav-item"><a class="nav-link" href="login.html">Login</a></li>
        <li class="nav-item"><a class="nav-link" href="register.html">Register</a></li>
        <li class="nav-item"><a class="nav-link" href="sesion1.html">Sesión 1</a></li>
        <li class="nav-item"><a class="nav-link" href="sesion2.html">Sesión 2</a></li>
        <li class="nav-item"><a class="nav-link" href="sesion3.html">Sesión 3</a></li>
        <li class="nav-item"><a class="nav-link" href="sesion4.html">Sesión 4</a></li>
      </ul>
    </div>
  </div>
</nav>
```

---

## 📥 Footer (NO MODIFICABLE)

```html
<footer class="bg-dark text-white text-center py-3">
  Todos los derechos reservados - 2025
</footer>
```

---

## ✅ Requerimientos por Grupo

### 👥 Grupo 1 – `index.html` (Página principal)

- Sección principal con bienvenida.
- Encabezado con título grande y subtítulo.
- Imagen de fondo o decorativa estilo “landing”.
- Tema de colores: **Primario (`bg-primary`), blanco y gris claro (`bg-light`)**.
- Solo deben insertar los contenidos del resto de los grupos dentro del `body`.

#### Aquí encontramos tres elementos: sección principal con bienvenida, encabezado grande y subtítulo, y tema de colores; **Primario (`bg-primary`), blanco y gris claro (`bg-light`)**.

```html
<section class="bg-primary text-white text-center py-5">
    <div class="container">
      <h1 class="display-4">Bienvenida a Maqueta Web</h1>
      <p class="lead">Diseñando experiencias digitales con creatividad y precisión</p>
    </div>
</section>
```

#### Imagen de fondo o decorativa estilo "landing":

```html
<section class="bg-light py-5">
    <div class="container">
      <img src="https://static.vecteezy.com/system/resources/previews/025/450/730/original/abstract-blue-background-with-lines-for-business-free-vector.jpg" alt="Diseño inspirador" class="img-fluid rounded mx-auto d-block">
    </div>
</section>
```

*Nota: recuerda que la imagen debe estar descargada en la misma carpeta de tu archivo index.html, sino, ésta no se visualizará.*









---







### 👥 Grupo 2 – `login.html`

- Formulario de inicio de sesión con campos:
  - Email
  - Contraseña
  - Checkbox "Recordarme"
- Fondo con clase `bg-light`, borde redondeado y sombra (`shadow`).
- Tema de colores: **gris claro (`bg-light`) y azul (`btn-primary`)**.
- Incluir ícono decorativo relacionado al acceso.

#### Email:

```html
<div class="mb-3">
  <label for="inputEmail" class="form-label">Correo electrónico</label>
  <input type="email" class="form-control" id="inputEmail" placeholder="nombre@ejemplo.com" required>
</div>
```

#### Contraseña:

```html
<div class="mb-3">
  <label for="inputPassword" class="form-label">Contraseña</label>
  <input type="password" class="form-control" id="inputPassword" placeholder="••••••••" required>
</div>
```

#### Checkbox "Recodarme":

```html
<div class="form-check mb-3">
  <input class="form-check-input" type="checkbox" id="rememberMe">
  <label class="form-check-label" for="rememberMe">
    Recordarme
  </label>
</div>
```

#### Fondo con clase `bg-light`, borde redondeado y sombra (`shadow`):

```html
<div class="bg-light p-5 rounded shadow" style="width: 100%; max-width: 400px;">
```

#### Tema de colores: **gris claro (`bg-light`) y azul (`btn-primary`)**:

```html
<button type="submit" class="btn btn-primary">Ingresar</button>
```

#### Incluir ícono decorativo relacionado al acceso:

```html
<i class="bi bi-person-circle fs-1 text-primary"></i>
```

---

### 👥 Grupo 3 – `register.html`

- Formulario de registro:
  - Nombre completo
  - Email
  - Contraseña
  - Repetir contraseña
  - Checkbox de aceptación de términos
- Estilo profesional: usa `card`, `mb-3`, `form-control`.
- Tema de colores: **verde (`btn-success`) y blanco**.
- Puedes agregar íconos relacionados a creación de cuenta.

#### Nombre completo

```html
<div class="mb-3">
  <label for="fullName" class="form-label">Nombre completo</label>
  <input type="text" class="form-control" id="fullName" required>
</div>
```

#### Email

```html
  <label for="email" class="form-label">Correo electrónico</label>
  <input type="email" class="form-control" id="email" required>
```

#### Contraseña

```html
<label for="password" class="form-label">Contraseña</label>
<input type="password" class="form-control" id="password" required>
```

#### Repetir contraseña

```html
<label for="confirmPassword" class="form-label">Repetir contraseña</label>
<input type="password" class="form-control" id="confirmPassword" required>
```

#### Checkbox de aceptación de términos

```html
<div class="form-check mb-3">
  <input type="checkbox" class="form-check-input" id="terms" required>
  <label class="form-check-label" for="terms">Acepto los términos y condiciones</label>
</div>                   
```

#### Estilo profesional: usa `card`, `mb-3`, `form-control`.

```html
/* Ejemplo de uso de estilo */
<div class="card-body">
  <h3 class="card-title text-center mb-4">
      <i class="bi bi-person-plus-fill text-success"></i> Formulario de Registro
  </h3>

<form>
  <div class="mb-3">
      <label for="fullName" class="form-label">Nombre completo</label>
      <input type="text" class="form-control" id="fullName" required>
</div>

```

#### Tema de colores: **verde (`btn-success`) y blanco**.

```html
<button type="submit" class="btn btn-success">
  <i class="bi bi-check-circle-fill"></i> Registrarse
</button>
```

### Incluir íconos relacionados a creación de cuenta.

```html
<i class="bi bi-person-plus-fill text-success"></i>
<i class="bi bi-check-circle-fill"></i>
```

---

### 👥 Grupo 4 – `sesion1.html` (Introducción)

- Contenido educativo dividido en 3 tarjetas:
  - ¿Qué es HTML?
  - ¿Qué es CSS?
  - ¿Qué es Bootstrap?
- Cada tarjeta debe tener botón “Leer más”.
- Tema de colores: **azul (`btn-outline-primary`) y blanco**.

---

### 👥 Grupo 5 – `sesion2.html` (Galería de proyectos)

- Tres tarjetas con imagen, título y descripción.
- Imágenes libres de proyectos ficticios.
- Cada tarjeta en columna (`col-12 col-md-4`) y dentro de `container`.
- Tema de colores: **neutro con acento en azul**.

---

### 👥 Grupo 6 – `sesion3.html` (Tabla de participantes)

- Tabla con tres columnas:
  - Nombre
  - Correo
  - Rol
- Usa clases `table table-striped`.
- Fondo blanco y container con márgenes (`mt-4`).
- Tema de colores: **gris (`table-secondary`) y blanco**.


```html
  <div class="container mt-4">

    <table class="table table-striped table-secondary">
      <thead>
        <tr>
          <th scope="col">#</th>
          <th scope="col">Nombre</th>
          <th scope="col">Correo</th>
          <th scope="col">Rol</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th scope="row">1</th>
          <td>Mark</td>
          <td>@mdo</td>
          <td>FrontEnd</td>
        </tr>
        <tr>
          <th scope="row">2</th>
          <td>Jacob</td>
          <td>@fat</td>
          <td>Backend</td>
        </tr>
        <tr>
          <th scope="row">3</th>
          <td>John</td>
          <td>@social</td>
          <td>ProductOwner</td>
        </tr>
      </tbody>
    </table>
  </div>
```

### 👥 Grupo 7 – `sesion4.html` (Formulario de contacto)

- Formulario con:
  - Nombre
  - Correo
  - Mensaje (textarea)
- Fondo gris claro (`bg-light`), bordes redondeados.
- Botón principal (`btn-primary`).
- Tema visual: **formal, con layout centrado y balanceado**.

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grupo 7 - Sección4</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.7/dist/css/bootstrap.min.css" rel="stylesheet">
    <link href="style.css" rel="stylesheet">
</head>
<body>

    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
        <div class="container">
            <a class="navbar-brand" href="#">MaquetaWeb</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item"><a class="nav-link" href="login.html">Login</a></li>
                    <li class="nav-item"><a class="nav-link" href="register.html">Register</a></li>
                    <li class="nav-item"><a class="nav-link" href="sesion1.html">Sesión 1</a></li>
                    <li class="nav-item"><a class="nav-link" href="sesion2.html">Sesión 2</a></li>
                    <li class="nav-item"><a class="nav-link" href="sesion3.html">Sesión 3</a></li>
                    <li class="nav-item"><a class="nav-link" href="sesion4.html">Sesión 4</a></li>
                </ul>
            </div>
        </div>
    </nav>

    <div class="container mt-5 d-flex justify-content-center">
        <form class="bg-light rounded p-4 shadow" style="width: 100%; max-width: 500px;">

            <h2 class="text-center">Contáctanos</h2>
            
            <div class="formulario mt-3 mb-3">
                <label for="inputNombre" class="form-label">Nombre</label>
                <input type="text" class="form-control" id="inputNombre" placeholder="Tu nombre">
            </div>

            <div class="formulario mt-3 mb-3">
                <label for="inputCorreo" class="form-label">Correo</label>
                <input type="email" class="form-control" id="inputCorreo" placeholder="nombre@example.com">
            </div>

            <div class="formulario mt-3 mb-3">
                <label for="textareaMensaje" class="form-label">Mensaje</label>
                <textarea class="form-control" id="textareaMensaje" rows="3" placeholder="Escribe tu mensaje aquí..."></textarea>
            </div>

            <div class="d-grid">
                <button type="submit" class="btn btn-primary">Enviar Mensaje</button>
            </div>

        </form>
    </div>

    <footer class="bg-dark text-white text-center py-3">
        Todos los derechos reservados - 2025
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.7/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>


## ⚠️ Advertencia Final

**Si cambias los nombres de los archivos o enlaces del navbar, el proyecto no funcionará.**  
Estas instrucciones simulan una entrega real para un cliente que **no acepta cambios arbitrarios**.

Tu misión es cumplir exactamente con lo solicitado. ¡Buena suerte! 💼
