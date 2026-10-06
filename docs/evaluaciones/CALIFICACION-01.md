# Retroalimentación — Taller evaluativo 01

**Estudiante:** Wolfang Felipe Pérez Roldán · **Taller:** Taller evaluativo 01 — Python y estructuras de datos
**Fecha límite:** 2026-10-06 23:59 · **Versión revisada:** commit `5c268e2`

Muy buen trabajo, el notebook está casi completo y bien resuelto.

## Nota

| Criterio | Puntos |
|---|---|
| Variables, tipos y operadores (Ej. 1 a 4) | 20 / 20 |
| Condicionales y clasificación (Ej. 5) | 13 / 15 |
| Bucles, acumuladores y control de flujo (Ej. 6 a 8) | 30 / 30 |
| Estructuras de datos nativas (Ej. 9) | 11 / 15 |
| Ejecución sin errores | 10 / 10 |
| Documentación en celdas de texto | 5 / 5 |
| Entrega correcta | 2 / 5 |
| **Total** | **91 / 100** |
| **Nota (0–5)** | **4.55** |

Este taller aporta **13.7 %** de los 15 % del momento evaluativo.

## 1. Variables, tipos y operadores (20 / 20)
**Lo que hizo bien:**
- Las siete variables tienen el tipo correcto y los verificó con `type()`.
- La conversión y los tres errores del Ejercicio 2 salen de operaciones, no de números escritos a mano.
- El Ejercicio 3 usa solo `//` y `%`.
- El Ejercicio 4 usa `and` y `not`, sin `if`, y los tres resultados son correctos.

## 2. Condicionales y clasificación (13 / 15)
**Lo que hizo bien:**
- Las cuatro categorías están bien ordenadas y la lectura 41.8 queda como "Dañina para grupos sensibles".
**Lo que puede mejorar:**
- Agregó una condición extra al inicio ("Dato no valido"). La guía pedía solo las cuatro categorías de la escala; esa condición añade una quinta categoría que no existe en la tabla.

## 3. Bucles, acumuladores y control de flujo (30 / 30)
**Lo que hizo bien:**
- Ejercicio 6: descarta los dos -999.0 con `continue` antes de acumular; da 10 válidas y promedio 22.55.
- Ejercicio 7: máximo 58.3, mínimo 7.5, con dos recorridos y sin `max()`, `min()` ni `sum()`.
- Ejercicio 8: el `while` actualiza la concentración dentro del bloque y termina (10 horas).

## 4. Estructuras de datos nativas (11 / 15)
**Lo que hizo bien:**
- Accede a los datos de cada estación por su clave.
- Usa `get` con "no disponible", así que no hay errores en las estaciones sin humedad.
**Lo que puede mejorar:**
- Las coordenadas se sacan con posiciones (`[0]` y `[1]`). La guía pedía desempaquetar la tupla en dos variables en una sola línea (`latitud, longitud = ...`).

## 5. Ejecución sin errores (10 / 10)
- El notebook corre completo desde cero sin errores y la celda de verificación imprime el mensaje final.

## 6. Documentación en celdas de texto (5 / 5)
- Los nueve ejercicios tienen su celda de texto explicativa y los nombres de variables son claros.

## 7. Entrega correcta (2 / 5)
**Lo que puede mejorar:**
- No siguió la convención acordada: el archivo se llama `taller_evaluativo_01_calidad_del_aire.ipynb` (con guiones bajos) y debía llamarse exactamente `taller-evaluativo-01-calidad-del-aire.ipynb` (con guiones).
- Sí está en la carpeta `ejercicios/` y se subió antes del plazo.

## ¿El notebook funciona?
Sí. Corre completo sin errores, la celda de verificación da "Verificación completada sin errores." y los resultados coinciden con los esperados.

## Para el próximo taller
- Copie el nombre del archivo exactamente como lo indica la guía.
- Use desempaquetado de tuplas (`a, b = tupla`) cuando se pida.
- Haga solo lo que pide la guía en cada cadena `if / elif / else`, sin condiciones adicionales.
- Siga ejecutando "Reiniciar y ejecutar todas" antes de entregar, como hizo esta vez.
