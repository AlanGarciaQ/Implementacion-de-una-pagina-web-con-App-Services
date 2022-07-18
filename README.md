# Implementación de una página web con App Services
**Objetivo:** Implementar una pagina web con el recurso de app Services de Azure.

![](/imagenes/app%20services.png)

**Requisitos**
- Cuenta de Azure con una suscripción activa
- Equipo de cómputo con sistema operativo: Windows, Linux o MacOs
- Repositorio con código de una página web en GitHub. [Repositorio utilizado](https://github.com/AlanGarciaQ/Pagina-web) 
 

**Pasos**  
Se inicia sesión en Portal.Azure.com.  
En la barra de búsqueda escribimos “App Services” y lo seleccionamos.  
Damos clic en el apartado crear.  
En la pestaña datos básicos, llenamos lo siguiente:  
**En Detalles del proyecto**  
Suscripción: La suscripción que queramos utilizar.  
Grupo de recursos: Podemos crear uno o seleccionar uno ya existente.
![Imagen 1](/imagenes/Imagen1.png)

**En Detalles de Instancia**  
Nombre: Pondremos el que queramos.    
Publicar: Dejamos el que está por defecto.  
Pila del entorno en tiempo de ejecución: seleccionaremos PHP 8.0.  
Sistema Operativo: Escogeremos Linux.  
Región: Podemos escoger cualquiera, pero si no queremos que haya mucha latencia escogemos uno cercano a donde vivimos.
![](/imagenes/Imagen2.png)

**En Plan de App Service**  
Plan de Linux: Dejamos el que está por defecto.  
SKU y Tamaño: Damos clic en el botón cambiar el tamaño y dentro de ahí seleccionamos el plan de tarifa F1, este lo seleccionamos para que no nos cobre por hora, ya que este plan te da 60 minutos gratis al día. 

Todo lo demás lo dejamos como esta, por último, damos clic en el botón de revisar y crear, y luego en crear.
![](/imagenes/Imagen3.png)

Cuando se termine de crear nuestro recurso, daremos clic en el botón de ir al recurso. 
En el menú de la parte de la izquierda le damos clic en la opción de centro de implementación.
En el apartado de origen seleccionaremos la opción de GitHub, y daremos clic en el botón de autorizar. Se nos pedirá que iniciemos sesión en GitHub.  
A continuación, llenamos los datos que nos piden:  
Organización: Ponemos el nombre de nuestro usuario en GitHub.  
Repositorio: El nombre del repositorio en el que esta nuestra página web.  
Rama: Seleccionamos Main.

Por último, le damos en Guardar. 
![](/imagenes/Imagen4.png)

Nos iremos a GitHub, donde se encuentra el repositorio con la página web, y nos vamos a la pestaña de Actions donde esperaremos a que se implemente la página. Cuando se implemente le daremos clic al lado de donde está el símbolo de la palomita verde.
![](/imagenes/Imagen5.png)

Daremos clic en el enlace que esta debajo de deploy para ver nuestra página web implementada. Para terminar aquí se nos muestra nuestra página web totalmente implementada.
![](/imagenes/Imagen6.png)
