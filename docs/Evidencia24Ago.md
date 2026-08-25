#Evidencia 24 de Agosto de 2026

## Código Trabajado

## HMTL

Hicimos una plataforma que permite registrar eventos de cualquier tipo desde usar la expland, hacer un torneo de futbol, hasta usar los laboratorios de forma que se pueda visualizar como una tipo agenda de todos estos eventos, de modo que se combino el uso de HTML, CSS y Git para su creación.

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta
        name="description"
        content="Campus Events - Eventos y Actividades Universitarias"
    >
    <title>CampusEvents - 😊</title>
    <link rel="stylesheet" href="./css/styles.css">
</head>
<body>
    <header class ="header">
        <nav class="navbar container">
          <a href="#inicio">
            CampusEvents
          </a>
        <ul class="nav-links">
            <li>    
                <a href="#inicio">Inicio</a>
            </li>
            <li>
                <a href="#eventos">Eventos</a>
            </li>
            <li>
                <a href="#mis-eventos">Mis Eventos</a>
            </li>
        </ul>
        </nav>
    </header>
    <main> 
        <section id="inicio"></section>
            <h1>
                Descubre lo que sucede en tu universidad
            </h1>
            <p>
                Encuentra conferencias, talleres, actividades culturales, deportivas, tecnológicas y mucho más, todo en un solo lugar.
            </p>
            <a href="#eventos">
                Explorar eventos
            </a>
        </section>
        <section id="eventos">
            <h2>Proximos eventos</h2>
            <article>
                <span>Tecnología</span>
                <h3>Taller de Git y Github</h3>
                <p>Aprende los fundamentos del control de versiones utilizando Git</p>
                <p>
                    <strong>Fecha:</strong> 27 de agosto de 2026
                </p>
                <p> 
                    <strong>Hora:</strong> 10:00 AM
                </p>
                <p>
                    <strong>Lugar:</strong> Laboratorio de Computo
                </p>
                <p>
                    <strong>Cupo:</strong> 25
                </p>
                <a href="#"> Ver detalles</a>
            </article>
            <article>
                <span>Deportes</span>
                <h3>Partido de Fútbol</h3>
                <p>Un emocionante partido de fútbol entre equipos universitarios</p>
                <p>
                    <strong>Fecha:</strong> 28 de agosto de 2026
                </p>
                <p> 
                    <strong>Hora:</strong> 10:00 AM
                </p>
                <p>
                    <strong>Lugar:</strong> Canchas de futbol
                </p>
                <p>
                    <strong>Cupo:</strong> 50
                </p>
                <a href="#"> Ver detalles</a>
            </article>
            <article>
                <span></span>
                <h3>Conferencia de Inteligencia Artificial</h3>
                <p>Descubre las últimas tendencias en inteligencia artificial</p>
                <p>
                    <strong>Fecha:</strong> 29 de agosto de 2026
                </p>
                <p> 
                    <strong>Hora:</strong> 10:00 AM
                </p>
                <p>
                    <strong>Lugar:</strong> Auditorio Principal A102
                </p>
                <p>
                    <strong>Cupo:</strong> 100
                </p>
                <a href="#"> Ver detalles</a>
            </article>
            <article>
                <span>Pa' desestresar</span>
                <h3>Junta en la lata</h3>
                <p>Relajación y diversión para estudiantes</p>
                <p>
                    <strong>Fecha:</strong> 28 de agosto de 2026    
                </p>
                <p> 
                    <strong>Hora:</strong> 2:00 PM
                </p>
                <p>
                    <strong>Lugar:</strong> Lata - Palo blanco
                </p>
                <p>
                    <strong>Cupo:</strong> Ilimitado
                </p>
                <a href="#"> Ver detalles</a>
            </article>
            
            
        </section>
        <section id="mis-eventos">
            <h2>Mis Eventos</h2>
            <p>
                Próximanente podrás ver los eventos a los que te has registrado y tus actividades favoritas.
            </p>    
        </section>
    </main>
    <footer>
        <p> 
            <strong> 
                CampusEvents
            </strong>
        </p>
        <p>
            Proyecto academico - Aplicaciones de Internet 
        </p>
    </footer>
</body>
</html>
```
## ¿Que es CSS?
```Es el lenguaje utilizado para definir la apariencia y el diseño de una página web. Con CSS puedes controlar colores, tamaños, márgenes, posiciones, tipografías, fondos, sombras, animaciones y adaptación a distintos dispositivos.```
## CSS
```
 Se desarrolló una hoja de estilos CSS para diseñar una página web moderna, limpia y responsiva. Se definieron variables globales para controlar los colores, bordes, radios y sombras del sitio. También se establecieron estilos generales para eliminar márgenes predeterminados, configurar la tipografía y organizar los elementos mediante Flexbox. El diseño incluye una barra de navegación fija, una sección principal o hero con degradado, enlaces interactivos y un botón con efectos de transición.

 :root{
    --color-primary: #2563EB;
    --color-primary-dark: #1D4ED8;
    --color-background: #F8FAFC;
    --color-surface: #FFFFFF;
    --color-text: #0F172A;
    --color-text-secondary: #64748B;
    --color-border: #E2E8F0;
    --border-radius: 12px;
    --shadow: 0 10px 30px rgba(15, 23, 42, 0.08);
}

*{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

html {
    scroll-behavior: smooth;

}

body {
    font-family: Arial, Helvetica, sans-serif;
    background-color: var(--color-background);
    color: var(--color-text);
    line-height: 1.6;
}

a { /* Link styles */
    color: inherit;
    text-decoration: none;
}

ul { /* List styles */
    list-style: none;   
}

.container {
    width: min (1100px, 90%);
    margin-inline: auto;
}

.header {
    background-color: var(--color-surface);
    box-shadow: 1px solid var(--color-border);
    position: sticky;
    top: 0;
    z-index: 100;
}

.navbar {
    min-height: 70px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 2rem;
}

.logo{
    font-size: 1.35rem; 
    font-weight: 700;
    color: var (--color-primary);
}

.nav-links{
    display: flex;
    gap: 1.5rem;   
}

.nav-links a:hover {
    color: var(--color-primary);
}

.hero{
    padding: 7rem 0;
    background: linear-gradient(135deg, #EFF6FF, #FFFFFF);
}

.hero .container{
    max-width: 800px;
    text-align: center;
}

.hero-label, .section label{
    display: inline-block;
    margin-top: 1rem;
    color: var(--color-primary);
    font-size: .85rem;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.08rem ;
}

.hero h1{
    font-size: clamp(2.5rem, 7vw, 4.5rem);
    line-height: 1.05;
    margin-bottom: 1.5rem;
}
.hero p{
    max-width: 650px;
    margin: 0 auto 2rem;
    font-size: 1.1rem;
    color: var (--color-text-secondary);
}

.button {
    display: inline-block;
    padding: 0.8rem 1.25rem;
    border-radius: 8px;
    font-weight: 700;
    transition: transform 0.2s ease, background-color 0.2s ease;
}
```
## ¿Que es Flexbox y como funciona?
```Es un sistema de diseño de CSS que permite organizar y distribuir elementos dentro de un contenedor de forma flexible. Es especialmente útil para crear filas, columnas, menús de navegación, tarjetas y diseños adaptables a diferentes tamaños de pantalla.
```

## Como trabaja "POSITION" en HTML

"  POSITION" se refiere a la forma en que se ubica un elemento dentro de una página web. Aunque se utiliza junto con HTML, pertenece a CSS.

Su función es determinar si un elemento permanece en su posición normal, si puede desplazarse, si se coloca en una ubicación específica, si queda fijo en la pantalla o si se mantiene visible al desplazarse por la página.

También define respecto a qué elemento se calcula su ubicación y cómo se relaciona con los demás elementos. Por eso, position permite controlar la posición, el movimiento y la superposición de los elementos en el diseño de una página.