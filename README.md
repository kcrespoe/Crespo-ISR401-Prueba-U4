# Prueba Práctica — Unidad IV — Ingeniería de Requisitos (ISR-401)

Sistema de Gestión de Pedidos — Validación, Gestión, Herramientas y Estándares de Requisitos.

**Estudiante:** Kleber Obed Crespo Espinoza
**Asignatura:** Ingeniería de Requerimientos
**Docente:** Ing. Gleiston Guerrero, Mg.
**Universidad:** Universidad Técnica Estatal de Quevedo — Facultad de Ciencias de la Computación — Ingeniería de Software, Cuarto Nivel

## Estructura del repositorio

```
.
├── main.tex          # Archivo principal LaTeX (carátula + P1-P10)
├── main.pdf           # PDF compilado (versión final)
└── README.md          # Este archivo
```

## Instrucciones de compilación

**Compilador:** `pdflatex` (TeX Live / MiKTeX)

**Dependencias (paquetes LaTeX):** `inputenc`, `babel` (spanish), `geometry`, `tikz` (con librerías `shapes`, `arrows.meta`, `positioning`, `calc`, `fit`, `backgrounds`), `longtable`, `booktabs`, `array`, `hyperref`, `enumitem`, `titlesec`, `xcolor`. Todos incluidos en una distribución estándar de TeX Live 2023+ o MiKTeX; no requieren instalación adicional.

**Archivo principal:** `main.tex`

**Orden de comandos** (se ejecuta dos veces para resolver referencias cruzadas y numeración):

```bash
pdflatex -interaction=nonstopmode main.tex
pdflatex -interaction=nonstopmode main.tex
```

Esto genera `main.pdf` en el mismo directorio.

### Compilar en Overleaf

1. Subir el contenido de este repositorio (o `main.tex`) como proyecto nuevo.
2. Overleaf detecta `main.tex` automáticamente como archivo raíz.
3. Compilar con el motor **pdfLaTeX** (configuración por defecto).

### Verificar reproducibilidad localmente

```bash
git clone https://github.com/usuario/repositorio.git
cd repositorio
pdflatex -interaction=nonstopmode main.tex
pdflatex -interaction=nonstopmode main.tex
```

Si `main.pdf` se genera sin errores, la compilación es reproducible.

## Contenido del documento

| Sección | Contenido |
|---|---|
| Carátula | Datos de identificación institucional y URL del repositorio |
| P1 | Diagrama de clases UML (TikZ) |
| P2 | Diagrama de actividades UML — "Registrar pedido" (TikZ) |
| P3 | Máquina de estados UML del ciclo de vida de Pedido (TikZ) |
| P4 | Tabla de consistencia entre P1–P3 e inconsistencia corregida |
| P5 | Especificación de 4 requisitos (2 FR, 2 NFR) con esquema de atributos |
| P6 | Priorización MoSCoW |
| P7 | Validación por inspección (ISO/IEC/IEEE 29148): defectos + retrabajo |
| P8 | Pruebas de aceptación trazadas |
| P9 | Matriz de trazabilidad |
| P10 | Gestión del cambio (CR-01) y línea base |
