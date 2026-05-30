# Resultados — Funciones Logarítmicas

| Campo | Valor |
|-------|-------|
| **Asignatura** | Cálculo Diferencial |
| **Unidad** | 1 — Funciones y Modelado |
| **Tema** | Funciones Logarítmicas |
| **Fecha** | 2026-05-30 |
| **Puntaje** | 0 / 6 (0%) |

---

## Resumen de ejercicios

| # | Ejercicio | Tu respuesta | Correcta | Estado |
|---|-----------|-------------|----------|--------|
| 1 | Conversión exponencial a logarítmica | `(sin respuesta)` | `5` | ❌ Incorrecto |
| 2 | Evaluación con base 10 | `(sin respuesta)` | `3` | ❌ Incorrecto |
| 3 | Propiedad del producto | `(sin respuesta)` | `5` | ❌ Incorrecto |
| 4 | Propiedad de la potencia | `(sin respuesta)` | `4` | ❌ Incorrecto |
| 5 | La inversa: ln y e son opuestas | `(sin respuesta)` | `4` | ❌ Incorrecto |
| 6 | Aplicación real: búsqueda binaria | `(sin respuesta)` | `10` | ❌ Incorrecto |

---

## Detalle por ejercicio

### Ejercicio 1: Conversión exponencial a logarítmica

> Convierte a forma logarítmica: 2⁵ = 32. ¿Cuánto vale log₂(32)?

**Tu respuesta:** `(sin respuesta)`  
**Respuesta correcta:** `5`  
**Estado:** Incorrecto  

**Explicación:**

log₂(32) = 5 porque 2⁵ = 2×2×2×2×2 = 32. El logaritmo devuelve el exponente.

**Pasos de solución:**

1. Identifica la base (2), el exponente (5) y el resultado (32).
2. La forma logarítmica pregunta: ¿a qué potencia hay que elevar 2 para obtener 32?
3. Escribe log₂(32) = ? Ese valor es el exponente que ya conoces.

---

### Ejercicio 2: Evaluación con base 10

> Calcula: log₁₀(1000) = ?

**Tu respuesta:** `(sin respuesta)`  
**Respuesta correcta:** `3`  
**Estado:** Incorrecto  

**Explicación:**

log₁₀(1000) = 3 porque 10³ = 1000. Un terremoto de magnitud 3 es 1000 veces más intenso que uno de magnitud 0.

**Pasos de solución:**

1. Pregúntate: ¿10 elevado a qué número da 1000?
2. 10¹ = 10 · 10² = 100 · 10³ = 1000.
3. Por lo tanto log₁₀(1000) = ese exponente.

---

### Ejercicio 3: Propiedad del producto

> Simplifica log₂(8 × 4) usando la propiedad del producto. ¿Cuál es el valor numérico final?

**Tu respuesta:** `(sin respuesta)`  
**Respuesta correcta:** `5`  
**Estado:** Incorrecto  

**Explicación:**

log₂(32) = 5. Verificación directa: 2⁵ = 32, y 8 × 4 = 32. La propiedad funciona.

**Pasos de solución:**

1. Aplica la propiedad de producto: log₂(8 × 4) = log₂(8) + log₂(4).
2. Calcula log₂(8): ¿2 elevado a qué da 8? → 2³ = 8, entonces log₂(8) = 3.
3. Calcula log₂(4): ¿2 elevado a qué da 4? → 2² = 4, entonces log₂(4) = 2.
4. Suma: 3 + 2 = ?

---

### Ejercicio 4: Propiedad de la potencia

> Simplifica log₃(9²) usando la propiedad de la potencia. ¿Cuál es el valor numérico?

**Tu respuesta:** `(sin respuesta)`  
**Respuesta correcta:** `4`  
**Estado:** Incorrecto  

**Explicación:**

log₃(81) = 4 porque 3⁴ = 81, y 9² = 81. La propiedad baja el exponente 2 como factor y luego evalúas el logaritmo restante.

**Pasos de solución:**

1. Aplica la propiedad de potencia: log₃(9²) = 2 · log₃(9).
2. Calcula log₃(9): ¿3 elevado a qué da 9? → 3² = 9, entonces log₃(9) = 2.
3. Multiplica: 2 · 2 = ?

---

### Ejercicio 5: La inversa: ln y e son opuestas

> Calcula: ln(e⁴) = ?

**Tu respuesta:** `(sin respuesta)`  
**Respuesta correcta:** `4`  
**Estado:** Incorrecto  

**Explicación:**

ln(e⁴) = 4. Esta propiedad permite despejar t en ecuaciones como e^(0.3t) = 5: aplicas ln a ambos lados y obtienes 0.3t = ln(5) ≈ 1.609, entonces t ≈ 5.36.

**Pasos de solución:**

1. Recuerda que ln y eˣ se cancelan mutuamente: son funciones inversas.
2. La regla es: ln(eˣ) = x para cualquier valor de x.
3. Aplícala directamente: ln(e⁴) = ?

---

### Ejercicio 6: Aplicación real: búsqueda binaria

> Una búsqueda binaria sobre una lista de 1024 elementos necesita log₂(1024) comparaciones en el peor caso. ¿Cuántas son?

**Tu respuesta:** `(sin respuesta)`  
**Respuesta correcta:** `10`  
**Estado:** Incorrecto  

**Explicación:**

log₂(1024) = 10. Con solo 10 comparaciones se encuentra cualquier elemento en una lista de 1024. Si la lista tuviera 1 048 576 elementos (2²⁰), solo necesitarías 20 comparaciones. Eso es la potencia de O(log n).

**Pasos de solución:**

1. Pregúntate: ¿2 elevado a qué número da 1024?
2. Verifica: 2¹=2, 2²=4, 2³=8, 2⁴=16, 2⁵=32, 2⁶=64, 2⁷=128, 2⁸=256, 2⁹=512, 2¹⁰=1024.
3. Por lo tanto log₂(1024) = ?

---

## Conceptos clave

### Definición fundamental

```
log_a(x) = y   <-->   a^y = x
```

### Los tres logaritmos esenciales

| Nombre | Notación | Base | Aplicación principal |
|--------|----------|------|----------------------|
| Logaritmo común | `log(x)` | 10 | Escala Richter, pH, decibeles |
| Logaritmo natural | `ln(x)` | e ≈ 2.71828 | Cálculo diferencial: d/dx[ln(x)] = 1/x |
| Logaritmo binario | `log₂(x)` | 2 | Complejidad algorítmica O(log n) |

### Propiedades algebraicas

| Propiedad | Regla | En palabras |
|-----------|-------|-------------|
| Producto | `log(a·b) = log(a) + log(b)` | Multiplicar adentro = sumar afuera |
| Cociente | `log(a/b) = log(a) − log(b)` | Dividir adentro = restar afuera |
| Potencia | `log(aⁿ) = n · log(a)` | El exponente baja como factor |
| Inversa | `ln(eˣ) = x` y `e^(ln x) = x` | ln y exp se cancelan mutuamente |

---

## Referencias bibliográficas

- Napier, J. (1614). *Mirifici Logarithmorum Canonis Descriptio*. Edimburgo.
- Euler, L. (1748). *Introductio in analysin infinitorum*. Lausana.
- Stewart, J. (2016). *Cálculo: Trascendentes tempranas* (8.ª ed.). Cengage Learning.
- Larson, R. y Edwards, B. (2017). *Cálculo* (10.ª ed.). McGraw-Hill Education.
