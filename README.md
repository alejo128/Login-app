# Login App
1. para iniciar el proyecto hay que correr 2 comandos
   - npm install 
   - npm start o si se tiene ya instalado el angular cli se puede abrir con el comando ng serve --open
   esto descargara todas las librerias usadas en el proyecto y lo abrira de manera local para correrlo en el navegador por defecto
2. al usar angular se aprovecho para dividir los componentes por carpetas
   - _components donde estan las alertas
   - _helpers para el manejo de los guards, un fakebackend y el interceptor 
   - _models es donde se creo el modelo que se iba a usar para las alertas y para el user 
   - _services se tiene un servicio para el account que es donde se llaman todas las funciones pertenecientes al account y lo mismo para las alertas
   - account es donde esta creado el componente principal de login y de register
   - home es el componente que muestra una pagina despues de logearse en el sistema
   - users este componente es el que permite la modificacion de los usuarios registrados, ya sea eliminacion, creacion o modificacion de los ya existentes
3. para mostrar siempre los iconos en orden aleatorio pienso que puede ser implementado por medio de una funcion que genere numeros aleatorios del 1 al 10, y de acuerdo a eso organizar los iconos en base al id que vaya saliendo, si se tiene un for que genere los numeros de manera aleatoria, teniendo en cuenta un array y sacar del array el numero que salga de la funcion aleatoria, creo que por medio de eso se puede lograr que se presenten de manera aleatoria.
4. para la validacion del nombre de usuario se hizo por medio de tokens y con el uso de reactive forms, de esta manera se pudo implementar de forma que el sistema sepa cuando ya existe ese usuario y emite un mensaje de error diciendo que ya esta creado ese usuario
5. para esta aplicacion se logro que al presionar cualquiera de las imagenes, esta detecte que fue clickeada y esta registra el numero que tiene asignado en el form de password, pero tiene un pequeño detalle que no se logro solucionar, y es que cuando se hace de esta forma tiene que ingresarse cualquier caracter de manera manual y este ser eliminado, para que el sistema detecte que se esta usando el form de password
6. se tiene un metodo implementado que permite validar una clave de 3 iconos cualquiera, asociada al usuario que se puso al registrarse, en este caso se puede probar usando el user juan y la contraseña Gato, perro, conejo. el sistema deberia ingresar satisfactoriamente, sino revisar si el usuario esta creado y intentarlo nuevamente

# Nota: tener en cuenta lo anteriormente mencionado en el punto 5, por temas de usabilidad con reactive forms, el sistema debe detectar que se use el campo de password, simplemente ingresar cualquier caracter desde el teclado y eliminarlo, ya despues si se puede usar los iconos para ingresar la clave elegida, tener en cuenta que el sistema solo acepta claves de 3 iconos siempre no de menos o de mas solo de 3.

# por 
# José Alejandro Diaz Urrego
