# ✈️ JL Airlines – Aplicación Web (HTML & CSS)

## 📝 Descripción General

**JL Airlines** es una aplicación web simulada para una aerolínea, diseñada para su uso **exclusivo en dispositivos móviles**. Permite a los usuarios gestionar servicios clave de una aerolínea como la búsqueda de vuelos, check-in, registro, consulta de vuelos, y recuperación de contraseña.

Este sistema fue construido utilizando únicamente **HTML5 y CSS3**, bajo un enfoque **mobile-first**, restringiendo el acceso desde computadoras de escritorio mediante `media queries`.

## 📷 Demostración visual de la interfaz

![alt text](./MULTIMEDIA/Captura%20de%20pantalla.png)

---

## 📁 Estructura de Archivos

```
PROYECTO---HTML/
│
├── index.html
├── styles.css
├── busqueda-vuelos.html
├── check-in.html
├── crear-contrasena.html
├── mis-vuelos.html
├── recuperar-contrasena.html
├── registro.html
├── vista-inicio.html
├── vuelos-disponibles.html
├── /MULTIMEDIA/
│   ├── avion.png
│   ├── buscar vuelos.png
│   ├── check In.png
│   ├── LOGO.png
│   ├── LOGO SIN FONDO.png
│   ├── LOGO USER.png
│   ├── mis vuelos.png
│   └── ChatGPT Image May 13, 2025, 12_03_53 PM.png
```

---

## 🛠️ Tecnologías Utilizadas

- **HTML5** para la estructura del contenido
- **CSS3** para los estilos, diseño y media queries
- **Media Queries** para bloquear el acceso desde PC y permitir solo móviles

---

## 🧭 Funcionalidades por Página

| Archivo                     | Descripción Funcional                                                                 |
|----------------------------|----------------------------------------------------------------------------------------|
| `index.html`               | Página de inicio de sesión para el usuario                                            |
| `registro.html`            | Registro de usuario con datos personales y selección de ciudad                        |
| `recuperar-contrasena.html`| Solicitud de recuperación de contraseña vía correo electrónico                         |
| `crear-contrasena.html`    | Creación de nueva contraseña                                                          |
| `vista-inicio.html`        | Menú principal con acceso a búsqueda de vuelos, check-in y consulta de vuelos         |
| `busqueda-vuelos.html`     | Formulario para ingresar origen, destino y fechas de viaje                            |
| `vuelos-disponibles.html`  | Resultados simulados de vuelos con horarios y tarifas                                 |
| `check-in.html`            | Check-in para vuelos activos y contacto de emergencia                                 |
| `mis-vuelos.html`          | Listado de vuelos registrados por el usuario y su estado (A TIEMPO, ATERRIZÓ, etc.)  |

---

## 🎨 Diseño y Estilos

La interfaz utiliza clases CSS como `.container`, `.caja`, `.card`, `.ticket`, `.logo`, `.linea`, entre otras, para estructurar y embellecer el contenido.

**Colores dominantes**: Verde oscuro (`#073e0e`, `#097a38`)  
**Tipografía**: `'Roboto', sans-serif`

```css
background: linear-gradient(to right, #073e0e, #097a38);
```

---

## 📱 Diseño Responsive

El diseño fue desarrollado bajo un enfoque **mobile-first**. Para evitar el uso en PC, se usa esta lógica:

```css
@media (min-width: 768px) {
    body::after {
        content: "Esta aplicación está optimizada para dispositivos móviles.";
    }
    body > * {
        display: none !important;
    }
}
```

---

## 🖼️ Multimedia Utilizada

El directorio `/MULTIMEDIA/` contiene todos los íconos y logos visuales utilizados en las vistas:

- ✈️ `LOGO.png`, `LOGO SIN FONDO.png`: logos institucionales
- 👤 `LOGO USER.png`: icono de usuario
- 🛫 `avion.png`, `mis vuelos.png`, `buscar vuelos.png`, `check In.png`: íconos funcionales por módulo
- 🧠 `ChatGPT Image May 13, 2025...`: imagen de apoyo o referencia IA

---

## 📌 Limitaciones Actuales

| Componente               | Estado         |
|--------------------------|----------------|
| Backend                  | ❌ No implementado |
| Base de datos            | ❌ No implementado |
| Validaciones JavaScript | ❌ No integradas |
| Optimización móvil       | ✅ Completada |

---

## 👤 Autor

**Proyecto desarrollado por:** _Jeferson Lopez_  
**Fecha de entrega:** Mayo 2025  
**Licencia:** Uso educativo y demostrativo