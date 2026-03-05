# 🌿 Serenidad

App de bienestar mental con respiración guiada, meditación y transformación de pensamientos mediante IA.

## Funcionalidades

- **Respiración consciente** — Técnicas 4-4, 4-7-8 y 5-5-5 con animación visual
- **Transformar pensamientos** — IA que reencuadra pensamientos negativos con compasión
- **Meditación** — Temporizador guiado de 3, 5 y 10 minutos
- **Estado de ánimo** — Recomendaciones personalizadas según cómo te sientes

## Despliegue

### Variables de entorno

En Vercel, añade la siguiente variable en **Settings → Environment Variables**:

```
ANTHROPIC_API_KEY=sk-ant-...
```

### Estructura

```
serenidad/
├── index.html        ← Frontend completo
├── api/
│   └── reframe.js    ← Serverless function (proxy seguro a Anthropic)
├── vercel.json       ← Configuración de Vercel
├── .gitignore
└── README.md
```

### Pasos

1. Clona o sube este repo a GitHub
2. Importa el proyecto en [vercel.com](https://vercel.com)
3. Añade `ANTHROPIC_API_KEY` en las variables de entorno
4. Despliega — cada `git push` redespliega automáticamente
