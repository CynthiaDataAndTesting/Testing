<div>
  <img src = "banner_proyecto.png" alt = "banner de proyecto">
</div>

<br>

<div>
  <p>Este proyecto lo realicé durante mi formación como Tester de Software de la mano de Jóvenes a Programar. Tuvo como principal objetivo poner en práctica los conocimientos aprendidos en un contexto de trabajo en equipo, asumiendo los roles que participan en el proceso de desarrollo de software. 
  <br>
  <br>
  En este caso, mi rol fue el de Team Manager y Líder de Documentación. 
  <br>
  Como Líder de equipo me dediqué a la búsqueda de herramientas, soluciones prácticas y procesos eficientes para que el equipo pudiera trabajar cómodamente. Tuve en cuenta las fortalezas y debilidades de cada miembro para que todos pudieran aplicar lo aprendido y se sintiera apoyado.
   <br>
  Como Líder de Documentación, me dediqué a crear modelos de reportes e informes para que todo el proyecto tuviera una coherencia al momento de llevar los registros. También creé un espacio en Google Drive para volcar los avances del equipo, y revisé redacción y coherencia de los distintos archivos.</p>
</div>

<div align = right>
  <a href = "#informes">
    <img alt="Static Badge" src="https://img.shields.io/badge/Informes%20completos%20-%20aqu%C3%AD%20-%20%23449BB3?style=for-the-badge">
  </a>
</div>

<br>

<div>
  <h2>Herramientas utilizadas:</h2>
  <div>
  <img width="100" height="100" src="https://img.icons8.com/bubbles/100/clickup.png" alt="clickup"/> <img width="96" height="96" src="https://img.icons8.com/fluency/96/ms-excel.png" alt="ms-excel"/> <img width="96" height="96" src="https://img.icons8.com/color/96/jira.png" alt="jira"/> <img width="96" height="96" src="https://img.icons8.com/color/96/google-drive--v2.png" alt="google-drive--v2"/> 
  </div>
</div>

<div>
  <p>
    <h1>Introducción</h1>
    <table>
      <tr>
        <th> <img  src = "logo.png" alt = "logo de la veterinaria guau guau"></th>
        <th>Este trabajo presenta los resultados del proceso de testing de las funcionalidades “Autenticación de Usuario”, “Registro de Nuevo Cliente”, “Registro de Mascota”, “Registro de Vacunas” y “Dashboard” de la web de la Veterinaria Guau Guau durante el período de prueba que abarca del 28/10/2024 al 10/11/2024. Además, se evaluó la integridad de la base de datos. El objetivo del testing fue evaluar la validación de datos, las formas de normalización, la accesiblidad, la compatibilidad y la usabilidad de la herramienta.</th>
      </tr>
    </table>
  </p>
</div>

<br>

<div>
  <h2>Pruebas que se ejecutaron</h2>
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

<br>

<div id = "informes">
  <h3>Ver informes completos aquí:</h3>
  <a href = "executive_report_testing.md">
    <img alt="Static Badge" src="https://img.shields.io/badge/Informe%20Final%20-%20ingl%C3%A9s%20-%20%23449BB3?style=for-the-badge">
  </a>
  <br>
  <a href = "Segundo_informe_etapa3.md">
    <img alt="Static Badge" src="https://img.shields.io/badge/Informe%20Final%20-%20espa%C3%B1ol%20-%20%23449BB3?style=for-the-badge">
  </a>
  <br>
  <a href = "https://youtu.be/ApZtqEXLhEA">
    <img alt="Static Badge" src="https://img.shields.io/badge/Video%20Presentaci%C3%B3n%20-%20aqu%C3%AD%20-%20%23449BB3?style=for-the-badge">
  </a>
</div>
