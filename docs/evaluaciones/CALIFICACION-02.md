# Retroalimentación — Taller evaluativo 02: Funciones y POO

**Estudiante:** Wolfang Felipe Pérez Roldán · **Taller:** Taller evaluativo 02 — Funciones y POO
**Fecha límite:** 2026-10-21 00:00 · **Versión revisada:** commit `937305b`

Muy buen trabajo: casi todo el taller funciona como se pedía.

## Nota

| Criterio | Puntos |
|---|---|
| Funciones: parámetros, valores por defecto y retorno (Ej. 1 a 3) | 20 / 20 |
| `map`, `filter` y `lambda` (Ej. 4) | 10 / 10 |
| Clases, atributos y métodos (Ej. 5 y 7) | 15 / 15 |
| Encapsulamiento y validación (Ej. 6) | 15 / 15 |
| `__repr__` y `__str__` (Ej. 6 a 8) | 10 / 10 |
| Integración de funciones y clases (Ej. 8) | 6 / 10 |
| Ejecución sin errores | 10 / 10 |
| Documentación | 3 / 5 |
| Entrega correcta | 2 / 5 |
| **Total** | **91 / 100** |
| **Nota (0–5)** | **4.55** |

Este taller aporta **13.7 %** de los 15 % del momento evaluativo.

## 1. Funciones: parámetros, valores por defecto y retorno (20 / 20)
**Lo que hizo bien:**
- `calibrar_lectura` tiene los valores por defecto en la firma, usa `return` y da 11.5 y 12.0 como se esperaba.
- `es_lectura_valida` responde bien para 25.0, -999.0, 600.0 y 0.0, sin leer variables de afuera.
- `promedio_valido` reutiliza `es_lectura_valida`, da 27.0 y devuelve `None` cuando no hay lecturas válidas.

## 2. `map`, `filter` y `lambda` (10 / 10)
**Lo que hizo bien:**
- Obtuvo 5 lecturas calibradas (de 11.5 a 61.9) y 2 excedencias, sin bucles `for` ni comprensiones.

## 3. Clases, atributos y métodos (15 / 15)
**Lo que hizo bien:**
- `Lectura` guarda sus tres datos con valores por defecto y `a_microgramos` da 25.2.
- `Estacion` guarda objetos `Lectura` y `valores()` devuelve los ocho valores usando `a_microgramos()`.

## 4. Encapsulamiento y validación (15 / 15)
**Lo que hizo bien:**
- `Sensor` lanza `ValueError` para el código vacío y la pendiente menor o igual a cero, antes de guardar datos.
- La pendiente y el intercepto quedan como `_pendiente` e `_intercepto`, y `calibrar` reutiliza `calibrar_lectura`.
- Dejó las pruebas de error comentadas, como se pedía.

## 5. `__repr__` y `__str__` (10 / 10)
**Lo que hizo bien:**
- Los textos de `Sensor`, `Estacion` e `InformeEstacion` coinciden exactamente con lo pedido.

## 6. Integración de funciones y clases (6 / 10)
**Lo que hizo bien:**
- `InformeEstacion` reutiliza `es_lectura_valida`, `promedio_valido`, `categoria_pm25` y el `calibrar` del sensor, y da 31.9 y "Moderada". Además resolvió el reto opcional de `excedencias` (da 2).

**Lo que puede mejorar:**
- En `categoria_pm25` la categoría "Buena" llega solo hasta 9.0, pero la escala oficial dice hasta 12.0. Por eso una concentración de 10 o 11 saldría como "Moderada" cuando debería ser "Buena". La verificación no lo detecta porque el ejemplo del taller cae en "Moderada".

## 7. Ejecución sin errores (10 / 10)
**Lo que hizo bien:**
- El notebook corre completo sin errores y no dejó celdas de prueba que fallen.

## 8. Documentación (3 / 5)
**Lo que hizo bien:**
- Cada ejercicio tiene su celda de texto previa y los nombres siguen las convenciones.

**Lo que puede mejorar:**
- Faltan docstrings de una línea en varios métodos: los `__init__` de las clases y los `__repr__` y `__str__`. El taller pedía uno en cada función, clase y método.

## 9. Entrega correcta (2 / 5)
**Lo que puede mejorar:**
- No siguió la estructura acordada: el archivo se llama `aller_evaluativo_02_funciones_y_poo.ipynb` y el nombre exacto debía ser `taller-evaluativo-02-funciones-y-poo.ipynb` (falta la "t" inicial y se usaron guiones bajos en lugar de guiones). Sí está en la carpeta `ejercicios/` y antes del plazo.

## ¿El notebook funciona?
Sí: corre completo sin errores y la celda de verificación imprime "Verificación completada sin errores." Los resultados coinciden con los esperados, salvo el límite de la categoría "Buena", que no estaba en la verificación.

## Para el próximo taller
- Copie el nombre del archivo tal como lo indica la guía, letra por letra.
- Compare cada rango de las tablas con el enunciado antes de dar un ejercicio por terminado.
- Pruebe sus funciones con valores en los bordes (por ejemplo 12.0, 35.4 y 55.4), no solo con los de la guía.
- Agregue un docstring de una línea a cada método, incluidos `__init__`, `__repr__` y `__str__`.
