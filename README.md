# FIR Test

Tests infinitos con los exámenes oficiales del FIR (Farmacéutico Interno Residente).

- Si fallas, ves la respuesta correcta y una explicación breve, y sigues adelante.
- **Repetición espaciada**: las falladas vuelven a salir a las ~5 preguntas y, a medida que las aciertas, se espacian (25 → 80 → ×facilidad). Dominada = 3 aciertos seguidos.
- Progreso en el navegador, con exportar/importar `.json` como copia de seguridad.
- Teclado: `1`–`4` para responder, `Enter` para la siguiente.

## Datos
Cuadernos oficiales (versión 0) y plantillas definitivas del portal FSE del Ministerio de Sanidad.

| Convocatoria | Preguntas | Anuladas | Explicaciones |
|---|---|---|---|
| 2025 | 210 | 83, 110, 116, 120 | ✔ |
| 2024 | 210 | 53, 169, 172, 190 | pendiente |
| 2023 | 210 | 28, 47, 126, 132, 180, 190 | pendiente |
| 2022 | 210 | — | pendiente |
| 2021 | 210 | 100, 182, 194 | pendiente |

Formato de `data/<año>.json`: `{id, y, n, q, o[4], c (1-4, null = anulada), img, res (reserva), e (explicación)}`.

Las explicaciones son breves y de estudio; ante duda, manda la bibliografía.
