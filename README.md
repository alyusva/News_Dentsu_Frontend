# Plataforma de Noticias IA & Marketing - Frontend

Una aplicación web moderna para visualizar noticias de Inteligencia Artificial y Marketing, diseñada específicamente para el equipo de Dentsu. La plataforma permite filtrar, navegar y acceder a contenido relevante de la industria de forma intuitiva.

## 🚀 Características

- **Interfaz moderna** con React 18 y Tailwind CSS
- **Modo claro/oscuro** para mejor experiencia de usuario
- **Filtrado de noticias** por categorías (IA, Marketing, o ambas)
- **Diseño responsive** optimizado para todos los dispositivos
- **Navegación fluida** con React Router
- **Componentes reutilizables** con arquitectura modular

## 🛠️ Stack Tecnológico

- **Frontend**: React 18 + Vite
- **Estilos**: Tailwind CSS + PostCSS
- **Enrutado**: React Router v6
- **Iconos**: Lucide React
- **Backend**: Google Cloud Run (microservicios)
- **Analytics**: Vercel Analytics

## 📦 Instalación y Desarrollo

### Prerrequisitos
- Node.js 16+
- npm o yarn

### Configuración inicial

1. Clona el repositorio:
```bash
git clone https://github.com/alyusva/News_Dentsu_Frontend.git
cd News_Dentsu_Frontend
```

2. Instala las dependencias:
```bash
npm install
```

3. Configura las variables de entorno:
```bash
cp .env.example .env
```

4. Inicia el servidor de desarrollo:
```bash
npm run dev
```

La aplicación estará disponible en `http://localhost:3000`

## 🔧 Scripts Disponibles

```bash
npm run dev      # Servidor de desarrollo
npm run build    # Build de producción
npm run preview  # Preview del build
npm run lint     # Linting con ESLint
```

## 🏗️ Estructura del Proyecto

```
News_Dentsu_Frontend/
├── index.html                    # Punto de entrada HTML principal
├── package.json                  # Dependencias y scripts de npm
├── package-lock.json             # Lock de versiones exactas
├── README.md                     # Documentación del proyecto
├── .gitignore                    # Archivos ignorados por Git
├── vite.config.js                # Configuración de Vite
├── tailwind.config.js            # Configuración de Tailwind CSS
├── postcss.config.js             # Configuración de PostCSS
├── eslint.config.js              # Configuración de ESLint
├── vercel.json                   # Configuración de despliegue Vercel
│
├── public/                       # Archivos estáticos públicos
│   ├── vite.svg                  # Icono de Vite (favicon)
│   └── _redirects               # Reglas de redirección (SPA)
│
├── src/                          # Código fuente principal
│   ├── main.jsx                  # Punto de entrada de React
│   ├── App.jsx                   # Componente raíz con Router
│   ├── index.css                 # Estilos globales con Tailwind
│   │
│   ├── components/               # Componentes reutilizables
│   │   ├── Footer.jsx            # Footer común de la aplicación
│   │   ├── ThemeProvider.jsx     # Context Provider para tema claro/oscuro
│   │   │
│   │   └── ui/                   # Componentes de UI base
│   │       └── button.jsx        # Componente Button reutilizable
│   │
│   ├── pages/                    # Páginas principales de la aplicación
│   │   ├── HomePage.jsx          # Página de inicio (landing)
│   │   └── NewsPage.jsx          # Página de noticias con filtros
│   │
│   └── lib/                      # Utilidades y helpers
│       └── utils.js              # Funciones de utilidad (cn para clases)
│
└── node_modules/                 # Dependencias de npm (generado)
    └── ...                          # Miles de archivos de dependencias
```

## 🌐 Backend Integration

Esta aplicación funciona en conjunto con el backend desarrollado en Node.js que proporciona:

- 📡 **API de noticias**: Agregación de múltiples fuentes especializadas
- 🔍 **Filtrado inteligente**: Categorización automática por IA y Marketing  
- 🤖 **Procesamiento con IA**: Análisis y estructuración de contenido
- ☁️ **Despliegue**: Google Cloud Run para alta disponibilidad

> **Backend Repository**: [News_Dentsu_Backend](https://github.com/alyusva/News_Dentsu_Backend)

### Variables de Entorno Requeridas

```env
VITE_API_URL=your_backend_url_here
```

## 🎨 Funcionalidades

### Página de Inicio
- Landing atractivo con información del proyecto
- Navegación directa a las noticias
- Alternador de tema claro/oscuro

### Página de Noticias
- Lista de noticias con filtros dinámicos
- Enlaces externos a fuentes originales
- Badges de categorización
- Interfaz de carga con estados de error

## 🚀 Despliegue

El proyecto está optimizado para despliegue en plataformas modernas como Vercel, Netlify o similares. El build de producción se genera con:

```bash
npm run build
```

## Contacto

- GitHub: [@alyusva](https://github.com/alyusva)
- Proyecto: [News_Dentsu_Frontend](https://github.com/alyusva/News_Dentsu_Frontend)
