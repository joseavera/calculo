# Clave de respuestas y explicaciones

**Evaluación:** Integración aplicada a Sistemas Computacionales
**Asignatura:** Cálculo Integral · Licenciatura en Sistemas Computacionales
**Unidad 1 · Tema:** Fórmulas básicas de integración
**Docente:** Mtro. José Armando Vera Rodríguez

> Importante: en la evaluación, el orden de los escenarios y de las opciones cambia en cada intento. Por eso esta clave identifica cada reactivo por su **tema** y cada respuesta por su **texto**, no por la letra (A, B, C, D) ni por el número de pregunta.

---

## Resumen de la Parte A (cada reactivo vale 1 punto, total 8)

| # | Tema del escenario | Respuesta correcta |
|---|---|---|
| 1 | Acumulación a partir de una tasa | 50 MB |
| 2 | Significado de la constante C | Lo que ya existía al inicio: los 200 GB |
| 3 | Del costo por GB al costo total | $80 |
| 4 | Revisión de código y verificación | Faltó dividir entre 5: lo correcto es x⁵/5 + C, y se comprueba derivando |
| 5 | Caso especial: 1/x | 10 ln\|t\| + C |
| 6 | Función exponencial | 3eᵗ |
| 7 | Función trigonométrica | sen t |
| 8 | Derivar o integrar: elegir la operación | De (I) a (II): integrar. De (II) a (I): derivar |

---

## Explicación de cada reactivo

### 1. Acumulación a partir de una tasa

**Escenario:** un servidor descarga actualizaciones a 5 MB por segundo, constante. ¿Cuántos MB habrá descargado a los 10 segundos?

**Respuesta correcta: 50 MB**

**Procedimiento:**

- Se integra la tasa: ∫ 5 dt = 5t + C.
- Como parte de 0 MB, entonces C = 0 y la descarga total es D(t) = 5t.
- Se evalúa en t = 10: D(10) = 5 · 10 = 50 MB.

**Por qué las otras opciones son incorrectas:**

- *5 MB:* confunde la tasa (lo que descarga cada segundo) con el total acumulado.
- *15 MB:* suma 5 + 10 en lugar de multiplicar.
- *500 MB:* multiplica de más (5 · 10²); la regla de ∫ k dt es kt, no kt².

**Idea clave:** la integral convierte una *tasa* (MB por segundo) en un *total* (MB).

---

### 2. Significado de la constante C

**Escenario:** un servicio de respaldos guarda 3 GB por hora; el total es S(t) = 3t + C y el servidor ya tenía 200 GB antes de medir.

**Respuesta correcta: lo que ya existía al inicio, los 200 GB**

**Explicación:**

- Si evalúas en t = 0: S(0) = 3(0) + C = C.
- Como al inicio había 200 GB, entonces C = 200.
- La constante de integración representa el **valor inicial** del sistema, lo que ya había antes de empezar a medir.

**Por qué las otras opciones son incorrectas:**

- *La rapidez de guardado:* eso es el 3 (la tasa), no la constante.
- *Un error que puede ignorarse:* C nunca se ignora; cambia el resultado final.
- *El tiempo que dura el respaldo:* el tiempo es la variable t.

---

### 3. Del costo por GB al costo total

**Escenario:** cada GB cuesta $3 y hay un cargo fijo de $50. El costo total es C(x) = 3x + 50. ¿Cuánto cuesta almacenar 10 GB?

**Respuesta correcta: $80**

**Procedimiento:**

- C(10) = 3(10) + 50 = 30 + 50 = 80.

**Por qué las otras opciones son incorrectas:**

- *$30:* olvida el cargo fijo de $50.
- *$53:* suma 3 + 50 sin multiplicar el costo por los 10 GB.
- *$150:* multiplica el cargo fijo por el costo por GB (3 · 50).

**Idea clave:** el cargo fijo cumple el papel de la constante de integración: es el costo cuando x = 0.

---

### 4. Revisión de código y verificación

**Escenario:** un compañero escribió que ∫ x⁴ dx = x⁵ + C.

**Respuesta correcta: faltó dividir entre 5; lo correcto es x⁵/5 + C, y se comprueba derivando el resultado**

**Procedimiento (regla de la potencia):**

- Se suma 1 al exponente: 4 + 1 = 5.
- Se divide entre el nuevo exponente: x⁵/5.
- Se agrega la constante: x⁵/5 + C.

**Verificación:** d/dx (x⁵/5) = 5x⁴/5 = x⁴. Al derivar se regresa al integrando original, por lo tanto el resultado es correcto.

**Por qué las otras opciones son incorrectas:**

- *No hay error:* si derivas x⁵ obtienes 5x⁴, no x⁴; la respuesta del compañero no pasa la verificación.
- *Restar 1 al exponente:* eso se hace al derivar, no al integrar.
- *Quitar la constante C:* la constante siempre debe aparecer en una integral indefinida.

**Idea clave:** derivar el resultado es la forma más rápida de comprobar si una integral quedó bien, igual que ejecutar una prueba después de modificar código.

---

### 5. Caso especial: 1/x

**Escenario:** una base de datos crece a una tasa g(t) = 10/t GB por mes. ¿Cuál es G(t), la función cuya derivada es g(t)?

**Respuesta correcta: 10 ln|t| + C**

**Procedimiento:**

- La constante 10 sale de la integral: ∫ 10/t dt = 10 ∫ (1/t) dt.
- La fórmula de la tabla indica que ∫ (1/t) dt = ln|t| + C.
- Resultado: G(t) = 10 ln|t| + C.

**Por qué es un caso especial:** la regla de la potencia (x^(n+1)/(n+1)) no funciona cuando n = −1, porque obligaría a dividir entre cero. Para 1/x se usa el logaritmo natural.

**Por qué las otras opciones son incorrectas:**

- *10eᵗ + C:* es la integral de una exponencial, no de 1/t.
- *5t² + C:* es la integral de 10t, es decir, trata a 10/t como si fuera 10t.
- *−10/t² + C:* es la **derivada** de 10/t; se hizo la operación contraria.

---

### 6. Función exponencial

**Escenario:** los usuarios nuevos de una aplicación por mes crecen según u'(t) = 3eᵗ (miles de usuarios por mes). ¿Qué función describe el total acumulado, sin considerar la constante?

**Respuesta correcta: 3eᵗ**

**Procedimiento:**

- Se saca la constante: ∫ 3eᵗ dt = 3 ∫ eᵗ dt.
- La función eᵗ es su propia integral: ∫ eᵗ dt = eᵗ + C.
- Resultado: 3eᵗ + C.

**Verificación:** d/dt (3eᵗ) = 3eᵗ, que coincide con la tasa dada.

**Por qué las otras opciones son incorrectas:**

- *3 ln|t|:* el logaritmo es la integral de 1/t, no de eᵗ.
- *eᵗ/3:* divide entre 3 cuando la constante debe multiplicar.
- *3t·eᵗ:* no cumple la verificación; su derivada incluye un término adicional.

---

### 7. Función trigonométrica

**Escenario:** un sensor registra una aceleración a(t) = cos t. Para obtener la velocidad se integra. ¿Cuál es v(t), sin considerar la constante?

**Respuesta correcta: sen t**

**Procedimiento:**

- De la tabla: ∫ cos t dt = sen t + C.

**Verificación:** d/dt (sen t) = cos t.

**Por qué las otras opciones son incorrectas:**

- *−sen t:* es la derivada de cos t, no su integral.
- *cos t:* no cambia nada; su derivada es −sen t, no cos t.
- *−cos t:* es la integral de sen t, no la de cos t.

**Idea clave:** conviene verificar siempre el signo derivando: la derivada de sen t es cos t (positivo), y la derivada de cos t es −sen t (negativo).

---

### 8. Derivar o integrar: elegir la operación

**Escenario:** (I) la rapidez con que cambia el número de usuarios conectados; (II) el número total de usuarios conectados en cada instante.

**Respuesta correcta: de (I) a (II), integrar; de (II) a (I), derivar**

**Explicación:**

- (I) es una **tasa de cambio**: cuántos usuarios se suman o se van cada minuto.
- (II) es un **total acumulado**: cuántos usuarios hay en cada instante.
- Para pasar de una tasa a un total se **integra** (acumular).
- Para pasar de un total a su tasa se **deriva** (medir cómo cambia).

**Analogía:** el velocímetro es la tasa; el odómetro es el total. El odómetro se obtiene acumulando lo que marca el velocímetro; el velocímetro indica qué tan rápido cambia el odómetro.

**Por qué las otras opciones son incorrectas:**

- *Derivar e integrar al revés:* intercambia las dos operaciones.
- *Integrar en ambos casos* o *derivar en ambos casos:* ignoran que son operaciones inversas.

---

## Parte B: orientación para la revisión (reflexión)

**Pregunta 1:** el alumno piensa en una aplicación, videojuego, red o base de datos que usa y explica (a) qué cosa cambia con el tiempo, (b) qué total le interesaría conocer a un ingeniero y (c) para qué le serviría saberlo.

**Qué buscar en la respuesta (sugerencia, ajustable a tu criterio):**

| Criterio | Qué indica una respuesta lograda |
|---|---|
| (a) Tasa | Identifica una cantidad que cambia con el tiempo, con una unidad razonable (mensajes por minuto, MB por segundo, usuarios por hora). |
| (b) Total acumulado | Señala el total que se obtendría al acumular esa tasa (mensajes totales, datos descargados, usuarios conectados). |
| (c) Decisión | Explica para qué serviría conocerlo: planear capacidad, controlar costos, evitar caídas, detectar anomalías de seguridad. |
| Coherencia | Las tres partes se relacionan entre sí y están redactadas con sus propias palabras. |

**Ejemplo de una buena respuesta:**

> En un videojuego en línea, el número de jugadores que se conectan por minuto es la tasa. El total de jugadores conectados a lo largo de la noche permitiría a un ingeniero saber cuántos servidores reservar en horas pico, para evitar caídas y controlar el costo de la infraestructura en la nube.

**Señales de una respuesta débil:**

- Solo menciona que "las integrales sirven para muchas cosas" sin ningún ejemplo concreto.
- Confunde la tasa con el total (por ejemplo, dice que el total es "cuántos se conectan por minuto").
- Es una definición copiada o muy general, sin relación con un sistema real.

**Pregunta 2 (opcional):** sirve como retroalimentación. Las dudas que los alumnos mencionen (por ejemplo, sobre la constante C o sobre el caso 1/x) pueden orientar el repaso de la siguiente sesión.

---

## Notas para la aplicación y la captura de resultados

- La Parte A se califica sola: el resultado muestra "Correcta", "Incorrecta" o "Sin responder" por tema, sin revelar la respuesta.
- La Parte B aparece completa en el resultado y en el PDF exportado. La calificación de esta parte queda a tu criterio.
- El resultado incluye nombre, fecha, número de intentos (recargas), infracciones por cambio de ventana y tiempo utilizado.
