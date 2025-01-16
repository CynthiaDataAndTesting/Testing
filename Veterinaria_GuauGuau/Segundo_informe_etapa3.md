<div align =  center>
<h1>INFORME EJECUTIVO DE TESTING</h1>
  <img src = "logo.png" alt = "logo">
  <br>
  <br>
  <p>
    Almirón, Sheila <br>
    Etchart, Emily <br>
    Grassi, Analía <br>
    Peruza, Lucía <br>
    Rodriguez, Cynthia
  <br>
  <br>
  Testers <br>
  Jóvenes a Programar <br>
  9 de Noviembre de 2024
  </p>
</div>

<br>

<div id = "indice">
  <h2>ÍNDICE</h2>
  <ol>
    <li>Introducción</li>
    <li>Alcance</li>
    <li>Desarrollo y resultados claves
    <br>
    <ol>
        <li>Autenticación de usuario</li>
        <li>Registro de nuevo Cliente</li>
        <li>Registro de Mascotas
        <br>
        <ol>
            <li>Versión Web</li>
            <li>Versión Mobile</li>
          </ol></li>
        <li>Registro de Vacunas</li>
        <li>Base de Datos</li>
        <li>Accesibilidad</li>
        <li>Compatibilidad y Usabilidad</li>
      </ol></li>
    <li>Datos y métricas</li>
    <li>Recomendaciones</li>
    <li>Conclusiones</li>
  </ol>
</div>

<br>

<div id = "introduccion">
  <h2>INTRODUCCIÓN</h2>
  <br>
  <p>
    Este trabajo presenta los resultados del proceso de testing de las funcionalidades “Autenticación de Usuario”, “Registro de Nuevo Cliente”, “Registro de Mascota”, “Registro de Vacunas” y “Dashboard” de la web de la Veterinaria Guau Guau durante el período de prueba que abarca del 28/10/2024 al 10/11/2024. Además, se evaluó la integridad de la base de datos. El objetivo del testing fue evaluar la validación de datos, las formas de normalización, la accesiblidad, la compatibilidad y la usabilidad de la herramienta.
  </p>
</div>

<br>

<div id = "alcance">
  <h2>ALCANCE</h2>
  <br>
  <p>
    El proceso de testing abarcó una amplia variedad de enfoques y técnicas incluyendo:
    <br>
    <br>
    <strong>Pruebas de validación de datos:</strong> Se realizaron distintas pruebas que verifican que los datos ingresados cumplen con los requisitos especificados (como formato de correos electrónicos, contraseñas, etc).
    <br>
    <br>
    <strong>Técnicas de valores límites:</strong> Se probaron los valores límites para cada campo en los distintos formularios.
    <br>
    <br>
    <strong>Pruebas de enfoque negativo:</strong> Se sometió a las funcionalidades a escenarios de prueba negativos, ingresando registros con datos incorrectos para evaluar la resistencia a errores de usuario. 
    <br>
    <br>
    <strong>Pruebas de enfoque positivo:</strong> Se realizaron pruebas para verificar que los distintos formularios funcionaran correctamente bajo condiciones normales, validando que los usuarios pudieran realizar acciones sin problemas.
   <br>
    <br>
   <strong>Pruebas de Compatibilidad:</strong> Se realizaron pruebas en dispositivos diferentes para verificar que la sección funcione tanto en PC como en Teléfono móvil. Además, se aplicaron pruebas en diferentes navegadores.
   <br>
    <br>
 <strong>Pruebas de Accesibilidad:</strong> Se aplicaron distintas pruebas que verifican el cumplimiento de las normas WCAG que definen la accesibilidad de un sitio web. Fueron tomados en cuenta los cuatro principios: Perceptible, Operable, Adaptable y Robusto.
  <br>
    <br>
    <strong>Pruebas de Usabilidad:</strong> Se exploraron las distintas secciones desde el punto de vista del usuario tomando como base la norma ISO 25010.
    <br>
    <br>
   <strong> Pruebas exploratorias:</strong> Se exploraron las distintas secciones para identificar posibles problemas y escenarios no documentados. Esto ayudó a descubrir áreas de mejora y a abordar situaciones inesperadas.
    <br>
    <br>
  <strong>  Pruebas de confirmación:</strong> Se hizo trabajo de retesting para verificar que las incidencias reportadas fueron efectivamente solucionadas.
    <br>
    <br>
  <strong>  Pruebas de Regresión:</strong> Se realizaron pruebas de regresión para verificar que las soluciones aplicadas por el equipo de desarrollo no hayan provocado nuevas incidencias.
    <br>
    <br>
    En el presente trabajo no se incluyen pruebas exhaustivas en los requerimientos no funcionales como rendimiento, mantenimiento o escalabilidad ya que el sistema no se encuentra alojado en un servidor.
  </p>
</div>

<br>

<div idd = "desarrollo">
  <h2>DESARROLLO Y RESULTADOS CLAVES</h2>
  <br>
  <h3>Autenticación de Usuario</h3>
  <p>En esta oportunidad se ejecutaron las 10 pruebas de validación de datos que en la instancia anterior estaban bloqueadas y no se pudieron ejecutar. Se utilizaron las credenciales proporcionadas por el equipo de desarrollo, alternando las pruebas para probar su accesibilidad y limitaciones.
  <br>
  <br>
  <h4>Análisis, login de usuario:</h4>
  <br>
  <br>
  De los 10 casos de prueba ejecutados, 5 fueron exitosos, cumpliendo con las expectativas tanto en las pruebas consideradas satisfactorias como en aquellas que se esperaba un mensaje de error, el cual se obtuvo correctamente. 
  <br>
  <br>
  Se ejecutaron las pruebas, detalladas en el informe de Plan de pruebas RF01, mediante las cuales se comprobó el correcto funcionamiento del login, que no permite dejar campos vacíos por lo cual da la alerta de error y para este caso puntual solo admite ingresar con los datos pre establecidos.
  <br>
  <br>
  Una vez que se accede de manera correcta, es posible continuar con las demás funcionalidades del sitio. 
  <br>
  <br>
  Por otro lado, se encontraron 5 casos de prueba bloqueados debido a la  imposibilidad de ejecutar las pruebas para el rol cliente, ya que no se contaba con los datos necesarios para un acceso adecuado.
  </p>
  <h4>Sistema mobile:</h4>
  <p>
   Se realizó una sesión exploratoria, con una duración aproximada de 5 minutos donde se observó el correcto funcionamiento de la página logrando ejecutar las pruebas preestablecidas, en los diferentes informes de pruebas ya presentados, con el fin de verificar su funcionamiento y se obtuvieron los resultados esperados. En términos generales el sistema opera en condiciones similares tanto en dispositivos móviles como en la web. Un detalle quizás poco relevante pero a modo de comentario adicional, es que en las pruebas realizadas en  no se logra apreciar el logo de la página, queda el icono, como si tuviera dificultades en cargar la imágen. 
  </p>
  <h4>Sesión exploratoria en la web, Navegador Firefox:</h4>
  <p>
   Se realizó una sesión de aproximadamente 15 minutos la cual permitió observar la funcionalidad, usabilidad y la interfaz de la web. Se insertaron datos para el login de usuario, registro de clientes, mascotas y vacunas para verificar su correcto funcionamiento. En general el sistema funcionó adecuadamente, visualmente la página se ve bien, cómo era de esperarse, el logo se aprecia correctamente y se puede hacer zoom en la pantalla y la barra lateral para scrollear funciona adecuadamente. Los botones cumplen con la característica de usabilidad y funcionalidad, permitiendo acceder al registro de clientes,mascotas y vacunas e ingresar los datos correctamente. 
  <br>
  <br>
Otra observación respecto al manejo intuitivo de la página, es que al momento de registrar clientes, mascotas y vacunas, el sistema no es intuitivo, debido a que al loguearse y apretar el botón de agregar cliente, te devuelve a la página de inicio, debiendo ingresar los datos de usuario y cliente nuevamente. Sin embargo haciendo clic en un botón que no tiene rótulo permite continuar con el registro de mascotas y vacunas.
  </p>
  <h4>Sesión exploratoria en la web, Navegador Opera GX:</h4>
  <p>
   Se realizó una sesión exploratoria utilizando el navegador Opera GX cuya duración fue de entre 10 a 15 minutos en la cual se investigó la funcionalidad, usabilidad y la interfaz de la web en este navegador. Se realizaron distintos ingresos con datos válidos e inválidos dentro del login de usuario, registro de clientes, mascotas y vacunas para verificar que los mismos cumplan su correcto funcionamiento. En términos generales el sistema funcionó adecuadamente, visualmente la página se ve bien con pequeñas sugerencias, el logo no se aprecia correctamente en este navegador, se puede hacer zoom in / zoom out en la pantalla y la barra de scroll funciona como se espera; los botones cumplen con la característica de usabilidad y funcionalidad, permitiendo acceder al registro de clientes, mascotas y vacunas e ingresar los datos correctamente.
  <br>
  <br>
  Se mantiene la misma observación mencionada en el navegador Firefox respecto al manejo intuitivo de la página.
  </p>
  <h3>Registro de nuevo Cliente</h3>
  <p>
   Pruebas Funcionales: En el retesting de las pruebas funcionales relacionadas con el registro de nuevos clientes en la aplicación Veterinaria Guau Guau la mayoría de las pruebas fallaron. Aunque el sistema permite registrar clientes y muestra una confirmación adecuada en algunos casos de registro exitoso, se detectaron fallos en 9 escenarios específicos. En estos casos, el sistema no mostró mensajes de error al ingresar datos inválidos en los campos de entrada, lo que permitió el registro incorrecto de clientes, afectando así la integridad de la información. 
<br>
<br>
Pruebas de Regresión: De las pruebas de regresión ejecutadas, las que fueron exitosas en etapas previas lograron mantener su estado positivo. Sin embargo, varias pruebas de regresión no lograron superar esta nueva etapa debido a que los defectos relacionados con datos inválidos persisten. 
<br>
<br>
Pruebas de Confirmación: Se realizaron pruebas de confirmación para verificar la corrección de incidentes previamente reportados. Estas pruebas revelaron que las incidencias siguen vigentes, especialmente en la validación de datos de entrada en los campos de nombre y apellido. Estos problemas continúan perjudicando el sistema al permitir el registro de clientes con datos incorrectos, demostrando que aún se requieren ajustes para garantizar una validación precisa y efectiva.
<br>
<br>
Validación de Datos: Se realizó una validación exhaustiva de los datos ingresados en el formulario de registro, verificando que el sistema detecte y gestione correctamente campos vacíos y formatos inválidos. La mayoría de los mensajes de error fueron adecuados, aunque se observaron casos donde datos inválidos en estos campos no fueron detectados correctamente, lo que permitió el registro incorrecto de clientes.  
  <br>
  <br>
Manejo de errores: Se comprobó que el sistema muestra mensajes de error claros cuando se omiten campos obligatorios. Sin embargo, en algunos casos de valores fuera de rango o con formatos no válidos, el sistema generó mensajes de éxito en lugar de error, lo que requiere ajuste. 
  <br>
  <br>
Hallazgos Adicionales: Durante el proceso de retesting, se identificaron inconsistencias en la validación de datos no válidos en ciertos campos, así como oportunidades de mejora en la claridad de algunos mensajes de confirmación y error. Se recomienda revisar y fortalecer la lógica de validación para asegurar que todos los datos ingresados sean verificados y gestionados correctamente, evitando registros incorrectos de clientes. 
  </p>
<h3>Registro de Mascotas</h3>
  <h4>Versión Web</h4>
  <p>
  La versión web mostró mejoras en la funcionalidad del campo de especie, aunque persisten algunos problemas menores de usabilidad:
    <ul>
      <li>Campo de Especie en Lista Desplegable: La lista desplegable permitió registrar correctamente las mascotas en categorías predeterminadas y mostrar especies no comunes con la opción “Otro”, mejorando la precisión de los registros.</li>
      <li>Errores en Validación de Otros Campos: Persisten algunos errores en la validación de datos en otros campos, sin bloquear el flujo de registro, pero afectando la integridad de los datos.</li>
      <li>Compatibilidad en Navegadores Secundarios: Se observaron diferencias en la visualización de elementos en Firefox y Safari, lo que podría mejorar para asegurar consistencia visual.</li>
    </ul>
  <br>
  Pruebas de validación de datos: El 73% de las pruebas de validación de datos  se completaron satisfactoriamente.  Pero se estima que el otro 27% de las funcionalidades del sistema no detecta valores límites, ni diferencia caracteres alfabéticos de alfanuméricos. 
  <br>
  <br>
  Prueba exploratoria: La interfaz de versión web funciona correctamente. Se adapta a la pantalla si el usuario se dispone a hacer zoom y no tiene problemas de usabilidad.
  </p>
  <h4>Versión Mobile</h4>
  <p>
   En la versión mobile, se observaron mejoras similares, aunque algunos problemas de visualización y usabilidad persisten:
    <ul>
      <li>Campo de Especie: La lista desplegable funcionó correctamente, permitiendo la selección de especies no comunes y registrando exitosamente en la lista de mascotas del cliente.</li>
      <li>Problemas de Visibilidad y Accesibilidad: La interfaz no se ajustó adecuadamente en todos los dispositivos móviles, afectando la navegación y la facilidad de uso en pantallas pequeñas.</li>
    </ul>
  Pruebas de validación de datos: El 35% de las pruebas de validación de datos se completaron satisfactoriamente. El sistema mobile presenta los mismos errores que su contraparte en Web. No detecta valores límites, ni diferencia caracteres alfabéticos de alfanuméricos. 
  <br>
  <br>
 Prueba exploratoria: La interfaz de la versión mobile presenta varios problemas. No es responsive, por lo que si el usuario decide hacer zoom, éste no se adapta a la pantalla del dispositivo. Además, el logo de la empresa no carga y está dañado. Los botones de “Cancelar” y “Registrar Vacunas” ahora si se encuentran conectados a los respectivos formularios. Por lo tanto, cumplen su función al ejecutarlos. 
  </p>
  <h3>Registro de Vacunas</h3>
  <p>
    <ul>
      <li>Pruebas Funcionales: Las pruebas funcionales confirmaron que el sistema permite el ingreso correcto de datos válidos en el módulo de registro de vacunas, mostrando un mensaje de confirmación exitoso al usuario cuando se completan todos los campos requeridos de manera adecuada.</li>
       <li>Validación de Campos Obligatorios: Las pruebas demostraron que el sistema responde adecuadamente a la omisión de datos en campos obligatorios, generando mensajes de error claros cuando el usuario deja en blanco alguno de los campos requeridos, como Nombre, Dosis, Fecha de Aplicación o Fecha de Vencimiento.</li>
       <li>Validación de Datos Fuera de Rango: La mayoría de los datos fuera de los límites permitidos fueron rechazados correctamente. Sin embargo, se identificaron algunos fallos críticos en el tratamiento de datos inválidos:
<br>
<ul>
  <li>Nombre con más de 100 caracteres: El sistema permitió el registro de nombres que exceden el límite de caracteres, lo cual debería ser rechazado y requiere corrección.</li>
  <li>Nombre con caracteres no alfanuméricos: El sistema permitió el registro de nombres que contienen caracteres especiales, lo cual no cumple con los requisitos y debe revisarse.</li>
  <li>Fecha de vencimiento anterior a la fecha de aplicación: Aunque se espera que el sistema rechace fechas de vencimiento que ocurren antes de la fecha de aplicación, en algunos casos, esta validación no se activó y el sistema permitió el registro incorrecto.</li>
</ul>
</li>
    </ul>
  Estos fallos indican que es necesario revisar las validaciones en el sistema para evitar que datos fuera de los rangos permitidos sean aceptados durante el registro de vacunas.
  </p>
</div>

<br>

<div>
  <h2>Base de Datos</h2>
  <p>
  La base de datos de la veterinaria Guau Guau está compuesta por tres entidades CLIENTE, MASCOTA y VACUNA. Todas ellas presentan oportunidades de mejoras o tienen alguna limitación con respecto a las formas de normalización.
<ol>
  <li>La tabla CLIENTES presenta una posibilidad de mejora en el atributo Dirección, ya que este no se encuentra normalizado.
    <br>
Esto permite: <br>
    <ul>
      <li>Realizar búsquedas o filtros más específicos. Por ejemplo, buscar clientes por ciudad o barrio.</li>
      <li>Colocar restricciones más específicas. Por ejemplo, que el numeroPuerta deba ser un número entero de hasta 4 dígitos.</li>
      <li>Aplicar cambios con mayor facilidad. Es posible realizar cambios en los distintos campos sin la necesidad de hacerlo para toda una cadena de dirección.</li>
    </ul>
</li>
  <li>Con respecto a la tabla MASCOTAS, se detectaron dos posibles mejoras en el atributo Especie: <br>
    <ul>
      <li>Utilizar una restricción CHECK para estandarizar los datos y evitar errores o variaciones innecesarias en la información. Por ejemplo, se evitarían inconsistencias como “perro”, “Perro”, “PERRO” para la misma especie. 
Esto brinda un mejoramiento en la calidad en la validación de datos y minimiza la posibilidad de errores humanos al ingresar especies no válidas. Por  último, la restricción CHECK permite facilidad de mantenimiento, ya que, si se necesita agregar más especies, solo basta con actualizar dicha restricción.</li>
      <li>Crear una tabla de referencia llamada ESPECIES. Esta tabla enlista las especies válidas. Luego se puede establecer una clave foránea en la tabla MASCOTAS que apunte a la tabla ESPECIES. 
Esto permite gestionar y actualizar las especies válidas de forma más sencilla.
</li>
    </ul>
  </li>
  <li>En la tabla VACUNAS se detectaron otras potenciales mejoras:
<br>
    <ul>
      <li>Con respecto al atributo Dosis se entiende que es necesaria una mejor clarificación.
</li>
      <li>Con respecto a los atributos Fecha Aplicación y Fecha Vencimiento, se sugiere agregar una restricción CHECK para asegurar que Fecha Vencimiento sea posterior a Fecha Aplicación. Esto evitaría errores en los registros de fechas. 
</li>
      <li>Otra posible sugerencia de mejora es crear una tabla de TIPOS_DE_VACUNAS con dos campos: Nombre y VacunaID. Luego, esta tabla puede ser referenciada en la tabla VACUNAS a través de una llave foránea. Esto puede resultar útil para estandarizar las vacunas en un solo lugar.</li>
      <li>Por último, se sugiere como mejora establecer una clave única compuesta por Mascota ID, Nombre y Fecha Aplicacion para evitar que se registre la misma vacuna para una mascota en la misma fecha. 
</li>
    </ul>
  </li>
</ol>  
  </p>
</div>

<br>

<div>
  <h2>Accesibilidad</h2>
  <p>
    El 64% de las pruebas realizadas para verificar la accesibilidad del sitio resultaron ser exitosas. <br>
Si bien esto puede percibirse como un sitio con una buena noticia para los usuarios con discapacidades visuales o motrices, aún queda mucho por mejorar en este aspecto. 
  </p>
</div>

<br>

<div>
  <h2>Compatibilidad y Usabilidad</h2>
  <p>
    Se realizaron 14 pruebas para verificar la compatibilidad y usabilidad del sitio web de la Veterinaria Guau Guau. 
El 86% de estas pruebas fueron ejecutadas con éxito. El 14% de las pruebas resultaron fallidas y todas éstas se concentraron en la parte móvil.
Todas las pruebas ejecutadas en distintos navegadores del entorno web resultaron exitosas. A partir de esto, se puede inferir que el sitio no presenta problemas de compatibilidad ni usabilidad en navegadores web. Sin embargo, estos problemas surgen en el entorno móvil, lo que sugiere que el desarrollo actual de las funcionalidades no está enfocado en estos usuarios.
  </p>
</div>

<br>

<div>
  <h2>DATOS Y MÉTRICAS</h2>
</div>

<br>

<div>
  <h2>RECOMENDACIONES</h2>
  <p>
    En base a los resultados obtenidos durante el proceso de testing se hacen las siguientes recomendaciones: <br>

Reforzar la validación de datos en los distintos formularios para proteger al sistema de los posibles errores de usuario, aplicando restricciones a los distintos campos. 
Se recomienda aplicar técnicas de valores límites, ya que este continúa siendo la mayor debilidad del sistema.  <br>

Para mejorar la compatibilidad del sitio se sugiere aplicar responsive design, para que éste se adapte a las distintas resoluciones de pantalla. También vuelve adaptables los elementos que lo componen, como las tablas en la sección “Dashboard”, ya que éstas se “salen” del formulario cuando contienen datos muy extensos. <br>

Con respecto a la usabilidad del sitio, se recomienda agregar al “Dashboard” una tabla de Clientes para poder gestionarlos desde la administración. Si se necesita “dar de baja” un cliente, el sistema no permite realizar esta acción. Tampoco se visualiza a qué cliente corresponde qué mascota debido a la ausencia de una tabla. 
Por último, para mejorar la usabilidad y la experiencia de usuario, se recomienda que el sistema permita “editar” mascotas y vacunas con el fin de actualizar o corregir información ya existente. 
En cuanto a la interfaz, se recomienda el uso de mensajes más descriptivos y reubicar algunos botones (como la casilla de registrar mascota en el formulario Registro de Cliente). <br>

En cuanto a la accesibilidad del sitio, se sugiere adoptar algunas medidas para mejorar la experiencia de los usuarios con discapacidades. Estas medidas se basan en las normas WCAG y son por ejemplo:
<br>
<ul>
  <li>Mejora en la navegación por teclado. El contenido principal no está señalizado y esto obliga al usuario a recorrer toda la página para poder encontrarlo.</li>
  <li>Agregar botones de ayuda o más información.</li>
  <li>Agregar al código atributos ARIA para mejorar la experiencia de usuarios no videntes o con discapacidades visuales. Sin estos atributos las tecnologías de asistencia no reconocen correctamente los mensajes. 
</li>
  <li>Cambiar el título de la página “Sistemas de Gestión de Clientes y Mascotas - Veterinaria XYZ” por el título “Sistemas de Gestión de Clientes y Mascotas - Guau Guau Veterinaria”. Esto permite que los usuarios no videntes puedan reconocer la empresa a través de la tecnología de asistencia. Un nombre de empresa incorrecto puede traer confusión y frustración. 
</li>
</ul>
<br>
En referencia a la documentación del sistema, se solicita agregar en los anexos del ESRE especificaciones más exhaustivas de las distintas variables que maneja el sistema. Por ejemplo, en el “Registro de Vacunas” se puede especificar qué se entiende por Dosis. Si se está haciendo referencia a la cantidad de dosis aplicada en la mascota (por ejemplo 0.5 mg) o si hace referencia al número de dosis aplicada en la mascota (por ejemplo primera o segunda dosis). <br>

Con respecto a la base de datos proporcionada, se sugiere adoptar un modelo que aporte mayor completitud que incluya las sugerencias aportadas en el informe técnico. <br>

Se muestra en el modelo las dos posibles formas de representar el atributo Dosis. Como un atributo único en el caso de que se entienda como el número de dosis aplicada. Como dos atributos distintos en caso de entenderla como la cantidad de dosis aplicada. <br>


  </p>
</div>

<br>

<div>
  <h2>CONCLUSIONES</h2>
  <h3>Validación de datos
</h3>
  <p>
    En términos generales, se puede decir que el sistema aún se encuentra con limitaciones. Si bien la mayoría de las pruebas realizadas se completaron con éxito, el 36% de las pruebas fallidas se relacionan a problemas de validación de datos y de usabilidad. Estos problemas pueden significar debilidades tanto en seguridad (inyecciones SQL por ejemplo) como en la integridad de la información (por ejemplo ingreso de información incompleta o datos erróneos). <br>
Además, pueden causar una mala experiencia de usuario reduciendo la confianza que tenga éste en el sistema reduciendo su disposición a utilizarlo. 
Problemas de validación en una etapa inicial, no solo dificulta el procesamiento de la información, sino que también puede implicar futuros costos de mantenimiento y corrección de errores. 

  </p>

  <h3>Usabilidad</h3>
  <p>
    En cuanto a la interfaz, se puede inferir que aplicar las sugerencias de mejora que aparecen en este informe (como agregar una tabla de gestión de clientes en la sección Dashboard) mejoraría la usabilidad de la herramienta. 

  </p>

  <h3>Accesibilidad</h3>
  <p>
    Por último, si bien la mayoría de las pruebas de accesibilidad fueron exitosas, el sitio aún carece de características importantes que incluyan a los usuarios de tecnologías de asistencia, como el uso de botones de ayuda o una buena configuración de alto contraste. 
  </p>

  <h3>Conclusión final</h3>
  <p>
    Por lo tanto, se concluye que la validación de datos sigue siendo el principal problema del sitio web de la veterinaria y desde el equipo se cree que éste debe ser atendido como prioridad. Una posible solución es agregar criterios de aceptación de datos en cada campo de los distintos formularios. Además, se sugiere reforzar la integridad de los datos permitiendo al usuario releer, corregir y confirmar los datos antes de registrar un nuevo cliente, mascota o vacuna. Esto permitirá optimizar la experiencia del usuario y reducir el riesgo de errores en futuras interacciones con el sistema.
<br>
<br>
Este informe resume los resultados clave del proceso de retesting. Si tienes alguna pregunta o necesitas información adicional, no dudes en contactarnos.

  </p>
</div>
  
<div align = right>
  <a href = "#indice"><img alt="Static Badge" src="https://img.shields.io/badge/INICIO%20%E2%98%9D%EF%B8%8F%20-%20blue?style=for-the-badge" width = 100px></a>
</div>
