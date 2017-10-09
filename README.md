
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

![Diagrama de Flujo](https://www.draw.io/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1&title=tarjeta%20de%20credito.html#R3Vxbb9s2FP4tezDqDGhA3e3HXNwuQ5sVTYdtj7TE2OpkUaPlJO6vH2ndScqmHFGNXRSFdESR0ne%2Bc%2BHRcUfWzerlI4HJ8jMOUDQyQfAysm5HpjnxTPovE2wzge14mWBBwiATGZXgIfyBciHIpZswQOvGwBTjKA2TptDHcYz8tCGDhODn5rBHHDVXTeACCYIHH0ai9K8wSJf5a5leJf8NhYtlsbLhTrMrc%2Bj%2FuyB4E%2BfrjUzrcfcnu7yCxVz5i66XMMDPNZE1G1k3BOM0O1q93KCIQVvAlt33oeVq%2BdwExanKDfZjAH1jTl8NoMD05u%2FtbIYnGG1Q8Qq7B023BTgooFjlp5ikS7zAMYxmlfR6BwBiSwB6tkxXET006OF3lKbbXN1wk2Iqqmb4hHGSj8vWZAu1vlcuWuMN8VHLyxTUgWSB0pYxVok6JTPCK5SSLb2HoAim4VNzfZjTalGOq6ClBzm6ikgbAtJ393c3d38IeDfRfF6GKXpI4O6ln6n1NRHOJ0UkRS%2F7sRPfOb%2FBsnNybptG%2BVxZglHwd1mzAhdoQMk9Jz6%2Blmv5rV9wSFct9WUDTl8TThEZ%2F%2FO7OF2Uj3GceiyJetz%2FNsx9Xd%2Fdf%2Fw6e5jRy%2Fd%2Ffp59pcQGt%2Bzs29XX32ffrqqBb4%2FxqpS3dVDeMM%2BJ89NBOC84H42cn8o4D1eMlvF8neygcyNG7HUCY3q8YMePmBRiumL9imw0nX%2FcYXjYZWr2yMqjQaeZ2XNreuzLDmMjFC%2Bo3XaBO1dgVB%2BhcKPhvhV8Rmb2V%2FmGi9axnK%2BhOWrCDpfoBVInQYckiITUghCppF8KkTmMxzZbYl7dY7sSj%2B1o8dhnlaUYQA59zy7bsoZz2UU8b%2FrsHfuD8GmvCT62mknloetyH5LgfrOaozZ3L72rzdKpkYJf2ANXTpuz6zKHAvWTtslKeeO1W9MvYxhjNhx5MK8bszdU%2BlVs8s%2FEmL1BjNk2BzRmBQUNvYOggaXp3IrzGoUtZ6hNszEREHqChNXLSudkMIfBrtRkl%2Bso9NGY%2BiK6JFPwTfNygpPxxYWANUUt1QDotAmoLfoEKaB8VOnHJ4jxYx3uiSBzwksOuFwRQ4LW4Q843w1gHE6YKe3eybkeOTQgXDPvsc4cCbsBRuGCJme3EXpkUzH0Qx9GV7k4ZZ6FBQ8%2FjBffdm7mvd2PrmxgN3VVnNd0Jds961GVrCTBu%2B84uGJVYnoW4xjJyHvY8Ypw1F5XxsxC9lrXO%2BGiJV%2FuyeKB4HqFiRyu6iFMpNGHmyp15n1aorog27%2FrJ%2F8wQ7mkfrdL7DymNDyMmg9qR1XN9pSbCKipmWIPt7VhuQNSfmCD%2F%2FRw4Lm48fQge4L%2BOOcInIvxmXliXteSbbEl4SyfvfXjiWWFspNNpM2JHPmeE2lH0Tp7MQgxTVSpZHaoMWkten4%2FzaJnp8mPrUt2wubYRRq7iTdSyO2qjW5AdUHHbB17AvVV02u6pXJ%2FX0%2FpB6uvWio5%2FclEEktTfdVoqsw19OR5wjrgQJ63f3z%2FeV6R4Lyp%2BtCEC%2FOSL8xSe9JSH7LE3pOsPtSo99DXuR2Pv%2B%2FEzKuarBj9a3agVMLoA7epAm6GBDcttQXLbMFtvVn9PEgssdQoK5brQUSaQrbUwOqSn22PZouzrIFoy2pWng4UbdFjBZhlw4xXYp3WKAq1F6VtSi5mH4QvLoqUCFBUKdx0VlBPkXZzh42kCRjugBbOa0JSObftofhsi57xRGCzRdikLUt6YHsbCRp6CVNWEwSXtmfn56wsaFwCozj%2FUsutQY9JXe4I9xYUbVuu09dmfhwXPMUv6wcnchRrjp1TSJ68E4OjX88poX1W33SHotFUjUa9KEjhe8DgXaEuh4dqV6iWPbAtVq%2Bz3JOgdVomCXnCwGIoMMBg0UiASlIukHZwaIlGjhjET9naVSKL89qawvG8lO0AWi13mIYifrdderL6rlFGRy27bUcBodOh46uZ1lYlan7Vng74Mbrw12%2BZwhNVCusJPuKnPNYYCcaN4AMG6g2yeGyAiM1ksGBjCtAkBK%2BSdPyOUpYaJ6QXA7aB9AkKwhRnY8MAvhsKLi6vm0rgKpsC9OP12v6cXjo%2FflZXh8cVwyd8kV65q4P7QGMo7vm6btX4By7WaW0q4n%2BM1hzf%2F9bO0dNJVJ4cXy%2FYn7C19OUO1Fzk8DR0jqOhyGduIp1hW%2FzVBWvKPOhST6mfh8uKJq4hcd0iTbT08zhiEeXc%2Bqccr9l17E0lbdyD4a3QPzV0TcQFTYAmhoSQhUz%2Fj8PFxL3IveLNChFcpF5VJhbGPiYE%2BSkeKv0SILMk6ZeMVFrSL1esjXy4u%2B%2Bzlb1oZwmwT3XAMDrEy3lG4k%2FzPpNeLsJNZT8QlLlOft%2BpgDo9rf7HjiyyVf8rijX7Hw%3D%3D "diagrama")
