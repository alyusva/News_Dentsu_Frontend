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
src/
├── components/          # Componentes reutilizables
│   ├── ui/             # Componentes de UI base
│   ├── Footer.jsx      # Footer de la aplicación
│   └── ThemeProvider.jsx # Proveedor de tema
├── pages/              # Páginas principales
│   ├── HomePage.jsx    # Página de inicio
│   └── NewsPage.jsx    # Página de noticias
├── lib/                # Utilidades y helpers
└── App.jsx             # Componente principal
```

## 🌐 API Integration

La aplicación se conecta a un backend desplegado en Google Cloud Run que proporciona:
- Agregación de noticias de múltiples fuentes
- Filtrado por categorías
- Procesamiento de contenido con IA

**Endpoint base**: `https://news-dentsu-backend-347262125232.europe-southwest1.run.app`

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

## 📄 Licencia

Proyecto privado para uso interno de Dentsu.
