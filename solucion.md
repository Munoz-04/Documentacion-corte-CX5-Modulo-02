1. **Documentación breve y clara de cada tema.**  
2. **Ejemplos de código bien explicados.**  
3. **Dos ejercicios intermedios por tema.**  
4. **Preguntas abiertas y teóricas para reforzar conceptos.**  
5. **Un proyecto final integrador.**

Voy a preparar un índice inicial y te detallaré cómo estructuraré el contenido.

---

### **Índice del Documento**

1. **Bucles en JavaScript**  
   * Documentación.  
   * Ejemplos.  
   * Ejercicios intermedios.  
   * Preguntas abiertas y teóricas.  
2. **Arrays en JavaScript**  
   * Documentación.  
   * Ejemplos.  
   * Ejercicios intermedios.  
   * Preguntas abiertas y teóricas.  
3. **Métodos avanzados de Arrays**  
   * Documentación.  
   * Ejemplos.  
   * Ejercicios intermedios.  
   * Preguntas abiertas y teóricas.  
4. **Objetos en JavaScript**  
   * Documentación.  
   * Ejemplos.  
   * Ejercicios intermedios.  
   * Preguntas abiertas y teóricas.  
5. **Funciones y Scope**  
   * Documentación.  
   * Ejemplos.  
   * Ejercicios intermedios.  
   * Preguntas abiertas y teóricas.  
6. **Funciones Flecha y Callbacks**  
   * Documentación.  
   * Ejemplos.  
   * Ejercicios intermedios.  
   * Preguntas abiertas y teóricas.  
7. **Closures y Funciones de Orden Superior**  
   * Documentación.  
   * Ejemplos.  
   * Ejercicios intermedios.  
   * Preguntas abiertas y teóricas.  
8. **Modularización y Reutilización de Código**  
   * Documentación.  
   * Ejemplos.  
   * Ejercicios intermedios.  
   * Preguntas abiertas y teóricas.  
9. **Proyecto Final: Gestor de Tareas Avanzado**  
   * Descripción del proyecto.  
   * Requerimientos.  
   * Pasos sugeridos.  
   * Código base para iniciar.

---

### **Formato por Tema**

#### **1\. Documentación**

* Definición y propósito del tema.  
* Sintaxis clave o estructuras importantes.

#### **2\. Ejemplos**

* Ejemplo sencillo para ilustrar el tema.  
* Ejemplo más elaborado que muestre aplicaciones prácticas.

#### **3\. Ejercicios Intermedios**

* Dos ejercicios diseñados para aplicar los conceptos del tema.  
* Incluyen una pequeña descripción, entrada esperada y resultados deseados.

#### **4\. Preguntas Abiertas y Teóricas**

* 4-5 preguntas para reflexionar sobre la teoría y su uso práctico.

---

### **1\. Bucles en JavaScript**

#### **Documentación**

* **¿Qué son los bucles?**  
  Los bucles permiten ejecutar un bloque de código varias veces mientras una condición sea verdadera. Son esenciales para trabajar con datos repetitivos o iterativos.  
* **Tipos principales de bucles en JavaScript:**  
  * `for`: Ideal cuando sabes cuántas iteraciones necesitas.  
  * `while`: Ejecuta mientras la condición sea verdadera.  
  * `do...while`: Similar al `while`, pero ejecuta el bloque al menos una vez.

---

#### **Ejemplo 1: Imprimir números del 1 al 10 con `for`**

`for (let i = 1; i <= 10; i++) {`  
    ``console.log(`Número: ${i}`);``  
`}`  
`// Salida:`  
`// Número: 1`  
`// Número: 2`  
`// ...`  
`// Número: 10`

**Explicación paso a paso:**

1. **Inicialización:** `let i = 1` establece la variable `i` en 1\.  
2. **Condición:** El bucle continúa mientras `i <= 10`.  
3. **Incremento:** Después de cada iteración, `i` aumenta en 1 (`i++`).

---

#### **Ejemplo 2: Encontrar números pares entre 1 y 20 con `while`**

`let i = 1;`  
`while (i <= 20) {`  
    `if (i % 2 === 0) {`  
        ``console.log(`${i} es par`);``  
    `}`  
    `i++;`  
`}`  
`// Salida:`  
`// 2 es par`  
`// 4 es par`  
`// ...`  
`// 20 es par`

**Explicación paso a paso:**

1. Inicializamos `i = 1`.  
2. Evaluamos `i % 2 === 0`. Si el residuo es 0, el número es par.  
3. Incrementamos `i` en cada iteración.

---

#### **Ejercicios Intermedios**

**Imprimir números primos entre 1 y 50** **Descripción:** Crear un programa que identifique y muestre los números primos entre 1 y 50\.  
**Solución paso a paso:**

1.   
   * **Bucle externo:** Itera sobre números del 2 al 50\.  
   * **Bucle interno:** Verifica si el número tiene divisores.  
   * Si no tiene divisores, es primo.

for (let num = 1; num <= 50; num++){
  let esPrimo = true;

  for (let i = 2; i < num ; i++) {
    if (num % i === 0){
      esPrimo = false;
      break
    }
  }
  if (esPrimo && num > 1) {
    console.log(num)
  }
}

---

**Generar la tabla de multiplicar de un número ingresado** **Descripción:** Pedir al usuario un número y mostrar su tabla de multiplicar hasta el 10\.  
**Solución paso a paso:**

2.   
   * **Prompt:** Solicita un número al usuario.  
   * **Bucle `for`:** Itera del 1 al 10\.  
   * **Salida:** Muestra el resultado de la multiplicación.

---
let numeroAsolicitar = 2;

for(i = 1; i<= 10; i++){
  console.log(i*numeroAsolicitar)
}

#### **Preguntas Abiertas y Teóricas**

1. ¿Cuál es la diferencia entre un bucle `for` y un bucle `while`?
- El bucle `for` es útil cuando sabes cuántas veces quieres iterar, y el `while` es útil cuando no lo sabes y la ejecución depende de una condición dinámica.
2. ¿Qué sucede si omites el incremento en un bucle `for`?  
- El bucle entra en un ciclo infinito y la variable de control no se actualiza.
3. ¿Qué problema puede ocurrir si un bucle `while` no tiene una condición de finalización válida?
- Cuando el bucle while no tiene una condicion de finalizacion valida ella adentra en un Bucle infinito.

### **2\. Arrays en JavaScript**

#### **Documentación**

**¿Qué son los arrays?**  
Los arrays son estructuras de datos que permiten almacenar múltiples valores en una sola variable. Cada elemento tiene un índice, que comienza en 0\.

`let frutas = ["manzana", "naranja", "plátano"];`  
`console.log(frutas[0]); // "manzana"`

*   
* **Métodos básicos:**  
  * `push(elemento)`: Agrega un elemento al final del array.  
  * `pop()`: Elimina el último elemento.  
  * `unshift(elemento)`: Agrega un elemento al inicio.  
  * `shift()`: Elimina el primer elemento.

---

#### **Ejemplo 1: Crear y modificar un array**

`let colores = ["rojo", "verde", "azul"];`  
`colores.push("amarillo"); // ["rojo", "verde", "azul", "amarillo"]`  
`colores.pop();            // ["rojo", "verde", "azul"]`  
`colores.unshift("blanco"); // ["blanco", "rojo", "verde", "azul"]`  
`colores.shift();           // ["rojo", "verde", "azul"]`  
`console.log(colores);      // ["rojo", "verde", "azul"]`

**Explicación paso a paso:**

1. Creamos un array con tres colores.  
2. Usamos `push` para agregar "amarillo" al final.  
3. Usamos `pop` para eliminar el último elemento.  
4. Usamos `unshift` para agregar "blanco" al inicio.  
5. Usamos `shift` para eliminar el primer elemento.

---

#### **Ejemplo 2: Iterar sobre un array**

`let numeros = [10, 20, 30, 40];`  
`for (let i = 0; i < numeros.length; i++) {`  
    ``console.log(`Elemento ${i}: ${numeros[i]}`);``  
`}`  
`// Salida:`  
`// Elemento 0: 10`  
`// Elemento 1: 20`  
`// Elemento 2: 30`  
`// Elemento 3: 40`

**Explicación paso a paso:**

1. Iteramos desde `i = 0` hasta `numeros.length - 1`.  
2. En cada iteración, accedemos al elemento con `numeros[i]`.  
3. Imprimimos el índice y el valor.

---

#### **Ejercicios Intermedios**

**Gestión de asistentes con un array**  
**Descripción:**  
Crear un programa que permita agregar, eliminar y listar asistentes de un evento usando métodos básicos de arrays.  
**Solución paso a paso:**

1. 

---

let asistentes = [];

function agregarAsistente(nombre) {
    asistentes.push(nombre);
    console.log(`${nombre} ha sido agregado como asistente.`);
}

function eliminarAsistente(nombre) {
    const index = asistentes.indexOf(nombre);
    if (index !== -1) {
        asistentes.splice(index, 1);
        console.log(`${nombre} ha sido eliminado de la lista de asistentes.`);
    } else {
        console.log(`El asistente ${nombre} no se encuentra en la lista.`);
    }
}

function listarAsistentes() {
    if (asistentes.length === 0) {
        console.log("No hay asistentes en la lista.");
    } else {
        console.log("Lista de asistentes:");
        asistentes.forEach((asistente, index) => {
            console.log(`${index + 1}. ${asistente}`);
        });
    }
}

**Encontrar el número más alto y más bajo en un array**  
**Descripción:**  
Crear un programa que recorra un array y encuentre el número más alto y el más bajo.  
**Solución paso a paso:**

2.   
   * Inicializamos `max` y `min` con el primer elemento del array.  
   * Iteramos desde el segundo elemento (`i = 1`) para comparar cada valor con `max` y `min`.  
   * Actualizamos `max` y `min` según sea necesario.

---

function encontrarMaximoyMinimo(valores){
  if (valores.length === 0){
    console.log("El array está vacio");
    return;
  }
}

let valorMaximo = [0];
let valorMinimo = [0];

for (let i = 1; i < valores.lenght ; i++){
  if(valores[i]>max){
    max = valores[i]
  } if (valores[i]< min){
    min = valores[i]
  }
  console.log(`El valor mas alto es ${max}`)
  console.log(`El valor mas bajo es ${min}`)
}

const valores = [2 , 3 , 5, 6, 10 , 12]

encontrarMaximoyMinimo(valores);

#### **Preguntas Abiertas y Teóricas**

1. ¿Qué ventaja tiene usar arrays en lugar de variables individuales?
- La ventaja es que conseguimos guardar varios datos de manera organizada en una misma variable.  
2. ¿Qué sucede si intentas acceder a un índice que no existe en un array?
- El sistema indicará un undefined,   
3. Explica la diferencia entre `push` y `unshift`.
- Push - agrega un elemento al final del array.
- Unshift - agrega un elemento al inicio del array. 
4. ¿Cómo puedes saber cuántos elementos hay en un array?
- Usando la propriedade .length. Exemplo : numeros.length.

### **3\. Métodos avanzados de Arrays**

#### **Documentación**

Los métodos avanzados de arrays permiten realizar operaciones complejas de manera más legible y eficiente que con bucles tradicionales.

**`map()`**: Crea un nuevo array aplicando una función a cada elemento.

`let numeros = [1, 2, 3];`  
`let cuadrados = numeros.map(n => n * n); // [1, 4, 9]`

* 

**`filter()`**: Crea un nuevo array con los elementos que cumplen una condición.

`let numeros = [1, 2, 3, 4, 5];`  
`let pares = numeros.filter(n => n % 2 === 0); // [2, 4]`

* 

**`reduce()`**: Reduce un array a un único valor, acumulando resultados.

`let numeros = [1, 2, 3, 4];`  
`let suma = numeros.reduce((total, n) => total + n, 0); // 10`

* 

---

#### **Ejemplo 1: Usar `map` para transformar datos**

`let precios = [100, 200, 300];`  
`let preciosConIVA = precios.map(precio => precio * 1.21);`  
`console.log(preciosConIVA); // [121, 242, 363]`

**Explicación paso a paso:**

1. Declaramos un array con precios originales.  
2. Usamos `map` para multiplicar cada precio por 1.21 (añadiendo el IVA).  
3. El resultado es un nuevo array con los precios actualizados.

---

#### **Ejemplo 2: Filtrar números mayores a 10 con `filter`**

`let numeros = [5, 10, 15, 20];`  
`let mayoresADiez = numeros.filter(n => n > 10);`  
`console.log(mayoresADiez); // [15, 20]`

**Explicación paso a paso:**

1. Declaramos un array con números.  
2. Usamos `filter` para seleccionar solo los números mayores a 10\.  
3. El resultado es un nuevo array con los números que cumplen la condición.

---

#### **Ejemplo 3: Calcular el total de ventas con `reduce`**

`let ventas = [500, 1200, 300, 800];`  
`let total = ventas.reduce((acumulado, venta) => acumulado + venta, 0);`  
``console.log(`Total de ventas: $${total}`); // Total de ventas: $2800``

**Explicación paso a paso:**

1. Declaramos un array con los montos de ventas.  
2. Usamos `reduce` para sumar todos los elementos.  
3. El acumulador inicia en 0 y se actualiza con cada venta.

---

#### **Ejercicios Intermedios**

**Filtrar números pares e imprimir su cuadrado** **Descripción:**  
Crear un programa que filtre los números pares de un array y luego devuelva un nuevo array con sus cuadrados.  
**Solución paso a paso:**

* Usamos `filter` para seleccionar números pares.  
  * Usamos `map` para calcular el cuadrado de cada par.  
  * El resultado es un array con los cuadrados de los números pares.

---

let numero = [1,2,3,4,5,6,7,8,9];

let resultado = numero
  resultado = resultado.filter(num => num % 2 === 0);
  resultado = resultado.map(n => n * n);

console.log(resultado);


**Calcular el promedio de un array** **Descripción:**  
Usar `reduce` para calcular el promedio de un array de números.  
**Solución paso a paso:**

2.   
   * Usamos `reduce` para obtener la suma total.  
   * Dividimos la suma entre la longitud del array para obtener el promedio.

---

let num = [1,2,3,4,5,6]

let suma = num.reduce((total,n)=> total+n,0);

console.log(suma/num.length)

#### **Preguntas Abiertas y Teóricas**

1. ¿Cuál es la diferencia entre `map` y `forEach`? 

- map - Crea un nuevo array basado en la transformacion de los elementos del array original.
- forEach - Solo itera sobre el array y ejecuta una función para cada elemento, pero no devuelve un nuevo array. 

2. Explica un caso práctico donde usarías `filter`.

- Se utiliza cuando necesitas crear un nuevo array con los elementos que cumplen con una condición específica.

3. ¿Qué sucede si omites el segundo parámetro de `reduce`?  

El segundo paramentro del reduce es el valor inicial da sumatoria, si caso lo omite, la primera iteración tomará el primer elemento del array como valor inicial del acumulador. 

4. ¿Cómo puedes combinar `map` y `filter` en una sola operación?

Puedes combinar map y filter para primero filtrar los elementos del array y luego aplicar una transformación a los elementos filtrados. 


### **4\. Objetos en JavaScript**

#### **Documentación**

**¿Qué son los objetos?**  
Un objeto es una colección de pares clave-valor. Las claves son identificadores únicos, y los valores pueden ser cualquier tipo de dato, incluyendo funciones.

`let persona = {`  
    `nombre: "Juan",`  
    `edad: 25,`  
    `saludar: function() {`  
        ``return `Hola, soy ${this.nombre}`;``  
    `}`  
`};`

*   
* **Acceso a propiedades:**  
  * Notación de punto: `persona.nombre`  
  * Notación de corchetes: `persona["edad"]`

**Modificar propiedades:**

`persona.nombre = "Carlos";`  
`persona["edad"] = 30;`

* 

**Agregar nuevas propiedades:**

`persona.ciudad = "Madrid";`

* 

**Eliminar propiedades:**

`delete persona.edad;`

* 

---

#### **Ejemplo 1: Crear y usar un objeto**

`let producto = {`  
    `nombre: "Laptop",`  
    `precio: 1500,`  
    `disponible: true`  
`};`

`console.log(producto.nombre); // "Laptop"`  
`producto.precio = 1400;       // Modificar precio`  
`producto.categoria = "Tecnología"; // Agregar nueva propiedad`  
`console.log(producto);`

**Explicación paso a paso:**

1. Creamos un objeto con tres propiedades (`nombre`, `precio`, `disponible`).  
2. Accedemos a `nombre` usando la notación de punto.  
3. Modificamos `precio` asignándole un nuevo valor.  
4. Agregamos una nueva propiedad `categoria`.

---

#### **Ejemplo 2: Métodos en objetos**

`let vehiculo = {`  
    `marca: "Toyota",`  
    `modelo: "Corolla",`  
    `encender: function() {`  
        `console.log("El vehículo está encendido");`  
    `}`  
`};`

`vehiculo.encender(); // "El vehículo está encendido"`

**Explicación paso a paso:**

1. Creamos un objeto `vehiculo` con dos propiedades (`marca`, `modelo`) y un método (`encender`).  
2. Llamamos al método `encender`, que ejecuta el bloque de código definido.

---

#### **Ejemplo 3: Iterar sobre un objeto**

`let estudiante = {`  
    `nombre: "Laura",`  
    `edad: 21,`  
    `carrera: "Ingeniería"`  
`};`

`for (let clave in estudiante) {`  
    ``console.log(`${clave}: ${estudiante[clave]}`);``  
`}`  
`// Salida:`  
`// nombre: Laura`  
`// edad: 21`  
`// carrera: Ingeniería`

**Explicación paso a paso:**

1. Usamos un bucle `for...in` para iterar sobre las claves del objeto.  
2. Accedemos al valor de cada clave con la notación de corchetes.

---

#### **Ejercicios Intermedios**

**Crear un objeto "Libro" con propiedades y métodos**  
**Descripción:**  
Crear un objeto que represente un libro, con las propiedades `titulo`, `autor`, y `numPaginas`. Agregar un método para mostrar la información del libro en un string.  
**Solución paso a paso:**

* Creamos un objeto con las propiedades indicadas.  
  * Añadimos el método `informacion` que usa `this` para acceder a las propiedades.

---

let libro = {  
    nombre: "Matrix",  
    autor: "Keano Reaves",
    numPaginas: 300,  
    informacion: function() {  
        console.log(this.nombre , this.autor , this.numPaginas );  
   }  
};

libro.informacion()

**Crear un inventario de productos**  
**Descripción:**  
Crear un array de objetos que represente un inventario de productos, con cada objeto conteniendo `nombre`, `precio`, y `cantidad`. Implementar una función que calcule el valor total del inventario.  
**Solución paso a paso:**

2.   
   * Creamos un array de objetos para representar los productos.  
   * Usamos `reduce` para calcular el valor total del inventario.

---

let material = [
  {nombre: "caneta", precio: 5,cantidad: 10 },
  {nombre: "boracha", precio: 15,cantidad: 5 },
  {nombre: "caderno", precio: 25,cantidad: 5 }
]

function calcularValorTotal(material) {
  return material.reduce((total, producto) => {
    return total + (producto.precio * producto.cantidad);
  }, 0);
}

const valorTotal = calcularValorTotal(material);

console.log(valorTotal)

#### **Preguntas Abiertas y Teóricas**

1. ¿Qué diferencia hay entre un objeto y un array en JavaScript?  

- Objetos: Usan claves para acceder a los valores.
- Arrays: Usan índices numéricos para acceder a los valores.

2. Explica cómo accederías a una propiedad con un nombre almacenado en una variable.  

- Usamos persona[propiedad] para acceder a la propiedad cuyo nombre está almacenado en la variable propiedad.

3. ¿Cómo puedes iterar sobre todas las claves de un objeto?

Para iterar sobre todas las claves de un objeto, puedes usar:

    - for...in: Es un bucle específico para recorrer las propiedades enumerables de un objeto.
   -  Object.keys(): Devuelve un array con las claves del objeto, lo que te permite usar métodos como forEach, map, o for...of.

4. ¿Qué sucede si intentas acceder a una propiedad que no existe?

- Si intentas acceder a una propiedad que no existe en un objeto, JavaScript devolverá undefined.

### **5\. Funciones y Scope**

#### **Documentación**

**¿Qué son las funciones?**  
Las funciones son bloques de código reutilizables que realizan una tarea específica. Pueden recibir parámetros y devolver resultados.  
**Sintaxis básica:**

`function saludar(nombre) {`  
    ``return `Hola, ${nombre}!`;``  
`}`  
`console.log(saludar("Ana")); // "Hola, Ana!"`

*   
* **Scope:**  
  Define dónde pueden accederse las variables en el código.  
  * **Global:** Las variables declaradas fuera de funciones pueden ser accedidas desde cualquier parte del programa.  
  * **Local:** Variables declaradas dentro de una función o bloque solo son accesibles dentro de ese ámbito.

**Ejemplo:**

`let global = "Hola";`  
`function ejemplo() {`  
    `let local = "Mundo";`  
    `console.log(global); // "Hola"`  
    `console.log(local);  // "Mundo"`  
`}`  
`ejemplo();`  
`console.log(local);      // Error: local no está definida`

* 

---

#### **Ejemplo 1: Función que calcula el área de un rectángulo**

`function calcularAreaRectangulo(base, altura) {`  
    `return base * altura;`  
`}`  
`console.log(calcularAreaRectangulo(5, 10)); // 50`

**Explicación paso a paso:**

1. Declaramos la función `calcularAreaRectangulo` con dos parámetros (`base`, `altura`).  
2. La función retorna el producto de `base` y `altura`.  
3. Llamamos a la función con valores específicos.

---

#### **Ejemplo 2: Scope global y local**

`let mensaje = "Mensaje global";`

`function mostrarMensaje() {`  
    `let mensaje = "Mensaje local";`  
    `console.log(mensaje); // "Mensaje local"`  
`}`

`mostrarMensaje();`  
`console.log(mensaje); // "Mensaje global"`

**Explicación paso a paso:**

1. Declaramos una variable global `mensaje`.  
2. Dentro de la función `mostrarMensaje`, declaramos otra variable `mensaje` que es local.  
3. La función accede a su variable local, mientras el código global accede a la variable global.

---

#### **Ejemplo 3: Funciones anidadas y scope**

`function exterior() {`  
    `let mensaje = "Desde exterior";`

    `function interior() {`  
        `console.log(mensaje);`  
    `}`

    `interior();`  
`}`

`exterior(); // "Desde exterior"`

**Explicación paso a paso:**

1. La función `interior` está anidada dentro de `exterior`.  
2. `interior` puede acceder a la variable `mensaje` porque pertenece al scope de `exterior`.

---

#### **Ejercicios Intermedios**

**Crear una función que determine si un número es par o impar**  
**Descripción:**  
Escribir una función que reciba un número y devuelva `"par"` si el número es par o `"impar"` si es impar.  
**Solución paso a paso:**

1.   
   * Usamos el operador `%` para determinar si el residuo al dividir entre 2 es 0\.  
   * Utilizamos el operador ternario para devolver el resultado.

---

let entrada = 2;

function parouImpar(){

  if(entrada % 2 === 0){
    console.log(`Este valor es par`)
  } else {
    console.log(`Este valor es impar`)
  }
}

parouImpar(entrada);

**Crear una función que devuelva la suma de los números de un array**  
**Descripción:**  
Crear una función que reciba un array de números y retorne la suma de sus elementos.  
**Solución paso a paso:**

2.   
   * Declaramos una variable `suma` inicializada en 0\.  
   * Usamos un bucle `for...of` para recorrer el array y sumar cada elemento.

---

function sumarVetor (arr) {
  return arr.reduce((sumatorio,valorAtual)=>sumatorio + valorAtual,0);
}

let numeros = [5,2,4,5,6,7]

let suma = sumarVetor(numeros)

console.log(suma)

#### **Preguntas Abiertas y Teóricas**

1. Explica la diferencia entre el scope global y local.
- Scope global vs local: Las variables en el scope global son accesibles desde cualquier parte del código, mientras que las variables en el scope local solo son accesibles dentro de la función o bloque donde fueron declaradas.
2. ¿Qué sucede si declaras una variable sin `let`, `const` o `var` dentro de una función?  
- Declarar variable sin let, const, o var: Si lo haces dentro de una función, JavaScript crea una variable global, lo cual puede generar problemas y es una mala práctica.

3. ¿Por qué es importante reutilizar código usando funciones?  
- Es importante para la modularidad, reducción de errores, mantenimiento, legibilidad y optimización del código.

4. ¿Qué pasa si intentas acceder a una variable declarada dentro de una función desde el código global?
- No puedes acceder a variables locales fuera de su función, ya que están limitadas al scope de esa función.
### **6\. Funciones Flecha y Callbacks**

#### **Documentación**

**Funciones Flecha:**  
Son una sintaxis más concisa para declarar funciones introducida en ES6. No tienen su propio `this`, lo que las hace ideales para ciertas tareas como callbacks o funciones simples.  
**Sintaxis básica:**

`// Función tradicional`  
`function sumar(a, b) {`  
    `return a + b;`  
`}`

`// Función flecha equivalente`  
`const sumar = (a, b) => a + b;`

`console.log(sumar(3, 4)); // 7`

* 

**Callbacks:**  
Son funciones que se pasan como argumentos a otras funciones y se ejecutan dentro de ellas, permitiendo personalizar su comportamiento.  
**Ejemplo básico de callback:**

`function procesarUsuario(nombre, callback) {`  
    ``console.log(`Procesando a ${nombre}`);``  
    `callback();`  
`}`

`procesarUsuario("Ana", () => console.log("¡Usuario procesado!"));`

* 

---

#### **Ejemplo 1: Usar funciones flecha para cálculos simples**

`const duplicar = num => num * 2;`  
`const sumar = (a, b) => a + b;`

`console.log(duplicar(5)); // 10`  
`console.log(sumar(3, 7)); // 10`

**Explicación paso a paso:**

1. Declaramos una función flecha `duplicar` que recibe un número y devuelve su doble.  
2. Declaramos otra función flecha `sumar` que toma dos números y retorna su suma.  
3. Llamamos a las funciones y mostramos los resultados.

---

#### **Ejemplo 2: Callback en un proceso asíncrono**

`setTimeout(() => {`  
    `console.log("Esto se ejecuta después de 2 segundos");`  
`}, 2000);`

**Explicación paso a paso:**

1. Usamos `setTimeout`, que recibe una función (callback) y un tiempo en milisegundos.  
2. La función flecha se ejecuta tras 2 segundos.

---

#### **Ejemplo 3: Uso combinado de funciones flecha y callbacks**

``const saludar = nombre => console.log(`Hola, ${nombre}!`);``  
`const procesarSaludo = (nombre, callback) => {`  
    `console.log("Procesando saludo...");`  
    `callback(nombre);`  
`};`

`procesarSaludo("Carlos", saludar);`  
`// Salida:`  
`// Procesando saludo...`  
`// Hola, Carlos!`

**Explicación paso a paso:**

1. Declaramos una función flecha `saludar` para imprimir un saludo.  
2. Creamos una función `procesarSaludo` que toma un nombre y un callback.  
3. Llamamos a `procesarSaludo` pasando `saludar` como callback.

---

#### **Ejercicios Intermedios**

**Crear un programa que use un callback para procesar números**  
**Descripción:**  
Escribir una función que reciba un array de números y un callback que determine qué hacer con esos números (por ejemplo, imprimirlos o sumarlos).  
**Solución paso a paso:**

1.   
   * La función `procesarNumeros` toma un array y un callback.  
   * Itera sobre los números y ejecuta el callback en cada uno.

---

function procesarNumeros(arr, callback) {
  return callback(arr);
}

function sumarNumeros(arr) {
  return arr.reduce((acumulador, valorActual) => acumulador + valorActual, 0);
}

function imprimirNumeros(arr) {
  arr.forEach(num => console.log(num));
}


let numeros = [1, 2, 3, 4, 5];

let suma = procesarNumeros(numeros, sumarNumeros);
console.log("Suma de los números:", suma);  // Suma de los números: 15

console.log("Imprimiendo los números:");
procesarNumeros(numeros, imprimirNumeros);


**Simular un proceso asíncrono con callbacks**  
**Descripción:**  
Crear un programa que simule una consulta a una base de datos, usando un callback para mostrar los resultados tras 3 segundos.  
**Solución paso a paso:**

2.   
   * Simulamos un retraso con `setTimeout`.  
   * El callback `mostrarUsuario` se ejecuta con los datos después de 3 segundos.

---

function consultarBaseDeDatos(callback) {
  console.log("Realizando consulta a la base de datos...");

  setTimeout(() => {
    const resultados = [
      { id: 1, nombre: "Producto 1", precio: 100 },
      { id: 2, nombre: "Producto 2", precio: 150 },
      { id: 3, nombre: "Producto 3", precio: 200 }
    ];

    callback(resultados);
  }, 3000); // Esperamos 3 segundos
}


function mostrarResultados(resultados) {
  console.log("Consulta completada. Resultados:");
  resultados.forEach(producto => {
    console.log(`ID: ${producto.id}, Nombre: ${producto.nombre}, Precio: $${producto.precio}`);
  });
}

consultarBaseDeDatos(mostrarResultados);


#### **Preguntas Abiertas y Teóricas**

1. ¿En qué situaciones las funciones flecha son más útiles que las funciones tradicionales?  
- Las funciones flecha son más útiles cuando se necesita una sintaxis concisa, especialmente en callbacks o funciones pequeñas, y cuando se quiere preservar el contexto de this.
2. Explica por qué las funciones flecha no tienen su propio contexto de `this`.  
- this en funciones flecha: Las funciones flecha no tienen su propio this; en su lugar, heredan el this del contexto léxico donde fueron definidas.
3. ¿Cuál es la ventaja de usar callbacks en procesos asíncronos? 
- Los callbacks permiten manejar procesos asíncronos sin bloquear el hilo de ejecución, lo que mejora la eficiencia y la capacidad de respuesta de las aplicaciones. 
4. ¿Qué sucedería si pasas un callback incorrecto a una función?
- Si se pasa un callback incorrecto, pueden ocurrir errores de tipo, comportamiento inesperado o incluso fallos en la ejecución, lo que puede causar que el programa no funcione correctamente.

### **7\. Closures y Funciones de Orden Superior**

#### **Documentación**

**Closures:**  
Un closure es una función que "recuerda" el contexto en el que fue creada, incluso después de que ese contexto haya terminado. Esto ocurre porque las funciones en JavaScript "encierran" las variables de su entorno léxico.  
**Ejemplo básico:**

`function crearContador() {`  
    `let contador = 0;`  
    `return function () {`  
        `contador++;`  
        `return contador;`  
    `};`  
`}`

`const contador1 = crearContador();`  
`console.log(contador1()); // 1`  
`console.log(contador1()); // 2`

* **Cómo funciona:**  
  * `contador` se declara en el contexto de `crearContador`.  
  * La función interna accede a `contador` incluso después de que `crearContador` haya terminado.

**Funciones de Orden Superior:**  
Son funciones que reciben otras funciones como parámetros o las devuelven como resultado.  
**Ejemplo básico:**

`const aplicarOperacion = (num, operacion) => operacion(num);`

`const duplicar = n => n * 2;`  
`console.log(aplicarOperacion(5, duplicar)); // 10`

* **Cómo funciona:**  
  * `aplicarOperacion` recibe un número y una función `operacion`.  
  * Aplica `operacion` al número.

---

#### **Ejemplo 1: Closure que guarda un valor inicial**

`function crearSaludo(saludo) {`  
    `return function (nombre) {`  
        ``return `${saludo}, ${nombre}!`;``  
    `};`  
`}`

`const saludarEnEspañol = crearSaludo("Hola");`  
`const saludarEnIngles = crearSaludo("Hello");`

`console.log(saludarEnEspañol("Carlos")); // "Hola, Carlos!"`  
`console.log(saludarEnIngles("John"));    // "Hello, John!"`

**Explicación paso a paso:**

1. `crearSaludo` toma un saludo como argumento.  
2. Devuelve una función que usa el saludo y el nombre.  
3. Creamos funciones específicas (`saludarEnEspañol`, `saludarEnIngles`) que recuerdan el saludo inicial.

---

#### **Ejemplo 2: Función de Orden Superior con `filter`**

`const filtrarArray = (array, condicion) => array.filter(condicion);`

`const esPar = num => num % 2 === 0;`  
`const numeros = [1, 2, 3, 4, 5, 6];`

`console.log(filtrarArray(numeros, esPar)); // [2, 4, 6]`

**Explicación paso a paso:**

1. `filtrarArray` es una función de orden superior que usa `filter`.  
2. `esPar` verifica si un número es par.  
3. Aplicamos `filtrarArray` para filtrar los números pares.

---

#### **Ejemplo 3: Closure para almacenar datos**

`function crearAlmacen() {`  
    `let almacen = [];`  
    `return {`  
        `agregar: item => almacen.push(item),`  
        `obtener: () => [...almacen],`  
    `};`  
`}`

`const miAlmacen = crearAlmacen();`  
`miAlmacen.agregar("Manzana");`  
`miAlmacen.agregar("Naranja");`  
`console.log(miAlmacen.obtener()); // ["Manzana", "Naranja"]`

**Explicación paso a paso:**

1. `crearAlmacen` crea un array `almacen` dentro de su contexto.  
2. Devuelve dos métodos: `agregar` para añadir elementos y `obtener` para recuperar los datos.  
3. Usamos `miAlmacen` para interactuar con los datos, protegidos por el closure.

---

#### **Ejercicios Intermedios**

**Crear un contador con incrementos personalizados**  
**Descripción:**  
Escribir una función que tome un número inicial y un incremento, y devuelva un closure que aumente el número inicial por el incremento cada vez que se llame.  
**Solución paso a paso:**

`—--------------------:`

1.   
   * Declaramos `contador` con el valor inicial.  
   * El closure incrementa el contador cada vez que se llama.

---

function crearContador(inicial, incremento) {
  
  let numero = inicial;
  
  return function() {
    numero += incremento;  // Aumenta el número por el incremento
    return numero;         // Devuelve el número actualizado
  };
}

const contador = crearContador(5, 3); /

console.log(contador()); 
console.log(contador()); 
console.log(contador()); 

**Crear una función que transforme un array de números**  
**Descripción:**  
Crear una función de orden superior que tome un array y una función de transformación, y devuelva un nuevo array con los elementos transformados.  
**Solución paso a paso:**  
—-------------:

2.   
   * `transformarArray` usa `map` para aplicar la transformación.  
   * La función `alCuadrado` transforma cada elemento del array.

---

function transformarArray(arr, transformacion) {

  let resultado = [];
  
  for (let i = 0; i < arr.length; i++) {
    resultado.push(transformacion(arr[i]));  // Aplicamos la transformación a cada elemento
  }
  
  return resultado;  // Devolvemos el nuevo array transformado
}


function multiplicarPorDos(numero) {
  return numero * 2;
}

const numeros = [1, 2, 3, 4, 5];

const numerosTransformados = transformarArray(numeros, multiplicarPorDos);

console.log(numerosTransformados);


#### **Preguntas Abiertas y Teóricas**

1. ¿Qué ventaja ofrece un closure frente a variables globales?  
- Los closures permiten encapsular datos, evitando el uso de variables globales, lo que mejora la seguridad, el control sobre los datos y evita conflictos de nombres.
2. Explica cómo puedes usar closures para proteger datos.
- Los closures permiten crear datos privados que solo pueden ser modificados o leídos mediante funciones específicas, manteniendo la privacidad y seguridad de los datos.  
3. ¿Qué es una función de orden superior y en qué casos es útil? 
- Son funciones que aceptan otras funciones como parámetros o devuelven funciones. Son útiles en casos como callbacks, composición de funciones y transformación de datos. 
4. Describe cómo puedes combinar `map` con funciones de orden superior.
- Puedes combinar map con otras funciones de orden superior como filter, reduce, etc., para realizar transformaciones y operaciones complejas sobre colecciones de datos de manera más declarativa y modular.

### **8\. Modularización y Reutilización de Código**

#### **Documentación**

* **¿Qué es la modularización?**  
  La modularización divide el código en partes más pequeñas y manejables, llamadas módulos. Cada módulo se encarga de una funcionalidad específica, facilitando la reutilización y el mantenimiento del código.  
* **Sintaxis básica de módulos (ES6):**

Exportar desde un módulo:

``export const saludar = nombre => `Hola, ${nombre}!`;``

* 

Importar en otro archivo:

`import { saludar } from './archivo.js';`  
`console.log(saludar("Juan")); // "Hola, Juan!"`

*   
* **Ventajas de la modularización:**  
  * Código más organizado y fácil de entender.  
  * Reutilización de componentes en diferentes partes del proyecto.  
  * Facilita las pruebas y depuración.

---

#### **Ejemplo 1: Dividir funciones en módulos**

**Contexto:**  
Tienes un archivo `math.js` que contiene funciones para sumar, restar y multiplicar. Puedes importarlas en un archivo principal `app.js` para utilizarlas.

1. Crea un archivo llamado `math.js` y escribe las funciones `sumar`, `restar`, y `multiplicar`.  
2. Usa `export` para que las funciones estén disponibles en otros archivos.  
3. En el archivo `app.js`, importa las funciones desde `math.js`.  
4. Utiliza las funciones en `app.js` para realizar operaciones matemáticas.

---
`math.js`
export function sumar(a, b) {
    return a + b;
}

export function restar(a, b) {
    return a - b;
}

export function multiplicar(a, b) {
    return a * b;
}

`app.js`
import { agregarProducto, eliminarProducto, calcularTotal, obtenerCarrito } from './carrito.js';

agregarProducto({ nombre: 'Manzanas', precio: 2, cantidad: 5 });
agregarProducto({ nombre: 'Pan', precio: 1.5, cantidad: 2 });
agregarProducto({ nombre: 'Leche', precio: 3, cantidad: 1 });

console.log('Carrito actual:', obtenerCarrito());


eliminarProducto('Pan');
console.log('Carrito después de eliminar Pan:', obtenerCarrito());

const total = calcularTotal();
console.log('Total a pagar:', total);


#### **Ejemplo 2: Crear módulos reutilizables en un carrito de compras**

**Contexto:**  
Un sistema de carrito de compras tiene funciones para agregar, eliminar y calcular el total de los productos.

1. Crea un archivo `carrito.js` que contenga las funciones necesarias: `agregarProducto`, `eliminarProducto` y `calcularTotal`.  
2. Usa un array para almacenar los productos y actualízalo con las funciones.  
3. Exporta las funciones para usarlas en otros archivos.  
4. En el archivo principal, importa las funciones y pruébalas simulando la interacción con el carrito.

---
`carrito.js`
let carrito = [];

export function agregarProducto(producto) {
    carrito.push(producto);
}

export function eliminarProducto(nombreProducto) {
    carrito = carrito.filter(producto => producto.nombre !== nombreProducto);
}

export function calcularTotal() {
    return carrito.reduce((total, producto) => total + producto.precio * producto.cantidad, 0);
}

export function obtenerCarrito() {
    return carrito;
}

`app.js`
import { agregarProducto, eliminarProducto, calcularTotal, obtenerCarrito } from './carrito.js';

agregarProducto({ nombre: 'Manzanas', precio: 2, cantidad: 5 });
agregarProducto({ nombre: 'Pan', precio: 1.5, cantidad: 2 });
agregarProducto({ nombre: 'Leche', precio: 3, cantidad: 1 });

console.log('Carrito actual:', obtenerCarrito());


eliminarProducto('Pan');
console.log('Carrito después de eliminar Pan:', obtenerCarrito());

const total = calcularTotal();
console.log('Total a pagar:', total);


#### **Ejercicios Intermedios**

1. **Dividir un programa de cálculo de áreas en módulos**  
   **Descripción:**  
   Diseña un programa que calcule el área de figuras geométricas (círculo, cuadrado, triángulo) y organiza cada cálculo en un módulo diferente.  
   **Pasos para resolverlo:**  
   1. Crea un archivo para cada figura: `circulo.js`, `cuadrado.js`, `triangulo.js`.  
   2. En cada archivo, escribe una función que reciba las dimensiones necesarias (por ejemplo, el radio para el círculo).  
   3. Usa `export` para hacer que cada función esté disponible en otros archivos.  
   4. Crea un archivo principal, `app.js`, e importa todas las funciones de cálculo.  
   5. Prueba las funciones llamándolas con diferentes valores y muestra los resultados.

---
`circulo.js`
export function areaCirculo(radio) {
  return Math.PI * radio * radio;
}

 `cuadrado.js`
export function areaCuadrado(lado) {
  return lado * lado;
}

 `triangulo.js`
export function areaTriangulo(base, altura) {
  return (base * altura) / 2;
}

import { areaCirculo } from './circulo.js';
import { areaCuadrado } from './cuadrado.js';
import { areaTriangulo } from './triangulo.js';

console.log(areaCirculo(5));
console.log(areaCuadrado(4));
console.log(areaTriangulo(6, 3));


2. **Crear un sistema de autenticación básico con módulos**  
   **Descripción:**  
   Diseña un programa que permita registrar usuarios, verificar contraseñas y mostrar información del usuario usando módulos separados.  
   **Pasos para resolverlo:**  
   1. Crea un archivo `registro.js` que contenga una función para registrar usuarios.  
   2. Crea un archivo `login.js` que contenga una función para verificar contraseñas.  
   3. Usa un array o un objeto en `registro.js` para almacenar los usuarios registrados.  
   4. Exporta las funciones de registro y login desde sus respectivos archivos.  
   5. En un archivo principal, importa las funciones y simula el flujo de registro e inicio de sesión.

---

`registro.js`
let usuarios = [];

export function registrarUsuario(nombre, contrasena) {
  usuarios.push({ nombre, contrasena });
  console.log("Usuario registrado exitosamente");
}

export function obtenerUsuarios() {
  return usuarios;
}


`login.js`
import { obtenerUsuarios } from './registro.js';

export function verificarLogin(nombre, contrasena) {
  const usuario = obtenerUsuarios().find(u => u.nombre === nombre);
  if (usuario && usuario.contrasena === contrasena) {
    console.log("Inicio de sesión exitoso");
  } else {
    console.log("Credenciales incorrectas");
  }
}


`app.js`
import { registrarUsuario } from './registro.js';
import { verificarLogin } from './login.js';

registrarUsuario('usuario1', '1234');
verificarLogin('usuario1', '1234'); // Inicio de sesión exitoso
verificarLogin('usuario1', 'abcd'); // Credenciales incorrectas


#### **Preguntas Abiertas y Teóricas**

1. ¿Qué diferencia hay entre `export` por defecto y `export` nombrado?
En un archivo, puedes exportar una sola cosa por defecto y, al importarla, puedes llamarla como quieras. También puedes exportar múltiples elementos a la vez, pero en ese caso debes usar sus nombres exactos al importarlos.

2. ¿Cómo ayuda la modularización en equipos grandes de desarrollo?  
La modularización permite que el proyecto sea mas organizado y facil de entender, es sencillo poder encontrar 
errores y arreglarlos, esto tambien permite que pueda reutilizarse en otros proyectos. 

3. Describe cómo dividirías un proyecto complejo en módulos.
Organizaria que funcionalidades tiene mi proyecto, para asi poder organizar los modulos
logrando que cada uno, haga su respectiva funcion y si con el transcurso de desarrollar el proyect 
veo que se puede seguir modularizando, lo hare respectivamente.

4. Explica los pasos necesarios para importar funciones de varios archivos en uno solo.
crear archivos separados para cada funcion 
difinir cada funcion 
en el archivo principal, importar las funciones ya previamente hechas
llama a las funciones importadas

### **Proyecto Final: Gestor de Tareas Avanzado**

#### **Descripción del proyecto**

Crear un gestor de tareas que permita a los usuarios:

* Agregar nuevas tareas.  
* Marcar tareas como completadas.  
* Eliminar tareas.  
* Filtrar tareas por estado (completadas o pendientes).  
* Persistir las tareas en el almacenamiento local del navegador para que no se pierdan al recargar la página.

---

#### **Requerimientos del proyecto**

1. **HTML y CSS:**  
   * Diseñar la interfaz de usuario con una lista de tareas y botones interactivos.  
   * Hacer que el diseño sea limpio y responsivo.  
2. **JavaScript:**  
   * Manipular el DOM para mostrar las tareas en pantalla.  
   * Usar objetos para representar cada tarea (con propiedades como `id`, `descripcion`, `completada`).  
   * Implementar funciones para agregar, marcar como completadas, eliminar y filtrar tareas.  
   * Guardar y cargar tareas usando `localStorage`.  
3. **Modularización:**  
   * Separar las funciones en módulos organizados (por ejemplo: un módulo para manejar las tareas y otro para la interfaz).

---

#### **Pasos para implementar el proyecto**

**1\. Diseñar la estructura HTML básica**

* Crea un archivo `index.html`.  
* Incluye los siguientes elementos:  
  * Un campo de texto y un botón para agregar tareas.  
  * Una lista (`<ul>`) donde se mostrarán las tareas.  
  * Botones para filtrar las tareas (por ejemplo, "Todas", "Completadas", "Pendientes").

**Pistas:**

* Usa etiquetas como `<input>`, `<button>`, y `<ul>` para crear la estructura.  
* Asegúrate de asignar identificadores (`id`) o clases (`class`) para facilitar la manipulación con CSS y JavaScript.

---

**2\. Estilizar con CSS**

* Crea un archivo `styles.css`.  
* Diseña un layout limpio, centrando los elementos.  
* Aplica estilos diferenciados a las tareas completadas (por ejemplo, tacharlas con `text-decoration: line-through`).

**Pistas:**

* Usa Flexbox para alinear los elementos.  
* Aplica pseudoclases como `:hover` para botones interactivos.

---

**3\. Estructurar las funciones de JavaScript**

* Crea un archivo `app.js`.

Define un array para almacenar las tareas, con el siguiente formato:  
javascript  
Copiar código  
`let tareas = [`  
    `{ id: 1, descripcion: "Estudiar JavaScript", completada: false },`  
    `{ id: 2, descripcion: "Leer un libro", completada: true },`  
`];`

*   
* Implementa las siguientes funciones:  
  * `agregarTarea(descripcion)`: Crea una nueva tarea con un `id` único.  
  * `mostrarTareas()`: Recorre el array y muestra las tareas en la lista `<ul>`.  
  * `marcarCompletada(id)`: Cambia el estado de una tarea a `completada`.  
  * `eliminarTarea(id)`: Elimina una tarea del array.  
  * `filtrarTareas(filtro)`: Muestra solo las tareas que cumplen el filtro ("completadas", "pendientes", "todas").

**Pistas:**

* Usa `document.createElement` para generar dinámicamente los elementos de la lista.  
* Añade eventos como `click` o `change` a los botones.

---

**4\. Conectar la interfaz con las funciones**

* Escucha los eventos del formulario para agregar tareas.  
* Usa `addEventListener` en los botones de filtrado para aplicar el filtro seleccionado.  
* Añade un evento `click` a cada tarea para marcarla como completada o eliminarla.

**Pistas:**



* Usa atributos personalizados (`data-id`) para asociar elementos HTML con el `id` de la tarea.  
* Manipula clases de CSS para cambiar la apariencia de las tareas completadas.

---

**5\. Persistir datos con `localStorage`**

* Al agregar, eliminar o actualizar una tarea, guarda el array en `localStorage`.  
* Carga las tareas desde `localStorage` al iniciar la página.

**Pistas:**

* Usa `JSON.stringify` para guardar el array en formato JSON.  
* Usa `JSON.parse` para recuperar los datos.

---

#### **Conceptos que practicarás**

* **HTML y CSS:**  
  * Crear una interfaz funcional y atractiva.  
  * Diseñar elementos interactivos y responsivos.  
* **JavaScript:**  
  * Manipulación del DOM.  
  * Uso de eventos para interactuar con el usuario.  
  * Gestión de datos dinámicos con arrays y objetos.  
* **Modularización:**  
  * Separar la lógica de manipulación de datos y la interfaz.  
* **`localStorage`:**  
  * Guardar y recuperar datos para mantener el estado del gestor.

---

#### **Preguntas Abiertas para Reflexionar**

1. ¿Qué ventajas tiene usar `localStorage` frente a guardar los datos solo en memoria?  
- Persistencia de datos entre sesiones, accesibilidad sin conexión, y facilidad de uso frente a almacenar datos solo en memoria.
2. ¿Cómo podrías mejorar la interfaz para hacerla más intuitiva?  
- Simplificar navegación, consistencia en diseño, retroalimentación clara, y asegurar que sea accesible y responsiva.
3. ¿Qué estrategia usarías para depurar errores si el gestor de tareas no funciona como esperas?  
- Usar console.log(), depuradores, pruebas unitarias y revisar el flujo de eventos y lógica de negocio.
4. ¿Cómo organizarías los módulos para mantener el proyecto escalable?
- Modularizar por funcionalidades, seguir el principio de responsabilidad única, usar patrones de diseño, y separar la lógica de negocio de la presentación.

