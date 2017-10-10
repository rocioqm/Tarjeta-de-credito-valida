
# TARJETA DE CRÉDITO VÁLIDA

## PSEUDOCODIGO

Creamos una función en la cuál podamos validar el número de una tarjeta de crédito.

Definimos primero la función con el nombre  isValidCard

function isValidCard(array) {

Iniciamos con un prompt para que el usuario ingrese su número de tarjeta.
  
  var cardNumber = parseInt(prompt('Ingrese su número de Tarjeta \n Nota: Debe contener 16 números y sin espacios.'));

con el sgte for buscamos algún espacio en el número de tarjeta

  for (i = 0; i.length < 16; i++) {

Creamos una condición en la cúal si hay no hay un espacio revertimos el orden del array, sino que nos regrese al prompt inicial.

    if (cardNumber(i) !== " ") {

      var cardNumber1 = cardNumber.slice(i, 0, cardNumber.pop())

    }

    else {

      return cardNumber;

    }
  }
una vez obtenido la invrsa del array inicial, multiplicamos por dos los números que se encuentren en la posición par,

pero como empiezo a contar desde el 0 y lo condiciono a que es mayor que cero, trabajaré con la posición impar.

   for (j = 0; 0 < j < cardNumber1.length; j + 2)

   var  cardNumber2=((j + 2) * 2);

una vez multiplicado, procedo a sumar los elementos de la variable cardNumber2
  var sum;

Se suman los numeros del do mientras se cumpla lo establecido en el while.
  do (sum = cardNumber1.slice(i) + cardNumber1.slice(i++));

  while (0 <= i < 16);

A la variable sum se le saca el modulo con 10 y se le introduce este resultado en una nueva variable llamada rest

  var rest = sum % 10;

Para saber si una tarjeta de crédito es válida, el módulo debe ser cero, es por eso que creamos un if
  
  if (rest = 0) {
   
si el residuo es cero, emitiremos un prompt con el mensaje "tarjeta de crédito válida"
    
    prompt('tarjeta de credito valida')
 
  }
 
sino devolveremos un prompt con el sgte mensaje.
 
  else {
   
    return prompt('numero de tarjeta incorrecto')
 
  }
 
  return(isValidCard)

};


## DIAGRAMA DE FLUJO

![Diagrama de Flujo](https://www.draw.io/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1&title=tarjeta%20de%20credito.html#R3VxZb%2BM2EP4tfTDWKdBA1Gk%2F5vBuU%2BymwWaLto%2ByxNgKZFGl5STeX1%2FSOnnIphxRiQMsFtKIoqhvht8cGmdkXa1evmA%2FXX5DIYxHphG%2BjKzrkWlOPJP8TwXbXGA7Xi5Y4CjMRaAW3Ec%2FYSE0CukmCuGaGZghFGdRygoDlCQwyBiZjzF6Zoc9oJh9auovoCC4D%2FxYlP4dhdmyeC3Tq%2BW%2Fw2ixLJ8M3Gl%2BZeWXg4s3WS%2F9ED03RNZsZF1hhLL8aPVyBWOKXYlLft%2FnlqvVwjBMMpUb7IfQD8CcrN2AoenNfytmePLjTfGyN7c3Vzd%2FFsvNtiUGGG2SENJpjJF1%2BbyMMnif%2BgG9%2BkyUTmTLbBWTM0AOi0khzuBL60pB9f7EbiBawQxvyZDiBssuINuytvBcKwCUqC4b4LuFzC90vqhmrmEhBwUyiihZAkoj0%2F1vQ7V2eXP75fvsfkYu3%2F71bfadIGdc07MfF9%2F%2FmP24qAe%2BP0hVMbV1YGpLMOUAgiHZhsUpwtkSLVDix7NaeslC2IDrEWbZtmASf5MhIqpn%2BIpQysBKH7QfVLIutMEB3L%2BNMh8vYLbPiETlYBj7WfTEPr9XpN2PhPRrUSxuvUMReWq1NWyD2xoTzuRzzRZ3cbqolnGceqYycvFXdP8n83W6g86NKYOsUz8hxwt6%2FIBwKSZPbF6RjSbzjzsMj7pMTZesPNroNDNdt6Zln3cYG8NkQQiyC9yFAuPmCIUbgfte8BmZ%2BT%2FlG85ax3JcQ2KglB4u4YtPSIIMSSGOyA6CuJbelSJzGNdotuz%2Fpmt0Ja7R0eEaS7%2FMUsIO3DB62qvhh1Yt1ATQlAc%2BDm83qzlsYxPpXW2GRGzA%2BIUuuOYEzmyqWMhonrRNVsmZ124No8AwtgIcxlaqkLNpK95QYRQwP5J3nw7i3YUkQaN3Bx8q%2BgLGIAqyrAEV5B1W0NCZGvErLB7leYNiLGeo7BdMBISefEzrLZXzAJTQ6ZWG7HwdRwEcE19BHkkVfMVeTlE6PjsTsCaoZRoAnbKA2iJnSwHlDbEXQE3Rv6%2BjPR5%2BjnnJAZcoYojhOvrpz3cDqA2ndCvt3sm5HDnEYV9S9ljnREJv8ONoQWKz6xg%2B0Kko%2BlHgxxeFOKPMQp17ECWLHzuaIRl9L7qyDZvVVXne0JWsSqFHVbLSD0%2FfSXhBq4zkLEEJlBnvYeIV4Wi8rswyS9lrqXfCRTN85pv7A4F6hYkcrrokTKSRw02VYtI%2BLRFd4O0%2FzZN%2F6UY5J7zbxXceU%2F8ZRs0HtaOqZnvKTWSoqZlg728bwwoCUl4w4CvbB9bFjScH%2BQr6szlHsLkEfTAm5nUtyYotic2aWphYIU47oUDakyPfcyBt86rQScJimKhSyOxQYtJa83w8zZpnp8mPLUt2wubYhzDZxDup43bVRjeguqBjto49gfKq6bXQUjOkH6y8asq%2BuJysJ8lpV7sncRTjvD48SRlTvKuSzITDQ%2FLxXGrCehoSxL6NvCTDlFjI61yPx487MSUyk9bnf80PlKoGfeA2VcANSHDTks5bZgtu683q7SCxxOqe7PuBHkRUChwnQ4aWpvo0YDXmAjUy7Jr0Cs8xDiS9%2B8f3n%2FRa0hi%2FpUjZlLw1e5stCmxsOVtWVPR07Dlb9G8houkKZSGxkA7KSvpZxeSSi%2FkH%2B7OzMmY1CKoEbjKr0Yxhd3NHTFRrAHdAf8BrQvJpw7aHYj9b9KMnApstwibt3dMD2%2FtwGvAlymjR1ji3Pbs4p3VbcG6A8vyukfwYPTqaggj3VnxtW4834mzBU%2FxaenAiR7Eo3Nmt8cY7AXrdlK3wPWDw7luX05pq962WHNgWq9d5IIzhOqt8UOGPKEUbwBiM7ASoJOUCaYeNHrL7UIXnoThpqsZJvex2WVDautuHaRLjywUVHs20V2bCWsoFJYW8Z4Qmqgjp4UOxJkh7KY0xw4fGQO0qFo%2BNIWIzGYr%2FHDFGPmX%2BUwncnNeWEY4H2xTATjFapdn4E1kxwconF0OanwQYhlGG8rFR6H8ayjY5pp9KbLNqCtBvnK%2Ftz%2Bml8%2BOtujo8rv4z4etSyl0d3AcaoJhSdM0E%2BAWXz2ltKuJ%2Fl8OO7z9zcPR0ElUnx6ej%2BwmrpZ1goOYihzdD5zgzFO2Zm0hjFOmIjdq0KfMgpZ5SPw%2F3y4WJCyTULZqJln4eR0yrPlr%2FlOOxXcfeVNLGPRjeClnS6YRxr47Q2j6osDtkOmATq6PQljB00co1WAueAAljlDLtaWw5qSQ4TjYriFEZG9ehcpQECGMYZGio%2BFiAzJLEx7JdryU%2BdsXk7fPNbZ%2B%2FNSj7jUIUEB1QjA7Z5Tw34q%2FzPrMSLgSZyn7AKfNt%2FAZXQJ2c1n%2BxI9%2F59Z89sWb%2FAw%3D%3D "diagrama")
