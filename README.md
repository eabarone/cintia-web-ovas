# 📚 CINTIA Web OVAs

Repositorio de **Objetos Virtuales de Aprendizaje (OVAs)** interactivos en formato web, desarrollados para estudiantes de último año de bachillerato del programa técnico.

Cada OVA es una página HTML autocontenida con elementos visuales, actividades prácticas y consolas interactivas.

---

## 📁 Estructura del repositorio

```
cintia-web-ovas/
├── README.md               ← Estás aquí
├── context.md              ← Instrucciones para la IA (léelas antes de crear un OVA)
├── template/               ← Plantilla vacía lista para usar
│   └── index.html
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

1. Copia la carpeta `template/` y renómbrala con el tema del OVA.  
   Ejemplo: `semestre_1/tecnico/matematicas/trigonometria/`
2. Agrega el logo del OVA en `img/logo.webp`.
3. Agrega las imágenes QR de los recursos en `img/`.

### Paso 2 — Abre tu modelo de IA preferido

Puedes usar **ChatGPT, Gemini, Claude, Copilot** o cualquier otro modelo de lenguaje.

### Paso 3 — Dale el contexto al modelo

Copia y pega el contenido completo del archivo `context.md` al inicio de tu conversación con la IA, **antes de cualquier instrucción**.

> 💡 El archivo `context.md` contiene todas las reglas de diseño, estructura y comportamiento que la IA debe seguir para que el OVA sea consistente con los demás.

### Paso 4 — Haz tu solicitud

Después de pegar el contexto, escribe tu instrucción. Puedes usar la plantilla de prompt del archivo [`PROMPT_GUIDE.md`](./PROMPT_GUIDE.md).

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
- **No omitir** el plugin de accesibilidad al final del `<body>`:  
  `<script src="https://elens.ecodestudio.dev/elens.js"></script>`
- **Siempre incluir** las secciones: Introducción, Objetivos, Contenido, Actividades, Evaluación, Recursos, Bibliografía.
- Cada recurso debe tener su imagen QR en `img/`.

---

## 👥 Créditos

**Centro de Innovación en TIC para el apoyo de la Docencia — CINTIA**  
Universidad de Córdoba
