# Retroalimentación — Taller evaluativo 03 (NumPy)

**Estudiante:** Santiago Rodríguez Muñoz · **Taller:** Taller evaluativo 03 — NumPy
**Fecha límite:** 2026-10-26 23:59 · **Versión revisada:** commit `12f1d2b`

Excelente trabajo: todos los resultados coinciden con los esperados.

## Nota

| Criterio | Puntos |
|---|---|
| Creación y atributos de arreglos (Ej. 1) | 10 / 10 |
| Indexación y slicing (Ej. 2) | 10 / 10 |
| Máscaras booleanas (Ej. 3) | 15 / 15 |
| Vectorización y broadcasting (Ej. 4) | 15 / 15 |
| Estadística por eje y funciones universales (Ej. 5 y 6) | 20 / 20 |
| Integración (Ej. 7) | 10 / 10 |
| Ejecución sin errores | 10 / 10 |
| Documentación | 4 / 5 |
| Entrega correcta | 5 / 5 |
| **Total** | **99 / 100** |
| **Nota (0–5)** | **4.95** |

Este taller aporta **14.9 %** de los 15 % del momento evaluativo.

## 1. Creación y atributos de arreglos (10 / 10)
**Lo que hizo bien:**
- Creó `lecturas_crudas` con `np.array` y leyó forma, dimensiones, tamaño y tipo de sus atributos.
- `dias` incluye el día 7, y `pendientes` e `interceptos` son correctos.

## 2. Indexación y slicing (10 / 10)
**Lo que hizo bien:**
- Cada resultado sale de una sola expresión, con el índice negativo y el bloque de forma (3, 4) bien recortado.

## 3. Máscaras booleanas (15 / 15)
**Lo que hizo bien:**
- `es_util` une dos comparaciones entre paréntesis con `&`.
- Quedan 5 lecturas útiles, 2 faltantes y el promedio es 27.0, sin bucles.

## 4. Vectorización y broadcasting (15 / 15)
**Lo que hizo bien:**
- Convirtió pendientes e interceptos en columnas (5, 1) y calibró todo de una vez, sin tocar `lecturas_crudas`.
- La explicación del error de formas (5, 7) contra (5,) es clara y correcta.
- El promedio calibrado de SBC-A es 31.9.

## 5. Estadística por eje y funciones universales (20 / 20)
**Lo que hizo bien:**
- Promedios por sensor y por día con el eje correcto, máximo por sensor y media sobre el límite (43.275).
- Usó `np.maximum`, `np.abs` y `np.round`, y `en_alerta` sobre una copia, con 8 celdas mayores que 0 y `calibradas` intacto.

## 6. Integración (10 / 10)
**Lo que hizo bien:**
- Conteos 9, 18, 7 y 1 (suman 35), día pico 5 y las dos líneas de salida idénticas a lo pedido.

## 7. Ejecución sin errores (10 / 10)
**Lo que hizo bien:**
- El notebook corre completo sin errores y la verificación imprime el mensaje final.

## 8. Documentación (4 / 5)
**Lo que hizo bien:**
- Los siete ejercicios tienen su celda de texto previa y los nombres están en `snake_case` sin tildes.

**Lo que puede mejorar:**
- La celda inicial quedó con los textos de ejemplo "[tu nombre aquí]" y "[fecha aquí]". Debía llevar su nombre completo y la fecha.

**Cómo corregirlo:**
- Abra la primera celda de texto del notebook, borre "[tu nombre aquí]" y "[fecha aquí]", y escriba en su lugar su nombre completo y la fecha de entrega.

## 9. Entrega correcta (5 / 5)
**Lo que hizo bien:**
- El notebook está en `ejercicios/` con el nombre exacto y a tiempo.

## ¿El notebook funciona?
Sí. Corre completo sin errores, la celda de verificación imprime "Verificación completada sin errores." y todos los resultados coinciden con los esperados.

## Para el próximo taller
- Antes de entregar, complete la celda inicial con su nombre y la fecha, siguiendo los pasos de «Cómo corregirlo».
- Relea la guía de entrega punto por punto para no dejar textos de plantilla.
- Siga usando operaciones de NumPy en vez de bucles, como lo hizo aquí.
