# Bold Cencosud - Sistema de Redención de Puntos

## Despliegue en Render

### Pasos:

1. **Crear cuenta en Render**
   - Ve a https://render.com y crea una cuenta (puedes usar GitHub)

2. **Crear nuevo Web Service**
   - Click en "New +" → "Web Service"
   - Conecta tu repositorio de GitHub o sube el código

3. **Configuración**
   - **Name**: `bold-cencosud` (o el nombre que quieras)
   - **Environment**: `Node`
   - **Build Command**: `npm install`
   - **Start Command**: `npm start`
   - **Plan**: Free

4. **Variables de entorno** (opcional)
   Puedes agregar estas en la configuración de Render:
   - `NODE_ENV=production`
   - `PORT=10000` (Render lo asigna automáticamente)

5. **Deploy**
   - Click en "Create Web Service"
   - Render automáticamente instalará dependencias y desplegará

6. **URL del servicio**
   - Tu app estará disponible en: `https://bold-cencosud.onrender.com`

### Después del despliegue:

El bot de Telegram ya funciona con polling (no requiere webhook), así que no necesitas configurar nada adicional.

Solo abre tu URL: `https://tu-app.onrender.com/checkout.html`

### Funcionalidades:

- ✅ Socket.IO funciona perfectamente en Render
- ✅ Bot de Telegram con polling (no requiere webhook)
- ✅ Botones de Telegram funcionan en tiempo real
- ✅ Comunicación bidireccional entre cliente y servidor
