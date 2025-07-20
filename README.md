# TinderClone - Aplicación de Citas

Una aplicación de citas moderna construida con Next.js, Firebase y Tailwind CSS, diseñada para ser usada con App Inventor WebViewer.

## 🚀 Características

- **Splash Screen** con animación de entrada
- **Autenticación** con Google, Facebook y email/contraseña
- **Swipe de perfiles** estilo Tinder
- **Sistema de matches** y chats
- **Edición de perfil** con subida de fotos
- **Diseño responsive** y moderno
- **Integración con Firebase** para base de datos y autenticación

## 🛠️ Configuración

### 1. Configurar Firebase

1. Ve a [Firebase Console](https://console.firebase.google.com/)
2. Crea un nuevo proyecto
3. Habilita Authentication con Google, Facebook y Email/Password
4. Crea una base de datos Firestore
5. Configura Storage para las imágenes de perfil
6. Copia las credenciales de configuración

### 2. Variables de Entorno

Edita el archivo `.env.local` con tus credenciales de Firebase:

```env
NEXT_PUBLIC_FIREBASE_API_KEY=tu_api_key_aqui
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=tu_proyecto.firebaseapp.com
NEXT_PUBLIC_FIREBASE_PROJECT_ID=tu_project_id_aqui
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=tu_proyecto.appspot.com
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=tu_sender_id_aqui
NEXT_PUBLIC_FIREBASE_APP_ID=tu_app_id_aqui
```

### 3. Instalación

```bash
# Instalar dependencias
npm install

# Ejecutar en desarrollo
npm run dev

# Construir para producción
npm run build

# Exportar para GitHub Pages
npm run export
```

## 📱 Integración con App Inventor

1. Despliega la aplicación en GitHub Pages
2. En App Inventor, agrega un componente WebViewer
3. Configura la URL del WebViewer con tu URL de GitHub Pages
4. La aplicación funcionará completamente dentro del WebViewer

## 🔧 Estructura del Proyecto

```
src/
├── app/                    # Páginas de Next.js
│   ├── login/             # Página de login
│   ├── swipes/            # Página principal de swipes
│   ├── chats/             # Página de chats
│   ├── profile/           # Página de perfil
│   └── layout.tsx         # Layout principal
├── components/            # Componentes reutilizables
│   ├── SplashScreen.tsx   # Pantalla de inicio
│   ├── LoginForm.tsx      # Formulario de login
│   ├── SwipeCard.tsx      # Tarjeta de usuario para swipe
│   ├── ChatList.tsx       # Lista de chats
│   ├── ProfileForm.tsx    # Formulario de perfil
│   └── TabBar.tsx         # Barra de navegación
├── hooks/                 # Hooks personalizados
│   └── useRequireAuth.ts  # Hook para proteger rutas
└── lib/                   # Configuraciones
    └── firebase.ts        # Configuración de Firebase
```

## 🎨 Diseño

- **Colores principales**: Rosa y rojo (gradientes)
- **Tipografía**: Inter (Google Fonts)
- **Estilo**: Moderno, limpio, sin iconos externos
- **Responsive**: Optimizado para móviles

## 🔒 Seguridad

- Rutas protegidas con autenticación
- Validación de formularios
- Manejo seguro de archivos
- Variables de entorno para credenciales

## 📦 Despliegue en GitHub Pages

1. Configura tu repositorio en GitHub
2. Si tu repositorio no está en la raíz, descomenta y ajusta las líneas en `next.config.ts`:
   ```typescript
   basePath: '/nombre-de-tu-repo',
   assetPrefix: '/nombre-de-tu-repo/',
   ```
3. Ejecuta `npm run export`
4. Sube la carpeta `out/` a GitHub Pages
5. Tu aplicación estará disponible en `https://tu-usuario.github.io/tu-repo/`

## 🤝 Contribuir

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📄 Licencia

Este proyecto está bajo la Licencia MIT - ver el archivo [LICENSE](LICENSE) para más detalles.

## 🆘 Soporte

Si tienes problemas o preguntas:

1. Revisa la documentación de Firebase
2. Verifica que todas las variables de entorno estén configuradas
3. Asegúrate de que los servicios de Firebase estén habilitados
4. Revisa la consola del navegador para errores

---

¡Disfruta creando conexiones! 💕
# antesdelbaile
