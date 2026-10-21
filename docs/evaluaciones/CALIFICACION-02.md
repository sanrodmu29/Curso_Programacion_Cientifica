# Retroalimentación — Funciones y POO

**Estudiante:** Santiago Rodríguez Muñoz · **Taller:** Taller evaluativo 02 — Funciones y POO
**Fecha límite:** 2026-10-21 00:00 · **Versión revisada:** commit `040fec4`

Excelente trabajo: casi todo está correcto y bien resuelto.

## Nota

| Criterio | Puntos |
|---|---|
| Funciones: parámetros, valores por defecto y retorno (Ej. 1 a 3) | 20 / 20 |
| `map`, `filter` y `lambda` (Ej. 4) | 10 / 10 |
| Clases, atributos y métodos (Ej. 5 y 7) | 15 / 15 |
| Encapsulamiento y validación (Ej. 6) | 15 / 15 |
| `__repr__` y `__str__` (Ej. 6 a 8) | 10 / 10 |
| Integración de funciones y clases (Ej. 8) | 10 / 10 |
| Ejecución sin errores | 10 / 10 |
| Documentación | 4 / 5 |
| Entrega correcta | 5 / 5 |
| **Total** | **99 / 100** |
| **Nota (0–5)** | **4.95** |

Este taller aporta **14.9 %** de los 15 % del momento evaluativo.

## 1. Funciones: parámetros, valores por defecto y retorno (20 / 20)
**Lo que hizo bien:**
- `calibrar_lectura` tiene los valores por defecto en la firma, usa `return` y da 11.5 y 12.0 como se esperaba.
- `es_lectura_valida` responde bien para 25.0, -999.0, 600.0 y 0.0, sin usar variables globales.
- `promedio_valido` reutiliza `es_lectura_valida`, da 27.0 y devuelve `None` cuando no hay lecturas válidas.

## 2. `map`, `filter` y `lambda` (10 / 10)
**Lo que hizo bien:**
- Obtuvo las 5 lecturas calibradas (de 11.5 a 61.9) y las 2 excedencias, sin bucles ni comprensiones.

## 3. Clases, atributos y métodos (15 / 15)
**Lo que hizo bien:**
- `Lectura` guarda sus tres datos con valores por defecto y convierte bien de mg/m³ a µg/m³ (25.2).
- `Estacion` guarda objetos `Lectura` y `valores()` usa `a_microgramos()`; los ocho valores coinciden con la lista original.

## 4. Encapsulamiento y validación (15 / 15)
**Lo que hizo bien:**
- `Sensor` lanza `ValueError` para código vacío y para pendiente menor o igual a cero, antes de guardar datos.
- La pendiente y el intercepto quedan como `_pendiente` e `_intercepto`, y `calibrar` reutiliza la función del Ejercicio 1.
- Dejó las pruebas de validación comentadas, así el notebook no falla.

## 5. `__repr__` y `__str__` (10 / 10)
**Lo que hizo bien:**
- Los textos de `Sensor`, `Estacion` e `InformeEstacion` coinciden exactamente con lo pedido.

## 6. Integración de funciones y clases (10 / 10)
**Lo que hizo bien:**
- `categoria_pm25` usa una sola cadena `if / elif / else` y cubre bien las cuatro categorías.
- `InformeEstacion` reutiliza las funciones y el método `calibrar` del sensor; da 31.9 y "Moderada".
- Además resolvió el reto opcional de `excedencias` (da 2).

## 7. Ejecución sin errores (10 / 10)
**Lo que hizo bien:**
- El notebook corre completo sin errores y la celda de verificación imprime el mensaje final.

## 8. Documentación (4 / 5)
**Lo que hizo bien:**
- Todas las funciones, clases y métodos tienen su docstring de una línea y los nombres siguen las convenciones.
- Los ejercicios tienen su celda de texto explicativa.

**Lo que puede mejorar:**
- La primera celda de texto tiene su nombre y la fecha, pero le falta el título del taller.
- La celda de texto del Ejercicio 8 explica lo que hace, pero no lo indica como "Ejercicio 8" como los demás.

## 9. Entrega correcta (5 / 5)
**Lo que hizo bien:**
- El notebook está en `ejercicios/` con el nombre exacto, en la rama `main`.

## ¿El notebook funciona?
Sí. Corre de principio a fin sin errores, la celda de verificación imprime "Verificación completada sin errores." y todos los resultados coinciden con los esperados.

## Para el próximo taller
- Incluya siempre en la primera celda el título del taller junto con su nombre y la fecha.
- Titule cada ejercicio con su número, incluido el último.
- Siga reiniciando y ejecutando todo antes de entregar, como lo hizo aquí.
