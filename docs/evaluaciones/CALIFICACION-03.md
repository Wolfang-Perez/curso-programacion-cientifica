# Retroalimentación — Taller evaluativo 03 (NumPy)

**Estudiante:** Wolfang Felipe Pérez Roldán · **Taller:** Taller evaluativo 03 — NumPy
**Fecha límite:** 2026-10-30 23:59 · **Versión revisada:** commit `8cb6847`

Excelente trabajo: todos los ejercicios están bien resueltos.

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
| Documentación | 5 / 5 |
| Entrega correcta | 2 / 5 |
| **Total** | **97 / 100** |
| **Nota (0–5)** | **4.85** |

Este taller aporta **14.6 %** de los 15 % del momento evaluativo.

## 1. Creación y atributos de arreglos (10 / 10)
**Lo que hizo bien:**
- `lecturas_crudas` se crea con `np.array` y una lista de listas, y sus atributos se leen del propio arreglo.
- `dias`, `pendientes` e `interceptos` son correctos.

## 2. Indexación y slicing (10 / 10)
**Lo que hizo bien:**
- Cada resultado sale de una sola expresión de indexación, con índice negativo donde se pedía.
- El bloque tiene la forma (3, 4) esperada.

## 3. Máscaras booleanas (15 / 15)
**Lo que hizo bien:**
- `es_util` une dos comparaciones entre paréntesis con `&`, sin bucles.
- Quedan 5 lecturas útiles, 2 faltantes y el promedio es 27.0.

## 4. Vectorización y broadcasting (15 / 15)
**Lo que hizo bien:**
- Convirtió pendientes e interceptos en columnas (5, 1) y calibró todo sin bucles.
- La celda de texto explica con claridad por qué falla la multiplicación con formas (5, 7) y (5,).
- El promedio calibrado de SBC-A da 31.9 y `lecturas_crudas` queda intacto.

## 5. Estadística por eje y funciones universales (20 / 20)
**Lo que hizo bien:**
- Los promedios por sensor y por día, los máximos y la media sobre el límite (43.275) son correctos.
- Usó `np.maximum`, `np.abs` y `np.round`, y `en_alerta` es una copia con máscara que deja 8 celdas y no altera `calibradas`.

## 6. Integración (10 / 10)
**Lo que hizo bien:**
- Los conteos 9, 18, 7 y 1 suman 35, y `dia_pico` es 5.
- Las dos líneas de salida coinciden con lo pedido. También resolvió el reto opcional con `np.digitize`.

## 7. Ejecución sin errores (10 / 10)
**Lo que hizo bien:**
- El notebook corre completo sin errores y la celda de verificación imprime el mensaje final.

## 8. Documentación (5 / 5)
**Lo que hizo bien:**
- Cada ejercicio tiene su celda de texto previa y los nombres de variables están en `snake_case` sin tildes.

## 9. Entrega correcta (2 / 5)
**Lo que hizo bien:**
- El notebook está en la carpeta `ejercicios/` de `main` y fue subido a tiempo.

**Lo que puede mejorar:**
- No siguió la estructura acordada: el archivo se llama `taller_evaluativo_03_numpy.ipynb` (con guiones bajos) y debía llamarse exactamente `taller-evaluativo-03-numpy.ipynb` (con guiones).

**Cómo corregirlo:**
- Cambie el nombre del archivo en `ejercicios/` para que use guiones medios, tal como lo indica la guía, y revise lo mismo en los demás talleres.

## ¿El notebook funciona?
Sí. Corre de principio a fin sin errores, la celda de verificación imprime "Verificación completada sin errores." y todos los resultados coinciden con los esperados.

## Para el próximo taller
- Copie el nombre del archivo exactamente como aparece en la guía antes de subirlo.
- Siga reiniciando y ejecutando todo antes de entregar, como lo hizo aquí.
- Mantenga las celdas de texto que explican cada ejercicio.
