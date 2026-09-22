# Taller Integrador Individual — Cortes 1 y 2
**Buenas Prácticas de Desarrollo de Software**

**Nombre completo:** Jhon Lara

## Tabla de hallazgos — Auditoría y corrección

| Defecto encontrado | Por qué era un problema | Cómo lo corrigió |
|---|---|---|
| Archivos `Mi Pagina De Notas.HTML` y `Estilos Del Sitio.CSS` con espacios | Los espacios en nombres de archivo generan problemas en URLs, Git y despliegue web | Se renombraron a `index.html` y `style.css` |
| Variables `a`, `b`, `c` | No indican qué almacenan (las tres notas ingresadas) | Se renombraron a `nota1`, `nota2`, `nota3` |
| Variable `x` con valor 3, declarada con `let` | Número sin definición y sin nombre, y `let` en un valor que nunca cambia sugiere descuido | Se renombró a `cantidadNotas` y se declaró con `const` |
| Variable `TempValue2` | Nombre poco descriptivo que no indica que almacena el promedio calculado | Se renombró a `promedio` |
| Variable `data1` (`let data1 = []`) | Se declaraba pero nunca se usaba en el código | Se eliminó por ser código sin uso |
| Función `calc()` | Nombre poco descriptivo, no indica qué calcula | Se renombró a `calcularPromedio()` |
| IDs `n1`, `n2`, `n3` | No describen que corresponden a las notas ingresadas | Se renombraron a `nota1`, `nota2`, `nota3` |
| IDs `r` y `r2` | No describen que son el resultado del promedio y el estado (aprobado/reprobado) | Se renombraron a `resultadoPromedio` y `resultadoEstado` |
| `<title>pagina</title>` | No describe el contenido de la página | Se cambió a `<title>Calculadora de Promedio</title>` |
| Función comentada `calcularAntiguo(...)` | Código muerto, ya no cumple ninguna función | Se eliminó |
| `console.log(...)` (x3) | Logs de depuración olvidados en el código de producción | Se eliminaron |
| Número `3.0` en la condición de aprobación | El umbral de aprobación no tiene nombre, obliga a adivinar su significado | Se extrajo a la constante `NOTA_MINIMA_APROBACION` |

## Sitio publicado
Pendiente.