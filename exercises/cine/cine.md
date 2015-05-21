##Propuesta de trabajo
Se desea informatizar la gestión de un cine.
 
**El funcionamiento del supuesto cine es el siguiente:**

Al cine le **llegan una serie de películas a través de sus proveedores** para proyectar en las diferentes salas que posee. Estas películas son de estreno a poner en cartelera. De cada 
película se requieren los siguientes datos:

- titulo,
- año,
- genero,
- director,
- nacionalidad,
- productora 
- el elenco de actores que intervienen en ella.

 Cuando la película llega, se:

- da de alta en el sistema, 
- se pone en cartelera 
- se le asigna sala y sesiones. 

Cada película se proyecta en una sala durante tres sesiones diferentes al día (17:00 h, 19:30 h, 22:45 h). El cine dispone de cuatro salas. Puede darse el caso de que se requieran varias unidades de una misma película, que por su gran tirada se tenga que proyectar en varias salas y en varias sesiones diferentes. Cuando sea este el caso, cuando llega la película, el sistema comprobará si ya está dada de alta con anterioridad, si es así se incrementará el número de unidades de la película. **Los datos de la película podrán ser modificados** con posterioridad a su alta en el caso de que se hayan introducido con algún error. En este caso el sistema buscará la película deseada y mostrará todos sus datos para que puedan ser modificados. Cuando se desee **retirar la película de la cartelera** del cine, los datos de ésta se mandarán a un historial de películas de cartelera, causando baja de las películas que están en cartelera.

En el sistema, de manera diaria, se realizan las **asignaciones de las proyecciones** de las películas, de tal forma que a una película se le asigna sala/s y sesión/es. Para ello, el sistema debe mostrar un listado de todas las películas que están en cartelera junto con las salas y sesiones disponibles, se realiza la asignación y se muestra la cartelera del día en los paneles habilitados al efecto para que el usuario pueda hacer uso de esta información. Una vez hechas las asignaciones, éstas pueden ser modificadas o anuladas en aras de poder realizar asignaciones nuevas.

Cuando una persona llega a la ventanilla del cine para **sacar su entrada**, le dice el número de entradas que quiere, la película que va a ver, (o la sala de la película) y la sesión a la que desea ver la película. La venta de entradas, únicamente se realizará por ventanilla, no teniendo en cuenta la reserva de entradas (ya sea por teléfono, por Internet,o en propia ventanilla con días de antelación). En función de estos datos, se comprueban si quedan asientos libres, es decir, si queda aforo en la sala para esa sesión proporcionando información al usuario de si es así o no.

En el caso de que no queden asientos, se informa al usuario y éste si le interesa, indicará de nuevo los datos necesarios para sacar entradas para otra película u otra sesión diferente. En el caso de que queden asientos libres, es decir, que no se haya completado el aforo de la sala, se **imprime la entrada** con el título, sala, sesión, precio y con los asientos sin numerar. Respecto al **precio de la entrada, éste puede variar** sabiendo que dependiendo del día (día del espectador, otro día de la semana), el coste de la entrada es diferente (6,00 euros, 8,50 euros respectivamente). Esto implica que el sistema debe tener posibilidad de dar **de alta las tasas** y también modificarlas para incrementar o decrementar los precios de las entradas.