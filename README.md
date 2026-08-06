# Fitalia Traslados — App de choferes (Android)

App web (Capacitor) que se compila a un APK de Android mediante GitHub Actions.

## Hito 1: generar el primer APK

### 1) Crear el repositorio
1. Entra a https://github.com y crea una cuenta (si no tienes).
2. Botón **New** → nombre `fitalia-traslados` → **Private** → **Create repository**.

### 2) Subir estos archivos
En el repo vacío: **Add file → Upload files** y arrastra TODO el contenido de esta
carpeta (incluida la carpeta `.github`). Luego **Commit changes**.
> Estructura esperada en el repo:
> ```
> package.json
> capacitor.config.json
> www/index.html
> .github/workflows/build-apk.yml
> ```

### 3) Compilar
- Ve a la pestaña **Actions** del repo.
- El flujo **Build APK** arranca solo al subir (o dale **Run workflow**).
- Espera a que termine en verde (~3-5 min).

### 4) Descargar e instalar
- Abre la corrida terminada → sección **Artifacts** → descarga **fitalia-traslados-apk**
  (es un .zip que trae `app-debug.apk`).
- Pásalo al teléfono Android e instálalo (activa **"Instalar apps de orígenes desconocidos"**
  cuando lo pida).
- Ábrela e inicia sesión como Roberto o Reinaldo.

Si el APK abre y puedes iniciar sesión, el Hito 1 está listo. Luego agregamos el
rastreo en segundo plano (Hito 2).
