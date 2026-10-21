# HelpUs — prototipo móvil

## Sacar el APK (sin instalar nada)
1. Crea un repositorio en GitHub y sube **el contenido de esta carpeta** (incluida `.github`).
2. Entra a la pestaña **Actions** → "Construir APK" → espera ~5 min.
3. Abre la ejecución terminada y descarga **HelpUs-apk** (Artifacts). Dentro está `app-debug.apk`.
4. Pásalo al celular e instálalo (permite "instalar apps desconocidas").

## Sacar el APK en tu PC (Node 20 + Android Studio)
```
npm install
npx cap add android
npx capacitor-assets generate --android
npx cap sync android
npx cap open android   # Build > Build APK(s)
```

## Probar rápido en el navegador
Abre `www/index.html` y activa la vista móvil (F12 → icono de celular).
