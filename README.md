# FIR Test

Tests infinitos con los exámenes oficiales del FIR (Farmacéutico Interno Residente).

- Si fallas, ves la respuesta correcta y una explicación breve, y sigues adelante.
- **Repetición espaciada**: las falladas vuelven a salir a las ~5 preguntas y, a medida que las aciertas, se espacian (25 → 80 → ×facilidad). Dominada = 3 aciertos seguidos.
- Progreso en el navegador, con exportar/importar `.json` como copia de seguridad.
- Teclado: `1`–`4` para responder, `Enter` para la siguiente.

## Datos
Cuadernos oficiales (versión 0) y plantillas definitivas del Ministerio de Sanidad. 2021-2025 desde el portal FSE; 2016-2020 desde las copias que publica La Chuleta del FIR (el portal solo conserva cinco convocatorias). La plantilla de 2019 procede de consalud.es y se contrastó con una copia independiente: coinciden las 180 respuestas.

| Convocatoria | Preguntas | Anuladas | Explicaciones |
|---|---|---|---|
| 2025 | 210 | 83, 110, 116, 120 | ✔ |
| 2024 | 210 | 53, 169, 172, 190 | 202 de 206 |
| 2023 | 210 | 28, 47, 126, 132, 180, 190 | pendiente |
| 2022 | 210 | — | pendiente |
| 2021 | 210 | 100, 182, 194 | pendiente |
| 2020 | 185 | 89, 97, 102 | pendiente |
| 2019 | 185 | 40, 57, 89, 96, 166 | pendiente |
| 2018 | 235 | 57, 223 | pendiente |
| 2017 | 235 | 45, 46, 108, 125, 158, 185 | pendiente |
| 2016 | 235 | 41, 44, 92, 97, 141, 177, 207 | pendiente |

En total, **2125 preguntas oficiales** de 10 convocatorias. El examen tenía 225+10 preguntas hasta 2018, 175+10 en 2019-2020 y 200+10 desde 2021.

Formato de `data/<año>.json`: `{id, y, n, q, o[4], c (1-4, null = anulada), img, res (reserva), e (explicación)}`.

## Clasificación por asignatura
Cada pregunta lleva el campo `m` con el manual AFIR al que corresponde (12 manuales, según amireducacion.com). La clasificación es automática: palabras clave más la estructura por bloques del examen, que agrupa las preguntas por materia. Puede fallar en los bordes entre bloques.

| Manual | Preguntas |
|---|---|
| Fisiología, Fisiopatología y Anatomía | 436 |
| Farmacología | 256 |
| Microbiología | 241 |
| Bioquímica | 186 |
| Técnicas Instrumentales | 185 |
| Misceláneas | 184 |
| Química Farmacéutica | 154 |
| Biofarmacia | 126 |
| Inmunología | 104 |
| Biología Molecular | 95 |
| Físico-Químicas | 88 |
| Tecnología Farmacéutica | 70 |

Las explicaciones son breves y de estudio; ante duda, manda la bibliografía.
