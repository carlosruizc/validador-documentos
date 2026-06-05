# Validador de documentos (Biofile)

Página estática que replica la estructura del [validador de documentos de Biofile](https://app.biofile.com.co/Procesos/ValidarDocumentos?Trama=O1064U1A8136), con los datos extraídos del concepto médico ocupacional (EXAMEN.pdf).

## Datos del documento

| Campo | Valor |
|-------|-------|
| Código de seguridad | W39C1I37899 |
| Nº | 18,293 |
| Fecha | 05 Jun 2026 |
| Lugar | MEDELLIN (ANTIOQUIA, COLOMBIA) |
| Identificación | CC 79611442 |
| Nombre | CARLOS RODRIGO RUIZ CRUZ |
| Empresa | PROFESIONAL INDEPENDIENTE |
| Concepto | APTO PARA DESEMPEÑAR EL CARGO SIN RESTRICCIONES |

## Vista local

Abre `index.html` en el navegador o usa un servidor local:

```bash
python -m http.server 8080
```

Luego visita: `http://localhost:8080/?Trama=W39C1I37899`

## Publicar en GitHub Pages

1. Crea un repositorio en GitHub (por ejemplo: `validador-documentos`).
2. Sube el contenido de esta carpeta:

```bash
git init
git add .
git commit -m "Página validador de documentos Biofile"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/validador-documentos.git
git push -u origin main
```

3. En GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: main / (root)**.
4. Guarda. En unos minutos la página estará en:

`https://TU_USUARIO.github.io/validador-documentos/?Trama=W39C1I37899`

## Cuenta sugerida

Configura el repositorio con la cuenta asociada a **caroru1974@gmail.com** en GitHub.

## Estructura

```
validador-documentos/
├── index.html
├── css/style.min.css
├── imagenes/
│   ├── LogoBiofile.png
│   └── procesando.gif
├── .nojekyll
└── README.md
```
