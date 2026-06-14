# Portafolio: Elaboración del Portafolio
**Asignatura:** Matemáticas Discretas  
**Autor:** Tyrone Efren Encarnación Erique  
**Docente:** Ing. Mario Cueva  
**Institución:** Universidad Nacional de Loja - Facultad de la Energía, las Industrias, y los Recursos Naturales No Renovables  
**Año:** 2026  

---



## 📌 Índice de Contenidos

| Sección | 
| :--- |
| 📘 [**1. Resumen Teórico**](#1-resumen-teórico) |
| 📂 [**2. Evidencias de Ejercicios**](#2-evidencias-de-ejercicios) | 
| 🚀 [**3. Ejercicio Aplicado - Caso Real**](#3-ejercicio-aplicado---caso-real) | 
| 🧠 [**4. Reflexión Personal**](#4-reflexión-personal) | 

---
  
---
  
---

## 1. Resumen Teórico

<details id="11-definición-de-proposición">
<summary><b>1.1 Definición de Proposición</b> (Clic para desplegar)</summary>
<br>

Una proposición es un enunciado declarativo que puede ser evaluado como verdadero (V) o falso (F), pero nunca ambos al mismo tiempo. Es la unidad básica sobre la que opera toda la lógica proposicional.

* **Ejemplo:** "El agua hierve a 100°C al nivel del mar" $\rightarrow$ Proposición VERDADERA.
* **Ejemplo:** $"2+2=5" \rightarrow$ Proposición FALSA.
* "¿Qué hora es?" **NO** es proposición (es una pregunta, no puede ser V ni F).
</details>

<details id="12-tipos-de-proposiciones">
<summary><b>1.2 Tipos de Proposiciones</b> (Clic para desplegar)</summary>
<br>

### Proposiciones Simples
Son aquellas que no pueden descomponerse en proposiciones más pequeñas. Se representan con letras minúsculas: $p, q, r, s...$
* $p$: "Hoy llueve"
* $q$: "Tengo paraguas"
* $r$: "El examen es mañana"

### Proposiciones Compuestas
Se forman al combinar proposiciones simples mediante conectores lógicos. Su valor de verdad depende de los valores de sus componentes y del conector utilizado.
* "Hoy llueve Y tengo paraguas" $\rightarrow p \wedge q$
* "Hoy llueve O tengo paraguas" $\rightarrow p \vee q$
* "Si llueve, ENTONCES me mojo" $\rightarrow p \rightarrow q$
</details>

<details id="13-conectores-lógicos">
<summary><b>1.3 Conectores Lógicos</b> (Clic para desplegar)</summary>
<br>

Los conectores lógicos son operadores que permiten construir proposiciones compuestas a partir de proposiciones simples. Cada conector tiene una tabla de verdad específica que define su comportamiento.

| Nombre | Símbolo | Lectura | Descripción |
| :--- | :---: | :---: | :--- |
| **Negación** | $\neg p$ | No $p$ | Invierte el valor de verdad de $p$ |
| **Conjunción** | $p \wedge q$ | $p$ y $q$ | Verdadera solo cuando ambas son verdaderas |
| **Disyunción** | $p \vee q$ | $p$ o $q$ | Falsa solo cuando ambas son falsas |
| **Condicional** | $p \rightarrow q$ | Si $p$, entonces $q$ | Falsa solo cuando $p$ es V y $q$ es F |
| **Bicondicional** | $p \leftrightarrow q$ | $p$ si y solo si $q$ | Verdadera cuando $p$ y $q$ tienen el mismo valor |
</details>

<details id="14-tablas-de-verdad">
<summary><b>1.4 Tablas de Verdad</b> (Clic para desplegar)</summary>
<br>

Una tabla de verdad es una herramienta sistemática que muestra todos los posibles valores de verdad de una proposición compuesta, según los valores de sus componentes simples. Si una proposición tiene $n$ variables, la tabla tendrá $2^n$ filas.

#### Negación y Conjunción
| $p$ | $\neg p$ | | $p$ | $q$ | $p \wedge q$ |
| :---: | :---: | :---: | :---: | :---: | :---: |
| V | F | | V | V | V |
| F | V | | V | F | F |
| | | | F | V | F |
| | | | F | F | F |

#### Disyunción y Condicional (Solo es FALSA cuando el antecedente es V y el consecuente es F)
| $p$ | $q$ | $p \vee q$ | | $p$ | $q$ | $p \rightarrow q$ |
| :---: | :---: | :---: | :---: | :---: | :---: |
| V | V | V | | V | V | V |
| V | F | V | | V | F | F |
| F | V | V | | F | V | V |
| F | F | F | | F | F | V |

#### Bicondicional (Verdadera cuando p y q tienen el mismo valor)
| $p$ | $q$ | $p \leftrightarrow q$ |
| :---: | :---: | :---: |
| V | V | V |
| V | F | F |
| F | V | F |
| F | F | V |

### Clasificación de proposiciones según su tabla de verdad
| Tipo | Definición | Ejemplo |
| :--- | :--- | :---: |
| **Tautología** | Siempre VERDADERA en todos los casos | $p \vee \neg p$ |
| **Contradicción** | Siempre FALSA en todos los casos | $p \wedge \neg p$ |
| **Contingencia** | Puede ser V o F según los valores de entrada | $p \rightarrow q$ |
</details>

<details id="15-principales-leyes-lógicas">
<summary><b>1.5 Principales Leyes Lógicas</b> (Clic para desplegar)</summary>
<br>

Las leyes lógicas son equivalencias que siempre se cumplen independientemente de los valores de verdad de las variables. Son fundamentales para simplificar y transformar expresiones lógicas.

| Ley | Expresión | Descripción |
| :--- | :--- | :--- |
| **Doble negación** | $\neg(\neg p) \equiv p$ | Negar dos veces equivale a afirmar |
| **Idempotencia ($\wedge$)** | $p \wedge p \equiv p$ | Conjunción de $p$ consigo misma |
| **Idempotencia ($\vee$)** | $p \vee p \equiv p$ | Disyunción de $p$ consigo misma |
| **Conmutativa ($\wedge$)** | $p \wedge q \equiv q \wedge p$ | El orden no altera la conjunción |
| **Conmutativa ($\vee$)** | $p \vee q \equiv q \vee p$ | El orden no altera la disyunción |
| **Asociativa ($\wedge$)** | $(p \wedge q) \wedge r \equiv p \wedge(q \wedge r)$ | Agrupación en conjunciones |
| **Asociativa ($\vee$)** | $(p \vee q) \vee r \equiv p \vee(q \vee r)$ | Agrupación en disyunciones |
| **Distributiva ($\wedge \text{ s/ } \vee$)** | $p \wedge(q \vee r) \equiv(p \wedge q) \vee(p \wedge r)$ | Distribución de $\wedge$ sobre $\vee$ |
| **Distributiva ($\vee \text{ s/ } \wedge$)** | $p \vee(q \wedge r) \equiv(p \vee q) \wedge(p \vee r)$ | Distribución de $\vee$ sobre $\wedge$ |
| **De Morgan ($\wedge$)** | $\neg(p \wedge q) \equiv \neg p \vee \neg q$ | Negar una conjunción |
| **De Morgan ($\vee$)** | $\neg(p \vee q) \equiv \neg p \wedge \neg q$ | Negar una disyunción |
| **Absorción ($\wedge$)** | $p \wedge(p \vee q) \equiv p$ | Absorción en conjunción |
| **Absorción ($\vee$)** | $p \vee(p \wedge q) \equiv p$ | Absorción en disyunción |
| **Implicación material** | $p \rightarrow q \equiv \neg p \vee q$ | El condicional como disyunción |
| **Contraposición** | $p \rightarrow q \equiv \neg q \rightarrow \neg p$ | El condicional y su contrapositivo |
| **Tercio excluido** | $p \vee \neg p \equiv V$ | Tautología clásica |
| **Contradicción** | $p \wedge \neg p \equiv F$ | Contradicción clásica |
</details>

<details id="16-reglas-de-inferencia">
<summary><b>1.6 Reglas de Inferencia</b> (Clic para desplegar)</summary>
<br>

Las reglas de inferencia son esquemas de razonamiento válidos que permiten derivar conclusiones a partir de premisas. Son la base de la demostración formal en lógica.

| Regla | Forma Simbólica | Descripción |
| :--- | :--- | :--- |
| **Modus Ponens** | $p, p \rightarrow q \vdash q$ | Si $p$ es V y $p \rightarrow q$ es V, entonces $q$ es V |
| **Modus Tollens** | $\neg q, p \rightarrow q \vdash \neg p$ | Si $q$ es F y $p \rightarrow q$ es V, entonces $p$ es F |
| **Silogismo hipotético** | $p \rightarrow q, q \rightarrow r \vdash p \rightarrow r$ | Cadena de condicionales |
| **Silogismo disyuntivo** | $p \vee q, \neg p \vdash q$ | Eliminación de una disyunción |
| **Simplificación** | $p \wedge q \vdash p$ | De la conjunción se puede extraer $p$ |
| **Conjunción** | $p, q \vdash p \wedge q$ | De dos verdades se obtiene su conjunción |
| **Adición** | $p \vdash p \vee q$ | Si $p$ es V, $p \vee q$ también lo es |
| **Dilema constructivo** | $(p \rightarrow q) \wedge(r \rightarrow s), p \vee r \vdash q \vee s$ | Combina dos condicionales con disyunción |
</details>

---

## 2. Evidencias de Ejercicios

<details id="2-evidencias-de-ejercicios">
<summary><b>Ver Enlaces de Evidencias</b> (Clic para desplegar)</summary>
<br>

* **2.1 Traducción de lenguaje natural a simbólico:** [Google Drive Folder](https://drive.google.com/drive/folders/1s%208UFLkLbAHji8p5qk3jmsJBgwNfK%209vt?usp=sharing)
* **2.2 Construcción de tabla de verdad:** [Google Drive Folder](https://drive.google.com/drive/folders/1KJceMNXVVJAyT2ike4s0MrNe9Z%206%20NBLT?usp=sharing)
* **2.3 Identificación de tautología, contradicción o contingencia:** [Google Drive Folder](https://drive.google.com/drive/folders/1LINeepisn5ZsB9LNdNYhyUylTbKJ-%206K-?usp=sharing)
* **2.4 Aplicación de leyes proposicionales:** [Google Drive Folder](https://drive.google.com/drive/folders/1y7OB%20O0fdBEZ0NqkaBQZG0KxkZ7%20mAidH?usp=sharing)
* **2.5 Validación de argumento lógico:** [Google Drive Folder](https://drive.google.com/drive/folders/1dyyHIN1voLq9a1xUCqvgYDUnaDdR%20DdBv?usp=sharing)
* **2.6 Portafolio General:** [Google Drive Folder](https://drive.google.com/drive/folders/1WsFIa--QkQ5Ywd0llmL-%20k8olla7CzJkq?usp=sharing)
</details>

---

## 3. Ejercicio Aplicado - Caso Real

<details id="3-ejercicio-aplicado---caso-real">
<summary><b>Ver Caso Aplicado (Estudio en la Biblioteca)</b> (Clic para desplegar)</summary>
<br>

**Situación cotidiana:** Tomar la decisión de salir a estudiar en biblioteca, en función de condiciones reales que se presentan durante la semana universitaria.

### 3.1 Planteamiento del Problema
Como estudiante universitario debo decidir cada día si voy a estudiar en la biblioteca o me quedo en casa. Esta decisión depende de varias condiciones simultáneas que ocurren en mi vida diaria. El objetivo es modelar esta situación con lógica proposicional para razonar formalmente sobre la decisión.

### 3.2 Definición de Proposiciones
| Variable | Proposición | Ejemplo concreto |
| :---: | :--- | :--- |
| **$p$** | Tengo examen mañana | "El docente confirmó la evaluación" |
| **$q$** | La biblioteca está abierta | "El horario de atención lo permite" |
| **$r$** | Terminé mis tareas del día | "No tengo pendientes urgentes" |
| **$s$** | Voy a estudiar a la biblioteca | "Mi decisión final de salir" |

### 3.3 Expresión Simbólica
Las condiciones de mi decisión se pueden expresar como las siguientes proposiciones compuestas:
* **Premisa 1:** Si tengo examen mañana, entonces necesito estudiar: $p \rightarrow s$
* **Premisa 2:** Solo voy a la biblioteca si está abierta Y ya terminé mis tareas: $s \rightarrow (q \wedge r)$
* **Premisa 3:** Hoy tengo examen mañana (dato del contexto): $p$
* **Premisa 4:** La biblioteca está abierta (dato del contexto): $q$
* **Premisa 5:** Terminé mis tareas (dato del contexto): $r$

### 3.4 Análisis con Lógica Proposicional
Aplicando reglas de inferencia paso a paso:

| Paso | Proposición derivada | Justificación |
| :---: | :--- | :--- |
| 1 | $p \text{ (premisa)} \rightarrow s$ | Modus Ponens aplicado a: $p$ y $p \rightarrow s$ |
| 2 | $\rightarrow(q \wedge r)$ <br> $s \text{ (de paso 1)}$ | Modus Ponens aplicado a: $s$ y $s \rightarrow(q \wedge r)$ |
| 3 | $q \text{ (premisa) y } r \text{ (premisa)} \rightarrow q \wedge r$ | Regla de Conjunción |
| 4 | $q \wedge r$ es VERDADERA (paso 3) | La condición del condicional se cumple |
| 5 | Por lo tanto: **$s$ es VERDADERA** | La conclusión del paso 2 es verificada |

### 3.5 Conclusión del Caso
**Conclusión formal:** Dado que $p$ es verdadera (tengo examen), $q$ es verdadera (biblioteca abierta) y $r$ es verdadera (tareas terminadas), se puede inferir lógicamente que $s = \text{VERDADERO}$.

Es decir: **Debo ir a estudiar a la biblioteca.** La decisión no es emocional ni al azar; es el resultado lógico de las condiciones del entorno. La lógica proposicional me permitió estructurar el razonamiento y llegar a una conclusión justificada paso a paso.
</details>

---

## 4. Reflexión Personal

<details id="41-qué-fue-lo-más-difícil-de-entender">
<summary><b>4.1 ¿Qué fue lo más difícil de entender?</b> (Clic para desplegar)</summary>
<br>

Sin duda, lo más desafiante fue comprender el conector condicional $(p \rightarrow q)$. Intuitivamente, me costaba aceptar que, si la premisa $p$ es falsa, la proposición condicional es verdadera sin importar el valor de $q$. Por ejemplo, la proposición *"Si el sol es verde, entonces puedo volar"* resulta verdadera desde el punto de vista lógico, aunque ambas partes sean absurdas en la realidad.

Este "problema" se repite con las tablas de verdad más complejas: cuando hay tres o cuatro variables, la cantidad de combinaciones crece exponencialmente ($2^3=8$ filas, $2^4=16$ filas) y mantener el orden sin cometer errores requería mucha concentración. Al principio confundía las columnas y obtenía resultados incorrectos.

Otro punto difícil fue la aplicación de las leyes de De Morgan en expresiones largas: saber exactamente qué negar y cómo distribuir los conectores al eliminar una negación sobre una conjunción o disyunción compuesta.
</details>

<details id="42-qué-tema-comprendí mejor">
<summary><b>4.2 ¿Qué tema comprendí mejor?</b> (Clic para desplegar)</summary>
<br>

El tema que comprendí con mayor facilidad y que disfruté más fue la construcción de tablas de verdad básicas, especialmente para la conjunción y la disyunción. Una vez que interioricé la "regla mnemotécnica" —la conjunción es como el AND de la electricidad: todo debe estar encendido para que haya resultado— el proceso se volvió muy mecánico y claro.

También encontré lógica (nunca mejor dicho) en las reglas de inferencia, en particular el Modus Ponens. Es exactamente la forma en que razonamos en el día a día: *"Si llueve, me mojo. Está lloviendo. Por lo tanto, me mojo."* Ver que ese razonamiento cotidiano tiene una estructura formal fue uno de los momentos más satisfactorios de la unidad.

Las leyes de equivalencia como la doble negación y las leyes de absorción también me resultaron intuitivas y fáciles de recordar, precisamente porque tienen un correlato natural en el lenguaje hablado.
</details>

<details id="43-cómo-puedo-aplicar-la-lógica-en-mi-carrera">
<summary><b>4.3 ¿Cómo puedo aplicar la lógica en mi carrera?</b> (Clic para desplegar)</summary>
<br>

La lógica proposicional tiene aplicaciones directas y concretas en prácticamente cualquier carrera del área de ciencias, tecnología, ingeniería o matemáticas, pero también en el ámbito humanístico y de gestión. A continuación identifico aplicaciones específicas:

| Área de aplicación | Ejemplo concreto |
| :--- | :--- |
| **Programación** | Las sentencias if-else, while y switch se basan en evaluaciones de verdad/falsedad de condiciones lógicas. |
| **Base de datos** | Las consultas SQL utilizan operadores AND, OR, NOT que corresponden directamente a $\wedge, \vee, \neg$. |
| **Ingeniería de sistemas** | Los circuitos digitales son implementaciones físicas de compuertas lógicas (AND, OR, NOT, NAND, NOR). |
| **Toma de decisiones** | Estructurar condiciones complejas para tomar decisiones empresariales de forma sistemática y libre de sesgos. |
| **Argumentación académica** | Identificar falacias y verificar la validez de argumentos en investigación, debates y proyectos. |
| **Seguridad informática** | Las reglas de firewalls y sistemas de control de acceso siguen patrones de lógica proposicional. |

En definitiva, la lógica proposicional no es simplemente un tema académico abstracto. Es una herramienta del pensamiento que, una vez internalizada, cambia la forma en que se analiza cualquier problema: se aprende a descomponer situaciones complejas en proposiciones simples, a establecer relaciones entre ellas y a llegar a conclusiones justificadas. Eso tiene valor en cualquier campo profesional.
</details>
