# MisGastos - Personal Finance Tracker

Aplicación web Single-Page Application (SPA) para el seguimiento de finanzas personales, gestión de presupuestos y visualización analítica de gastos.

## 🏗️ Arquitectura y Funcionamiento Interno
El proyecto está diseñado siguiendo una arquitectura puramente frontend, priorizando la privacidad del usuario y la latencia cero:
- **Persistencia de Datos:** Utiliza la Web Storage API (localStorage) para mantener el estado de la aplicación entre sesiones (mg_gen_expenses y mg_gen_budget). Los datos nunca abandonan el dispositivo del cliente.
- **Motor de Renderizado:** Manipulación directa del DOM (Vanilla JavaScript) optimizada para evitar dependencias pesadas, garantizando tiempos de carga ultrarrápidos y bajo consumo de memoria RAM.
- **Visualización de Datos:** Implementa renderizado en <canvas> nativo con algoritmos matemáticos en 2D para generar gráficos de dona y barras dinámicos sin librerías de terceros excesivas.

## 📂 Estructura del Proyecto
`plaintext
mis-gastos-generales/
├── gastos-generales.html      # Estructura principal, estilos embebidos y lógica JS
├── misgastos_general.ico      # Icono de la aplicación
├── misgastos_general_icon...  # Recursos gráficos base
└── README.md
`

## ⚙️ Configuración y Despliegue
La aplicación es estática y no requiere entorno de ejecución (Runtime) en el servidor. 
1. Clonar el repositorio.
2. Abrir directamente gastos-generales.html en cualquier navegador web moderno.
