# ejercicios-basicos-js
Ejercicios básicos de Java Script perfectos para comenzar a entender el lenguaje.


# Indice:


    01. Escribe un programa de una sola línea que haga que aparezca en la pantalla un alert que diga “Hello World”.
    02. Escribe un programa de una sola línea que escriba en la pantalla un texto que diga “Hello World” (document.write).
    03. Escribe un programa de una sola línea que escriba en la pantalla el resultado de sumar 3 + 5.
    04. Escribe un programa de dos líneas que pida el nombre del usuario con un prompt y escriba un texto que diga “Hola nombreUsuario”
    05. Escribe un programa de tres líneas que pida un número, pida otro número y escriba el resultado de sumar estos dos números.
    06. Escribe un programa que pida dos números y escriba en la pantalla cual es el mayor.
    07. Escribe un programa que pida 3 números y escriba en la pantalla el mayor de los tres.
    08. Escribe un programa que pida un número y diga si es divisible por 2
    09. Escribe un programa que pida una frase y escriba cuantas veces aparece la letra a
    10. Escribe un programa que pida una frase y escriba las vocales que aparecen
    11. Escribe un programa que pida una frase y escriba cuántas de las letras que tiene son vocales
    12. Escribe un programa que pida una frase y escriba cuántas veces aparecen cada una de las vocales
    13. Escribe un programa que pida un número y nos diga si es divisible por 2, 3, 5 o 7 (sólo hay que comprobar si lo es por uno de los cuatro)
    14. Añadir al ejercicio anterior que nos diga por cual de los cuatro es divisible (hay que decir todos por los que es divisible)
    15. Escribir un programa que escriba en pantalla los divisores de un número dado
    16. Escribir un programa que escriba en pantalla los divisores comunes de dos números dados
    17. Escribir un programa que nos diga si un número dado es primo (no es divisible por ninguno otro número que no sea él mismo o la unidad)

# Ejercicio 01
Escribe un programa de una sola línea que haga que aparezca en la pantalla un alert que diga “Hello World”.
```html
    <script>
      alert( 'Hello, world!' );    
    </script>
```
# Ejercicio 02
Escribe un programa de una sola línea que escriba en la pantalla un texto que diga “Hello World” (document.write).
```html
    <script>
      document.write( 'Hello, world!' );    
    </script>
```
# Ejercicio 03
Escribe un programa de una sola línea que escriba en la pantalla el resultado de sumar 3 + 5.
```html
    <script>
      document.write( 3 + 5 );    
    </script>
```
# Ejercicio 04
Escribe un programa de dos líneas que pida el nombre del usuario con un prompt y escriba un texto que diga “Hola nombreUsuario”
```html
    <script>
      var nombre = prompt("Escribe tu nombre");
      document.write("Hola "+nombre);
    </script>
```
# Ejercicio 05
Escribe un programa de tres líneas que pida un número, pida otro número y escriba el resultado de sumar estos dos números.
```html
    <script>
      var n1 = prompt("Escribe un número");
      var n2 = prompt("Escribe otro número");
      document.write("El resultado de la suma es: "+ ( parseInt(n1)+ parseInt(n2) ) );
    </script>
```
# Ejercicio 06
Escribe un programa que pida dos números y escriba en la pantalla cual es el mayor.
```html
    <script>
      var n1 = prompt("Escribe un número");
      var n2 = prompt("Escribe otro número");
      n1 = parseInt(n1);
      n2 = parseInt(n2);
      if (n1 >= n2) {
        document.write(n1);
      } else {
        document.write(n2);
      }
    </script>
```
# Ejercicio 07
Escribe un programa que pida 3 números y escriba en la pantalla el mayor de los tres.
```html
    <script>
      var n1 = prompt("Escribe un número");
      var n2 = prompt("Escribe otro número");
      var n3 = prompt("Escribe otro número");
      n1 = parseInt(n1);
      n2 = parseInt(n2);
      n3 = parseInt(n3);
      if (n1 > n2 && n1 > n3) {
        document.write(n1);
      } else if (n2 > n3) {
        document.write(n2);
      } else {
        document.write(n3);
      }  
    </script>
```
# Ejercicio 08
Escribe un programa que pida un número y diga si es divisible por 2.
```html
    <script>
      var n1 = prompt("Escribe un número");
      if (n1 % 2 === 0) {
        document.write("Es divisible por 2");
      } else {
        document.write("No es divisible por 2");
      }
    </script>
```
# Ejercicio 09
Escribe un programa que pida una frase y escriba cuantas veces aparece la letra a.
```html
    <script>
      var text = prompt("Escribe una frase");
      var nText = text.length;
      var i;
      var cont=0;
      for (i = 0; i < nText; i++) {
        if (text.substr(i,1) === "a") {
          cont = cont + 1;
        }
      }
      document.write("La letra a aparece " + cont + " veces en la frase");
    </script>
```
# Ejercicio 10
Escribe un programa que pida una frase y escriba las vocales que aparecen.
```html
    <script>
      var text = prompt("Escribe una frase");
      var nText = text.length;
      var i;
      var lista = [];
      for (i = 0; i < nText; i++) {
        if (text.substr(i,1) === "a" || text.substr(i,1) === "e" || text.substr(i,1) === "i" || text.substr(i,1) === "o" || text.substr(i,1) === "u") {
          lista.push(text.substr(i,1));
        }
      }
      document.write("Aparecen las siguientes vocales: (" + lista + ")");
    </script>
```
# Ejercicio 11
Escribe un programa que pida una frase y escriba cuántas de las letras que tiene son vocales.
```html
<script>
  var text = prompt("Escribe una frase");
  var nText = text.length;
  var i;
  var cont=0;
  for (i = 0; i < nText; i++) {
    if (text.substr(i,1) === "a" || text.substr(i,1) === "e" || text.substr(i,1) === "i" || text.substr(i,1) === "o" || text.substr(i,1) === "u") {
      cont = cont + 1;
    }
  }
  document.write("Aparecen " + cont + " veces vocales en la frase");
</script>
```
# Ejercicio 12
Escribe un programa que pida una frase y escriba cuántas veces aparecen cada una de las vocales.
```html
    <script>
      var text = prompt("Escribe una frase");
      var nText = text.length;
      var cont;
      var a=0,e=0,i=0,o=0,u=0;
      for (cont = 0; cont < nText; cont++) {
        if (text.substr(cont,1) === "a"){a++;};  
        if (text.substr(cont,1) === "e"){e++;}; 
        if (text.substr(cont,1) === "i"){i++;}; 
        if (text.substr(cont,1) === "o"){o++;};
        if (text.substr(cont,1) === "u"){u++;};
      }
      document.write("La letra a aparece " + a + " veces<br>");
      document.write("La letra e aparece " + e + " veces<br>");
      document.write("La letra i aparece " + i + " veces<br>");
      document.write("La letra o aparece " + o + " veces<br>");
      document.write("La letra u aparece " + u + " veces<br>");
    </script>
```
# Ejercicio 13
Escribe un programa que pida un número y nos diga si es divisible por 2, 3, 5 o 7 (sólo hay que comprobar si lo es por uno de los cuatro).
```html
    <script>
      var i = prompt("Introduce un número");
      if (i%2==0){document.write("Es divisible entre 2<br>");}
      else if (i%3==0){document.write("Es divisible entre 3<br>");}
      else if (i%5==0){document.write("Es divisible entre 5<br>");}
      else if (i%7==0){document.write("Es divisible entre 7<br>");};
    </script>
```
# Ejercicio 14
Añadir al ejercicio anterior que nos diga por cual de los cuatro es divisible (hay que decir todos por los que es divisible).
```html
    <script>
      var i = prompt("Introduce un número");
      if (i%2==0){document.write("Es divisible entre 2<br>");};
      if (i%3==0){document.write("Es divisible entre 3<br>");};
      if (i%5==0){document.write("Es divisible entre 5<br>");};
      if (i%7==0){document.write("Es divisible entre 7<br>");};
    </script>
```
# Ejercicio 15
Escribir un programa que escriba en pantalla los divisores de un número dado.
```html
    <script>
      var numero = prompt("Introduce un número");
      var divisores = [];
      for(var i = 1; i <= numero; i++){
        if(numero % i == 0){
          divisores.push(i);
        }
      }
      document.write("Los divisores de "+numero+" son: "+divisores);
    </script>
```
# Ejercicio 16
Escribir un programa que escriba en pantalla los divisores comunes de dos números dados.
```html
    <script>
      //programa que escriba en pantalla los divisores comunes de dos números dados
      var num1 = prompt("Introduce el primer número"); 
      var num2 = prompt("Introduce el segundo número");
      var divisores = [];
      for (var i = 1; i <= num1; i++) {
        if (num1 % i == 0 && num2 % i == 0) {
          divisores.push(i);
        }
      }
      document.write("Los divisores comunes de "+num1+" y "+num2+" son: "+divisores);
    </script>
```
# Ejercicio 17
Escribir un programa que nos diga si un número dado es primo (no es divisible por ninguno otro número que no sea él mismo o la unidad).
```html
    <script>
      var numero = prompt("Introduce un número");
      parseInt(numero);
      var contador = 0;
      for(var i = 1; i <= numero; i++){
        if(numero % i == 0){
          contador++;
        }
      }
      if(contador == 2){
        document.write("Es primo");
      }else{
        document.write("No es primo");
      }
    </script>
```
