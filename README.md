
# Despliegue de Landing Page en Render.com

Este README proporciona instrucciones paso a paso para desplegar tu landing page en [Render.com](https://render.com), un servicio de alojamiento en la nube moderno y sencillo de usar.

## Requisitos Previos

- Una cuenta en [Render.com](https://render.com) (puedes registrarte gratis)
- Tu código de landing page en un repositorio Git (GitHub, GitLab, etc.)
- Conocimientos básicos de Git

## Estructura de Archivos Recomendada

Para desplegar correctamente tu landing page en Render.com, deberías tener la siguiente estructura de archivos mínima:

```
landing-page/
├── index.html
└── README.md
```

## Pasos para el Despliegue

### 1. Preparar el Proyecto

1. Crea un nuevo repositorio en GitHub o GitLab
2. Guarda tu archivo `index.html` en la raíz del repositorio
3. Asegúrate de hacer commit y push de tus cambios al repositorio

### 2. Iniciar Sesión en Render.com

1. Ve a [Render.com](https://render.com)
2. Inicia sesión o crea una cuenta si aún no tienes una
3. Puedes registrarte utilizando tu cuenta de GitHub, GitLab o una dirección de correo electrónico

### 3. Crear un Nuevo Servicio Web Estático

1. En el Dashboard de Render, haz clic en el botón "New +"
2. Selecciona "Static Site" de las opciones disponibles

### 4. Conectar tu Repositorio

1. Selecciona el repositorio donde has subido tu landing page
   - Si es la primera vez, es posible que necesites conectar tu cuenta de GitHub o GitLab
   - Autoriza a Render para acceder a tus repositorios

### 5. Configurar el Servicio

Completa la configuración con los siguientes detalles:

- **Name**: Elige un nombre para tu sitio (por ejemplo, "mi-landing-page")
- **Branch**: La rama del repositorio que quieres desplegar (generalmente `main` o `master`)
- **Root Directory**: Deja en blanco si tu `index.html` está en la raíz del repositorio
- **Build Command**: No es necesario para un HTML estático simple, deja en blanco
- **Publish Directory**: `.` (punto) para indicar el directorio raíz

### 6. Opciones Avanzadas (Opcional)

1. Haz clic en "Advanced" para ver opciones adicionales
2. Aquí puedes configurar:
   - Variables de entorno (no necesarias para esta landing page)
   - Dominio personalizado (disponible en planes de pago)
   - Auto-deploy settings (activado por defecto)

### 7. Crear y Desplegar

1. Haz clic en "Create Static Site"
2. Render comenzará a desplegar tu sitio automáticamente
3. Espera a que el proceso de despliegue termine (normalmente toma menos de un minuto)

### 8. Acceder a tu Sitio

Una vez completado el despliegue:

1. Verás un enlace a tu sitio con un dominio `*.onrender.com`
2. Haz clic en el enlace para ver tu landing page en vivo

## Personalización del Dominio (Opcional)

Si deseas usar un dominio personalizado:

1. Ve a la página de tu sitio en el dashboard de Render
2. Navega a la pestaña "Settings"
3. Desplázate hasta "Custom Domain"
4. Sigue las instrucciones para configurar tu dominio personalizado
   - Necesitarás acceso a la configuración DNS de tu dominio
   - Render proporciona instrucciones específicas para cada proveedor de dominio

## Actualizaciones Futuras

Para actualizar tu landing page:

1. Realiza cambios en tu archivo `index.html` localmente
2. Haz commit y push de estos cambios a tu repositorio
3. Render detectará automáticamente los cambios y volverá a desplegar tu sitio
4. Los cambios estarán visibles en pocos minutos

## Solución de Problemas Comunes

### El sitio no se actualiza después de un push

- Verifica en el dashboard de Render que el despliegue automático esté activado
- Comprueba los logs de despliegue para ver si hay errores
- Intenta un despliegue manual haciendo clic en "Manual Deploy" > "Deploy latest commit"

### Problemas con rutas de archivos

- Si utilizas CSS o JavaScript en archivos separados, asegúrate de usar rutas relativas correctas
- Para sitios estáticos simples, considera incluir el CSS dentro del archivo HTML como se ha hecho en este ejemplo

### Problemas de visualización

- Usa la consola del navegador para detectar errores
- Verifica que las rutas a las imágenes sean correctas
- Comprueba que el sitio sea responsivo probándolo en diferentes dispositivos

## Recursos Adicionales

- [Documentación oficial de Render para sitios estáticos](https://render.com/docs/static-sites)
- [Configuración de dominio personalizado en Render](https://render.com/docs/custom-domains)
- [Precios y planes de Render](https://render.com/pricing)

---

Con este README tienes todas las instrucciones necesarias para desplegar tu landing page en Render.com. Si tienes alguna pregunta adicional o necesitas ayuda con el proceso de despliegue, no dudes en consultar la documentación oficial de Render o contactar con su soporte.