# MISAGI Sistema de Flota

## ⚡ Instrucciones para publicar en GitHub Pages

### Paso 1 — Crear repositorio
1. Ve a https://github.com/new
2. Nombre: `misagi-flota`
3. Público ✓ → "Create repository"

### Paso 2 — Subir archivos
1. Arrastra estos 2 archivos al repo:
   - `index.html`
   - `LOGOMSG.png`

### Paso 3 — Activar GitHub Pages
1. Settings → Pages
2. Source: Deploy from branch → `main`
3. Guardar

### Paso 4 — Tu URL será:
`https://TU_USUARIO.github.io/misagi-flota`

## ⚠️ Firebase Firestore — Reglas necesarias
En Firebase Console → Firestore → Reglas:
```
rules_version = '2';
service cloud.firestore {
  match /databases/{database}/documents {
    match /{document=**} {
      allow read, write: if true;
    }
  }
}
```

## ⚠️ IMPORTANTE
**NO abras index.html directamente** (doble click). 
Debe abrirse desde GitHub Pages o un servidor HTTP.
