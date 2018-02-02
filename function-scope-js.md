## Funciones globales
- Estas funciónes son definidas en el ámbito global
```
$(document).ready(function() 
```
## Funciones  Locales

- Estas funciónes son definidas en el ámbito local(dentro de otra función)

```
function activeButton() {
        ...
} 
```
```
function desactiveButton() {  
        ...
  } 
```
```
function longitud(input) {
        ...
    }
  }
```
```
function isValidCreditCard(numberCard) {
        ...
  }
 
```
## Funciones Statement

```
function soloNumeros(input) {
        ....
  }
 ```
 ```
function activeButton() {
        ...
} 
```
```
function desactiveButton() {  
        ...
  } 
```
```
function longitud(input) {
     ....
    }
  }
```
```
function isValidCreditCard(numberCard) {
    ...
  }
 
```
## Funciones de callback
- llama a una funcion y le envía por parámetro otra función (un callback)

```
// Funcion que valida que sea una un numero de tarjeta valido   
  function isValidCreditCard(numberCard) {
    var creditCardNumber = soloNumeros(longitud(numberCard));
  }
```
```
$(document).ready(function() {})
```

## Funciones clousures y Local Scope
- Los closures son funciones que manejan variables independientes. E
```
 function soloNumeros(input) {
    var regex = /^[0-9]+$/;
    if (regex.test(input)) {
      return input;
    }
  }
```
```

  function isValidCreditCard(numberCard) {
    var creditCardNumber = soloNumeros(longitud(numberCard));
    if (creditCardNumber !== undefined) {
      var arr = [];
      var sumaTotal = 0;
      for (var index = creditCardNumber.length - 1; index >= 0; index--) {
        arr.push(creditCardNumber[index]);
      }
      for (var index = 1; index < arr.length; index = index + 2) {
        arr[index] = arr[index] * 2;
        if (arr[index] >= 10) {
          arr[index] = arr[index] - 9;
        }    
      }
     
  }
  }
  ```
## Funciones de stack execution (pila de llamadas)
```
$(document).ready(function() {
```

## Funciones que forman parte de la cola de Eventos (event queue)
```
$inputCard.on('input', function() {
    isValidCreditCard($(this).val().trim());
  });
```

```
function activeButton() {
        ...
} 
```
```
function desactiveButton() {  
        ...
  } 
```
```
function longitud(input) {
        ...
    }
  }
```
```
function isValidCreditCard(numberCard) {
        ...
  }
 
```
