# 📚 CINTIA Web OVAs

Repositorio de **Objetos Virtuales de Aprendizaje (OVAs)** interactivos en formato web, desarrollados para estudiantes de último año de bachillerato del programa técnico.

Cada OVA es una página HTML autocontenida con elementos visuales, actividades prácticas gamificadas e interactividad sin depender de frameworks externos.

---

## 📁 Estructura del repositorio

```
cintia-web-ovas/
├── README.md               ← Estás aquí
├── context.md              ← Instrucciones para la IA (léelas antes de crear un OVA)
├── PROMPT_GUIDE.md         ← Guía paso a paso para crear OVAs con IA
├── template/               ← Plantilla vacía oficial — punto de partida para nuevos OVAs
│   ├── index.html
│   └── img/
│       └── logo.webp       ← Logo compartido por todos los OVAs
├── semestre_1/
│   └── tecnico/
│       ├── matematicas/
│       └── programacion-web/
└── semestre_2/
    └── tecnico/
        ├── backend/
        │   ├── unidad_1/
        │   ├── unidad_2/
        │   └── Unidad_3/
        └── base_de_datos/
```

---

## 🚀 ¿Cómo crear un nuevo OVA con IA?

### Paso 1 — Prepara tu carpeta

1. Copia la carpeta `template/` completa (ya incluye `img/logo.webp`) y renómbrala con el tema del OVA.  
   Ejemplo: `semestre_1/tecnico/matematicas/trigonometria/`
2. Agrega las imágenes QR de los recursos en `img/` (una por cada recurso de la sección Recursos).

### Paso 2 — Prepara tu guía de aprendizaje

Escribe tu guía en formato Markdown con las secciones del OVA: Introducción, Objetivos, Contenido, Actividades, Recursos y Bibliografía. La IA usará esta guía como base y la enriquecerá con información de internet.

> 💡 No necesita ser perfecta — un esquema con los puntos clave es suficiente.

### Paso 3 — Dale el contexto a la IA

Si usas un **editor con agente integrado** (Windsurf, Cursor, Copilot, etc.), dile al agente:
```
Lee el archivo context.md que está en la raíz del repositorio y memoriza sus reglas.
```

Si usas un modelo web sin acceso a archivos (ChatGPT, Gemini, Claude web), copia y pega el contenido de `context.md` directamente en el chat.

### Paso 4 — Genera el OVA

Usa la plantilla de prompt del archivo [`PROMPT_GUIDE.md`](./PROMPT_GUIDE.md), pega tu guía de aprendizaje en el bloque indicado y envíalo. La IA generará el OVA completo.

### Paso 5 — Activa los recursos externos

El OVA generado tendrá **cards verdes** donde la IA sugiere videos o recursos externos. Para activarlas, busca el recurso y dile al agente en el chat:
```
Encontré un recurso para el recurso-ext-1. URL: [url] Título: [título]
```
El agente edita el archivo directamente — sin tocar código.

---

## ✅ OVA de referencia visual

El OVA **`introduccion-nodejs`** es el estándar de referencia para estilos y estructura:

```
semestre_2/tecnico/backend/unidad_2/introduccion-nodejs/index.html
```

Ante cualquier duda de cómo debe verse algo, consulta ese archivo.

---

## ⚠️ Reglas importantes

- **No modificar** el layout base (sidebar, mobile header, footer de créditos).
- **Gamificación obligatoria** en Contenido y Actividades: puntos, misiones, insignias, progreso visible.
- **No incrustar iframes** de YouTube ni inventar URLs — usar las cards de recurso externo.
- **No agregar controles de voz propios** — el plugin de accesibilidad ya los incluye.
- **No omitir** el plugin de accesibilidad al final del `<body>`:  
  `<script src="https://elens.ecodestudio.dev/elens.js"></script>`
- **Siempre incluir** las 7 secciones: Introducción, Objetivos, Contenido, Actividades, Evaluación, Recursos, Bibliografía.
- Cada recurso debe tener su imagen QR en `img/`.

---

## 👥 Créditos

**Centro de Innovación en TIC para el apoyo de la Docencia — CINTIA**  
Universidad de Córdoba
