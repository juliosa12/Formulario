## Formulario

**Formulario de Registro de Trabajador**

Creamos la estructura básica de html mas script source para tailwind, configurando los estilos a media que se va programando. En el formulario en si creamos las clases para cada datos que vamos a poner, select para los sexos y el boton para registrar.

**<input class="border rounded-md" type="text" id="nombre" placeholder="Nombre" >
<input class="border rounded-md" type="text" id="apellido" placeholder="Apellido">    
<input class="border rounded-md" type="date" id="fechaNacimiento" placeholder="Fecha de Nacimiento">
<input class="border rounded-md" type="number" id="telefono" placeholder="Telefono">
<input class="border rounded-md" type="email" id="correo" placeholder="Correo">
<input class="border rounded-md" type="text" id="direccion" placeholder="Direccion">
<input class="border rounded-md" type="number" id="sueldo" placeholder="Su Sueldo">**

Ponemos los nombres en la tabla y vamos a acomodar los datos donde corresponda.

Vamos a proceder a llamar a esas clases con su id, y poner los valores donde correspondan, para que nos salga el valor que pone el trabajador en la casilla correspondiente.

Pero queremos que las listas se mantengan, para eso necesitamos meter nuestros datos en un array.

trabajadores.forEach(trabajador =>{

                let tablerow = 
                `<tr>
                    <th>${trabajador.nombre}</th>
                    <th>${trabajador.apellido}</th>
                    <th>${trabajador.edad}</th>
                    <th>${trabajador.telefono}</th>
                    <th>${trabajador.correo}</th>
                    <th>${trabajador.direccion}</th>
                    <th>$${trabajador.sueldo}</th>
                    <th>${trabajador.genero}</th>
                </tr>`** 

Lo guardamos en un local storage para que al recargar la página se mantengan los datos que ya hayamos metido.

