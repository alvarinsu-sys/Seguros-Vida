# Seguros de vida y rentas actuariales · dosier y calculadora

Autor: **Álvaro Insua Muñoz** · Máster en Ciencias Actuariales y Financieras (UC3M)

Página web autocontenida (un solo `index.html`) que reúne:

- **Dosier técnico**: fundamentos (ramo de vida, tablas de mortalidad, probabilidades, variable aleatoria valor actual, tabla de contingencia, momentos de orden k, funciones de conmutación), seguros de vida (temporal, capital diferido/dotal, mixto, vida entera, diferidos y combinaciones) y rentas (financieras y actuariales: temporales, vitalicias, fraccionadas y diferidas).
- **Calculadora**: tabla de contingencia completa, momentos de orden 1–4, varianza, asimetría, curtosis y coeficiente de variación de cualquier seguro o renta, gráficos de la distribución del valor actual y tabla de conmutación (qx, px, lx, dx, Dx, Nx, Sx, Cx, Mx, Rx, Ax, äx).
- **Ejercicios de clase** resueltos, erratas detectadas en los apuntes y glosario.

## Datos

Tablas PER2020 y PASEM2020 (1.er y 2.º orden, edades 0–120) de la Resolución de 17 de diciembre de 2020 de la DGSFP, [BOE-A-2020-17154](https://www.boe.es/buscar/doc.php?id=BOE-A-2020-17154). Ajuste generacional de las PER: `q = q_base · exp(−λx · (año nacimiento + x − 2012))`.

## Hipótesis de cálculo

- Pago del capital por fallecimiento al final del año de fallecimiento.
- Edades no enteras (rentas fraccionadas): interpolación lineal de lx dentro de cada año de edad.
- ω = 120: la vida entera desde x dura ω − x + 1 años.

## Publicar en GitHub Pages

1. Crea un repositorio y sube `index.html` (y este README).
2. En *Settings → Pages* elige la rama `main` y la carpeta raíz.
3. La página queda en `https://<usuario>.github.io/<repositorio>/`.

No necesita servidor ni compilación. Carga MathJax desde jsDelivr y las fuentes desde Google Fonts.

Herramienta de estudio; no sustituye las bases técnicas de una entidad aseguradora.
