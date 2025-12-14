# 💼 Portfolio Multi-Página - Técnico en TI & Ciberseguridad

Portfolio profesional con **páginas separadas** para cada sección, optimizado para generar confianza y convertir visitas en clientes.

## 📂 Estructura del Sitio

```
portfolio/
├── index.html              # Página principal
├── sobre-mi.html           # Página "Sobre mí" completa
├── servicios.html          # Todos los servicios detallados
├── proyectos.html          # Índice de todos los proyectos
├── tecnologias.html        # Stack tecnológico
├── contacto.html           # Información de contacto
│
├── proyecto-cctv.html      # Proyecto individual: CCTV
├── proyecto-firewall.html  # Proyecto individual: Firewall
├── proyecto-automatizacion.html  # Proyecto individual: Bot
│
├── styles.css              # Estilos compartidos
└── script.js               # JavaScript compartido
```

## 🚀 Características

- ✨ Diseño moderno con estética cyberpunk/tech
- 📄 **Páginas separadas** para mejor organización
- 🔗 **Página individual por proyecto** con detalles completos
- 📱 100% Responsive (móvil, tablet, desktop)
- ⚡ Navegación fluida entre páginas
- 🎯 Optimizado para conversión (WhatsApp, email, LinkedIn)
- 🎨 CSS y JS compartidos entre páginas (fácil mantenimiento)

## 🌐 Despliegue en GitHub Pages

### Paso 1: Crear Repositorio

**Opción A - Sitio personal (Recomendado):**
```bash
# En GitHub: Crear repositorio con nombre: tu-usuario.github.io
```

**Opción B - Sitio de proyecto:**
```bash
# En GitHub: Crear repositorio con cualquier nombre (ej: portfolio)
```

### Paso 2: Subir Archivos

```bash
# 1. Inicializar repositorio en tu carpeta local
git init

# 2. Agregar todos los archivos
git add .

# 3. Hacer commit inicial
git commit -m "🚀 Portfolio multi-página inicial"

# 4. Crear rama main
git branch -M main

# 5. Conectar con GitHub
git remote add origin https://github.com/TU-USUARIO/tu-repositorio.git

# 6. Subir archivos
git push -u origin main
```

### Paso 3: Configurar GitHub Pages

**Para Opción A (tu-usuario.github.io):**
- Tu sitio estará automáticamente en: `https://tu-usuario.github.io`

**Para Opción B (repositorio de proyecto):**
1. Ve a tu repositorio en GitHub
2. Click en **Settings** → **Pages**
3. En **Source**, selecciona: **Deploy from a branch**
4. Branch: **main** / Folder: **/ (root)**
5. Click **Save**
6. Tu sitio estará en: `https://tu-usuario.github.io/nombre-repositorio`

## ✏️ Personalización Rápida

### 1. Información Personal

Busca y reemplaza en **TODOS los archivos HTML** (usa buscar global):

```
"Denilson" → Tu nombre
"San Luis Potosí, México" → Tu ciudad
"524444000000" → Tu número WhatsApp (formato internacional sin +)
"denilson.tech@gmail.com" → Tu email
"denilson-tech" → Tu usuario de GitHub
"/in/denilson-tech" → Tu perfil de LinkedIn
```

**Tip:** Usa el comando "Buscar en archivos" de tu editor (Ctrl+Shift+F en VS Code).

### 2. Cambiar Colores

Edita `styles.css` (líneas 1-12):

```css
:root {
    --accent: #00ff9f;        /* Color principal */
    --accent-dim: #00cc7f;    /* Color hover */
    /* ... */
}
```

**Paletas alternativas:**

Azul:
```css
--accent: #00d4ff;
--accent-dim: #00a8cc;
```

Morado:
```css
--accent: #a855f7;
--accent-dim: #9333ea;
```

Naranja:
```css
--accent: #ff6b35;
--accent-dim: #ff5722;
```

### 3. Actualizar Estadísticas

En `index.html` (línea ~60):
```html
<div class="stat-number">3+</div>  <!-- Cambia "3+" -->
<div class="stat-label">Años de experiencia</div>
```

### 4. Agregar Más Proyectos

**Opción 1 - Solo en el índice (proyectos.html):**
- Copia un bloque `<div class="project-card">` existente
- Modifica título, descripción y tecnologías

**Opción 2 - Con página individual:**
1. Duplica `proyecto-cctv.html` → `proyecto-nuevo.html`
2. Personaliza el contenido
3. Agrega el enlace en `proyectos.html`:
```html
<a href="proyecto-nuevo.html" class="project-card-link">
    ...
</a>
```

### 5. Agregar CV Descargable

1. Sube tu CV: `cv-denilson.pdf`
2. El enlace ya está en `sobre-mi.html` (línea ~155)
3. Verifica que funcione

## 📸 Agregar Imágenes a Proyectos

### Crear carpeta de imágenes:
```bash
mkdir images
```

### Estructura recomendada:
```
portfolio/
├── images/
│   ├── proyecto-cctv-1.jpg
│   ├── proyecto-firewall-1.jpg
│   └── ...
```

### Reemplazar en HTML:

**De esto:**
```html
<div class="project-image">📷</div>
```

**A esto:**
```html
<div class="project-image">
    <img src="images/proyecto-cctv-1.jpg" alt="Sistema CCTV" 
         style="width: 100%; height: 100%; object-fit: cover;">
</div>
```

## 📄 Estructura de Página de Proyecto

Cada proyecto individual tiene:
- ✅ Breadcrumb (navegación)
- ✅ Header con meta información
- ✅ Imagen hero grande
- ✅ Sección "Problema"
- ✅ Sección "Solución"
- ✅ Proceso de implementación
- ✅ Stack tecnológico
- ✅ Resultados medibles
- ✅ Testimonio del cliente (opcional)
- ✅ CTA para contacto

## 🎯 Ventajas de Páginas Separadas

1. **SEO mejorado:** Cada página tiene su propio título y meta descripción
2. **Carga más rápida:** Solo se carga el contenido necesario
3. **Mejor navegación:** URLs claras (ej: `/proyecto-cctv.html`)
4. **Fácil mantenimiento:** Editas solo la página que necesitas
5. **Escalable:** Agrega nuevos proyectos sin tocar otros archivos
6. **Profesional:** Similar a sitios web corporativos

## ✅ Checklist Pre-Lanzamiento

### Información Personal
- [ ] Nombre actualizado en todas las páginas
- [ ] Número de WhatsApp correcto
- [ ] Email actualizado
- [ ] Links a redes sociales funcionando

### Contenido
- [ ] Estadísticas de experiencia actualizadas
- [ ] Servicios corresponden a tu oferta real
- [ ] Al menos 3 proyectos detallados
- [ ] Página "Sobre mí" personalizada

### Técnico
- [ ] Todos los enlaces internos funcionan
- [ ] Navegación entre páginas fluida
- [ ] Responsive en móvil probado
- [ ] Botón WhatsApp con mensaje pre-escrito

### Opcional
- [ ] CV descargable agregado
- [ ] Imágenes de proyectos reales
- [ ] Favicon personalizado
- [ ] Google Analytics instalado

## 🔧 Comandos Git Útiles

```bash
# Ver estado de archivos
git status

# Agregar cambios
git add .

# Hacer commit
git commit -m "Descripción de cambios"

# Subir a GitHub
git push

# Ver historial
git log --oneline
```

## 🆘 Solución de Problemas

**Problema: Mi sitio no se actualiza en GitHub Pages**
- Espera 5-10 minutos después de hacer push
- Verifica que GitHub Pages esté habilitado (Settings → Pages)
- Revisa que el branch sea "main"

**Problema: Los estilos no se aplican**
- Verifica que `styles.css` esté en la misma carpeta que el HTML
- Limpia caché del navegador (Ctrl + Shift + R)

**Problema: La navegación no funciona**
- Verifica que todos los archivos HTML existan
- Revisa los nombres de archivos (sensibles a mayúsculas)

## 📊 Agregar Google Analytics (Opcional)

1. Crea cuenta en Google Analytics
2. Obtén tu código de seguimiento
3. Agrega antes del `</head>` en **cada HTML**:

```html
<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

## 🚀 Próximos Pasos Sugeridos

1. **Más proyectos:** Agrega 3-6 proyectos más con páginas individuales
2. **Blog:** Crea carpeta `blog/` con artículos técnicos
3. **Formulario:** Integra Google Forms o Formspree en contacto
4. **Testimonios:** Página dedicada a opiniones de clientes
5. **Certificaciones:** Página con badges y certificados
6. **Calculadora:** Herramienta para cotización automática

## 💡 Tips para Contenido

### Para Proyectos:
- Usa el formato **Problema → Solución → Resultados**
- Incluye números concretos (90% reducción, 30 días, 50+ equipos)
- Agrega tecnologías específicas (versiones, modelos)
- Menciona beneficios del cliente

### Para Sobre Mí:
- Destaca experiencia práctica sobre teórica
- Menciona proyectos actuales (SiiX EMS)
- Incluye habilidades técnicas concretas
- Agrega certificaciones relevantes

### Para Servicios:
- Enfócate en beneficios, no solo características
- Usa verbos de acción (Implemento, Configuro, Optimizo)
- Menciona para quién es cada servicio
- Incluye ejemplos concretos

## 📞 Soporte

Si tienes dudas:
1. Revisa este README
2. Busca en los archivos HTML (están comentados)
3. Verifica la consola del navegador (F12)

---

**Hecho con** ⚡ **para profesionales de TI que quieren destacar online**

## 📄 Licencia

Uso libre. Personalízalo como quieras para tu portfolio profesional.
