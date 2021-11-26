# Prueba de tester 1

## Casos de usos
Un banco financiero implementó el juego, Adivina tu número, la cual consiste en adivinar un número entre 1 al 100 durante 10 intentos. Así mismo para facilitar dicho juego se debe cumplir los siguientes requisitos:
* El número a adivinar debe pertenecer al conjunto de los enteros (e.g. 1, 2, 3...)
* El número que ingresará el jugador debe pertenecer al conjunto de los enteros (e.g. 1, 2, 3...), en caso que no ingrese un número entero, debe mostrarse una alerta al usuario y no se debe incrementar un intento de prueba.
* Sí el número que ingresó el jugador es mayor al número a adivinar, se debe mostrar el siguiente mensaje en color negro: "Incorrecto! El número es mayor!", en caso que sea menor, se debe mostrar: "Incorrecto! El número es menor!".
* Si después de 10 intentos, el usuario no adivina el número, se debe mostrarse el mensaje de color rojo: "!!!Pérdistes!!!"
* Si el usuario adivina el número antes de los 10 intentos, se debe mostrar el mensaje de color verde: "Felicitaciones! adivinaste el número!".

# Listado de Cambios
let randomNumber = Math.random() * 10;
let randomNumber =  (Math.floor(Math.random()*100)+1);
Al momento de elegir el número random el código lo generaba de manera erronea, se corrigió la función para que pudiera generar el número entre el rango de 1 a 100 como lo solicitaba las reglas del negocio

const lowOrHi = document.querySelector('.lowOrHi');//no esta declarado la clase de la etiqueta 

 let userGuess = guessField.value.trim();//se recomienda trimiar los campos para quitar los espacions en blanco en el sting

## Se utilizo try catch para manejar fragmentos de código que son propensos a fallar
* Se agregaron las validaciones para solicitar el ingreso de números
* el rango valido 1 a 100 
* que no se permite el ingreso de campo vacío

* No realizaba de manera correcta las validaciones
* En las distintas validaciones se estaban mostrando los mensajes con el color equivocado

  guessSubmit.addEventListener('click', checkGuess);//el método no se llamó correctamente
  resetButton.addEventListener('click', resetGame);// em método no está declarado correctamente
*