# 🎉 Guía para Publicar en Render

## Paso 1: Preparar tu repositorio Git

1. Abre la terminal en la carpeta de tu proyecto
2. Inicializa Git (si no lo has hecho):
   ```bash
   git init
   ```
3. Añade todos los archivos:
   ```bash
   git add .
   ```
4. Crea tu primer commit:
   ```bash
   git commit -m "Iniciar proyecto"
   ```
5. Crea un repositorio en GitHub y sube tu código:
   ```bash
   git branch -M main
   git remote add origin https://github.com/TU_USUARIO/regalo-dhara.git
   git push -u origin main
   ```

## Paso 2: Crear una cuenta en Render

1. Ve a [render.com](https://render.com)
2. Haz clic en **Sign Up** (Registrarse)
3. Elige **Sign up with GitHub** para conectar tu cuenta de GitHub
4. Autoriza Render para acceder a tus repositorios

## Paso 3: Crear un nuevo Servicio en Render

1. En el dashboard de Render, haz clic en **New +** (Nuevo +)
2. Selecciona **Web Service** (Servicio Web)
3. Conecta tu repositorio:
   - Selecciona el repositorio `regalo-dhara`
   - Haz clic en **Connect**

## Paso 4: Configurar el Servicio

Completa los campos de la siguiente manera:

- **Name**: `regalo-dhara` (o el nombre que prefieras)
- **Runtime**: `Node`
- **Build Command**: `npm install`
- **Start Command**: `npm start`
- **Plan**: Selecciona **Free** (Gratuito) si es tu primera vez

## Paso 5: Desplegar

1. Haz clic en **Create Web Service** (Crear Servicio Web)
2. Render comenzará a compilar e desplegar tu aplicación
3. Espera a que veas el mensaje "Your service is live 🎉"
4. Copia tu URL (por ejemplo: https://regalo-dhara.onrender.com)

## Paso 6: Verificar que todo funciona

1. Abre tu URL en el navegador
2. Verifica que:
   - Los botones funcionan correctamente
   - La música se reproduce
   - Los mensajes están en español ✅
   - Las imágenes GIF carguen correctamente

## ¡Listo! 🎊

Tu app está publicada y puedes compartir el enlace con quien quieras.

### Próximas actualizaciones

Si haces cambios en tu código:

1. Crea un commit con los cambios:
   ```bash
   git add .
   git commit -m "Descripción del cambio"
   ```
2. Sube a GitHub:
   ```bash
   git push
   ```
3. Render se actualizará automáticamente 🚀

---

## Troubleshooting

**¿La app no carga?**
- Verifica que `package.json` y `server.js` estén en la carpeta raíz
- Comprueba los logs en Render Dashboard

**¿Los archivos no se encuentran?**
- Asegúrate de que index.html, style.css, script.js y yes.html estén en la carpeta raíz

**¿El puerto no es correcto?**
- El servidor usa automáticamente el puerto asignado por Render via `process.env.PORT`
