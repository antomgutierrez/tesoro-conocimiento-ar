# 🚀 Guía de Despliegue - GitHub Pages

## 📋 Pasos para Desplegar el Proyecto

### 1. Preparar el Repositorio

```bash
# Inicializar git si no está inicializado
git init

# Agregar todos los archivos
git add .

# Hacer el primer commit
git commit -m "Initial commit: AR Treasure Hunt project"

# Conectar con el repositorio remoto (reemplaza con tu URL)
git remote add origin https://github.com/TU_USUARIO/tesoro-conocimiento-ar.git

# Subir al repositorio
git push -u origin main
```

### 2. Configurar GitHub Pages

1. **Ve a tu repositorio en GitHub**
2. **Haz clic en "Settings"** (Configuración)
3. **Desplázate hasta "Pages"** en el menú lateral
4. **En "Source"**, selecciona **"GitHub Actions"**
5. **Guarda la configuración**

**Nota**: El workflow actualizado usa las versiones más recientes de las acciones de GitHub (v4) para evitar problemas de compatibilidad.

### 3. Verificar el Despliegue

- **URL del juego**: `https://TU_USUARIO.github.io/tesoro-conocimiento-ar/`
- **Tiempo de despliegue**: 2-5 minutos después del push
- **Estado del despliegue**: Ve a la pestaña "Actions" en tu repositorio

### 4. Configuración Adicional

#### HTTPS (Recomendado)
- GitHub Pages soporta HTTPS automáticamente
- Para forzar HTTPS, ve a Settings > Pages > "Enforce HTTPS"

#### Dominio Personalizado (Opcional)
- Si tienes un dominio personalizado, agrégalo en Settings > Pages > Custom domain
- Actualiza el archivo `.github/pages.yml` con tu dominio

### 5. Estructura de Archivos para GitHub Pages

```
tesoro-conocimiento-ar/
├── .github/
│   ├── workflows/
│   │   └── deploy.yml          # Workflow de despliegue automático
│   └── pages.yml               # Configuración de Pages
├── markers/                    # Marcadores AR (.patt files)
├── index.html                  # Página principal del juego
├── generar-marcadores.html     # Generador de marcadores
├── README.md                   # Documentación
└── deploy-instructions.md      # Esta guía
```

### 6. Solución de Problemas

#### El sitio no se despliega
- Verifica que el workflow esté habilitado en Settings > Actions
- Revisa los logs en la pestaña "Actions"
- Asegúrate de que el archivo `index.html` esté en la raíz

#### Los marcadores no funcionan
- Verifica que los archivos `.patt` estén en la carpeta `markers/`
- Asegúrate de que el sitio esté en HTTPS (requerido para cámara)
- Prueba en diferentes navegadores

#### La cámara no funciona
- El sitio debe estar en HTTPS
- Verifica permisos del navegador
- Prueba en dispositivos móviles

### 7. Testing Local

Antes de desplegar, puedes probar localmente:

```bash
# Usando Python
python -m http.server 8000

# Usando Node.js
npx serve .

# Usando PHP
php -S localhost:8000
```

Luego ve a `http://localhost:8000`

### 8. Actualizaciones

Para actualizar el sitio:
1. Haz cambios en tu código local
2. Haz commit y push:
   ```bash
   git add .
   git commit -m "Update: descripción del cambio"
   git push
   ```
3. El despliegue se ejecutará automáticamente

### 9. Monitoreo

- **GitHub Actions**: Monitorea el estado del despliegue
- **GitHub Pages**: Ve el estado en Settings > Pages
- **Analytics**: Puedes agregar Google Analytics al `index.html`

---

## 🎯 Checklist de Despliegue

- [ ] Repositorio creado en GitHub
- [ ] Código subido al repositorio
- [ ] GitHub Pages habilitado
- [ ] Workflow de despliegue configurado
- [ ] Sitio accesible en la URL
- [ ] Marcadores AR funcionando
- [ ] Cámara funcionando en móvil
- [ ] HTTPS habilitado

---

**¡Tu juego de Realidad Aumentada estará listo para que Bruno, Maxi y Gonzalo lo prueben!** 🎓✨
