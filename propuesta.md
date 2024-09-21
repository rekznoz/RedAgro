# Documento de propuesta  

### Indice
1. [Idea de la aplicación](#idea-de-la-aplicación)
2. [Audiencia objetiva](#audiencia-objetiva)
3. [Análisis de mercado](#análisis-de-mercado)
4. [Funcionalidades clave](#funcionalidades-clave)
5. [Modelos de ejecución](#modelos-de-ejecución)
6. [Lenguajes de programación web](#lenguajes-de-programación-web)
7. [Tecnologías a utilizar](#tecnologías-a-utilizar)
8. [Compatibilidad en navegadores](#compatibilidad-en-navegadores)

## Idea de la aplicación

Mi idea es la de desarrollar una **plataforma** que conecte a los trabajadores del campo como **pequeñas y medianas empresas agrícolas, agricultores locales o autonómicos**, el propósito de la aplicación es permitir a los trabajadores crear perfiles donde puedan explicar su experiencia, habilidad y disponibilidad mientras las empresas podrán publicar ofertas de trabajo o búsqueda de recursos, la idea es facilitar el contacto de las empresas con trabajadores mas desconocidos para **promover** en cierta manera que el pequeño agricultor tenga la **oportunidad** de ofrecer su producto de forma nacional. 

## Audiencia objetiva

### Trabajadores del campo (Jornaleros y Agricultores)

Muchas veces a estas personas les es difícil tener un acceso a oportunidades laborales directamente con el empresario y tienen que depender de intermediarios que pueden llevarse cierto porcentaje de lo que producen o lo que ganan haciendo su trabajo.  

- Tendrian acceso directo a empleados sin intermediarios.  
- Una mayor visibilidad de su trabajo.  
- Posibilidad de establecer contactos con empresas.

### Pequeña y mediana empresa y agricultores independientes

Las empresas o agricultores que necesiten contratar mano de obra, muchas veces tienen difícil   
encontrar trabajadores en su zona, ya sea por la lejanía o por el difícil acceso a la misma.

- Acceso a una lista de trabajadores disponibles según región o zona.  
- Facilitar el proceso de contratación sin terceras personas.  
- Reducción del gasto en búsqueda de mano de obra.

## Análisis de mercado

### Plataformas similares

1. [AgroJob](https://agrojobs.agenciascolocacion.com/) 
2. [FarmForce](https://farmforce.com/)

### Características Comunes

1. Perfiles de usuario, todas las plataformas permiten a los trabajadores crear un perfil donde destacar su experiencia, habilidades y disponibilidad.
   
2. Ofertas de empleo filtradas, permiten que las publicaciones de las empresas sean filtradas por ubicación, habilidad, tipo… y los trabajadores pueden buscar por esos criterios.

3. Comunicacion Interna, ofrece un sistema de mensajería o chat entre empresas y trabajadores es comun.

4. Calificaciones y Reseñas, se pueden clasificar con reseñas los empleados, trabajadores y empresas.

### Oportunidades de Diferenciación
	
1. Un enfoque mas centrado en los agricultores rurales de zonas remotas y autónomos, las webs estan mas centradas en las grandes empresas y mi objetivo es centrarme en la pequeña y mediana empresa y/o en los agricultores autónomos.

2. Las plataformas en general estan creadas de forma muy intrincada y complicada, mi idea es que al entrar tengas acceso a la información necesaria, ya que a la persona que entra no le interesa información que no quiere ver o una pantalla de inicio que no le ayuda en nada hay que pensar también que muchas veces las personas mas rurales tienen difícil el entendimiento de las plataformas digitales por eso debe ser simple y llana.

3. Darle un apoyo a la transparencia y el trabajo justo, haciendo promoción a las condiciones laborales justas y a la transparencia en los salarios del jornalero y su contrato, dando herramientas por ejemplo que permitan a un trabajadores verificar la reputación de la empresa en términos de condiciones y remuneración.

### Valor Añadido

1. Inclusión y Acceso Rural, enfocarse en poblaciones rurales, dando acceso a empleos en zonas de difícil acceso.

2. Transparencia y Ética Laboral, promocionar condiciones laborales justas y herramientas para evaluar tanto a empleadores como a trabajadores, lo que genera confianza en el uso de la plataforma.

3. Solución Integral Agrícola, ofrecer no solo una conexión entre trabajadores y empleadores, sino también una plataforma agrícola, incluyendo recursos adicionales que amplíen el valor de la plataforma.

## Funcionalidades clave

### 1. Perfil de Usuario para Trabajadores del Campo

* **Información básica:** Nombre, ubicación, experiencia laboral, habilidades específicas (tipos de cultivos que pueden recolectar, maquinaria que saben manejar, etc.).  
* **Disponibilidad:** Horarios o temporadas en las que están disponibles para trabajar.  
* **Portafolio:** Imágenes o videos de su trabajo, testimonios o referencias de empleadores anteriores.  
* **Certificaciones:** Si tienen alguna formación técnica o capacitación, deberían poder subir estos documentos.  
* **Ubicación geográfica:** Un mapa para visualizar las regiones donde trabajan o prefieren trabajar.

### 2. Perfil de Usuario para Empresas y Agricultores

* **Información de la empresa o agricultor individual:** Nombre, ubicación, tipos de cultivos, tamaño del terreno.  
* **Ofertas laborales:** Publicar vacantes para trabajos temporales o a largo plazo, con detalles sobre salario, duración del trabajo, y condiciones laborales.  
* **Requisitos:** Las habilidades y experiencia necesarias para los trabajos.  
* **Valoraciones:** Posibilidad de valorar y comentar a los trabajadores después de haber colaborado con ellos.

### 3. Sistema de Búsqueda y Filtro

* **Por ubicación:** Las empresas podrían buscar trabajadores disponibles en zonas específicas.  
* **Por habilidad o experiencia:** Filtrar a trabajadores que tengan experiencia en tipos específicos de cultivos o tareas (recolección de frutas, manejo de maquinaria agrícola, etc.).  
* **Por disponibilidad temporal:** Especialmente importante en la agricultura, donde muchas labores son estacionales.

### 4. Calificación y Referencias

* **Sistema de calificaciones:** Tanto empresas como trabajadores podrían calificarse mutuamente, con base en la calidad del trabajo o las condiciones ofrecidas.  
* **Referencias:** Opción de que los trabajadores puedan incluir referencias de empleadores anteriores que respalden su experiencia.

### 5. Énfasis en la Transparencia y las Buenas Prácticas

* **Condiciones laborales justas:** Debería haber un enfoque en promover la transparencia sobre las condiciones de trabajo y asegurar que las empresas ofrezcan contratos justos y condiciones dignas para los trabajadores del campo.  
    
## Modelos de ejecución

	En el modelo cliente la aplicación se ejecuta en el dispositivo del usuario con lo cual es necesario   
	descargar el código y procesarlo en su máquina, en el modelo servidor el codigo se ejecuta en un  
	servidor ajeno al cliente y el cliente solo recibe los resultados, el cliente vendría a ser un intermediario   
	entre usuario y servidor.

	**Caracteristicas:**

- En el modelo cliente el código se ejecuta en un navegador o una aplicación instalada mientras que en servidor todo el procesamiento de datos ocurre en un sistema aparte.  
- En el modelo cliente los recursos utilizados son los del dispositivos del usuario, mientras que en el servidor el procesamiento lo realiza un sistema que esta dedicado a ello.  
- En el modelo cliente las respuestas a las acciones del usuario deberian ser inmediatas, sin necesidad de necesitar una respuesta de un tercero, mientras que en el servidor tiene que estar en continuo contacto el cliente con el servidor, y el cliente debe esperar la respuesta del servidor  
- En el modelo cliente, el código es totalmente accesible por cualquier usuario para ser manipulado a su gusto en buena o mala manera, en el modelo servidor el codigo esta oculto en el servidor y no puede ser editado por personas ajenas a el.  
- El modelo cliente esta limitado a la capacidad del dispositivo del usuario no puede escalar por sí solo, en el modelo servidor, el servidor esta abierto a cambios y siempre puede escalar su potencia.

	**Ventajas**

1. **Interactividad**: En el **modelo cliente** las respuestas son rápidas y fluidas, permitiendo una experiencia de usuario más dinámica, mientras que en **servidor** la interacción puede ser más lenta debido a la latencia en la comunicación.  
2. **Carga en el Servidor**: En el **modelo cliente** se reduce la carga del servidor, ya que el procesamiento se realiza en el dispositivo del usuario, mientras que en **servidor** el servidor asume todo el procesamiento, lo que puede provocar cuellos de botella si hay muchos usuarios.  
3. **Desarrollo Offline**: En el **modelo cliente** es posible trabajar con ciertas funcionalidades sin conexión a Internet, mientras que en **servidor** se necesita conexión constante para acceder a la aplicación.  
4. **Uso de Recursos Locales**: En el **modelo cliente** se aprovechan los recursos del dispositivo del usuario (como GPU para gráficos), mientras que en **servidor** depende de la capacidad del servidor para realizar tareas pesadas.  
5. **Menos Costos de Servidor**: En el **modelo cliente** puede reducirse el costo de infraestructura de servidores, mientras que en **servidor** los costos pueden aumentar a medida que se escala para atender más usuarios.

   ### **Inconvenientes**

1. **Dependencia del Cliente**: En el **modelo cliente** la experiencia del usuario puede verse afectada por las limitaciones del dispositivo, mientras que en **servidor** se garantiza una experiencia uniforme ya que todo el procesamiento es centralizado.  
2. **Seguridad**: En el **modelo cliente** el código puede ser examinado y manipulado por los usuarios, lo que puede generar riesgos de seguridad, mientras que en **servidor** el código y los datos sensibles están protegidos en el servidor.  
3. **Compatibilidad**: En el **modelo cliente** el desarrollo debe considerar diferentes dispositivos y navegadores, lo que puede aumentar la complejidad, mientras que en **servidor** se trabaja en un entorno más homogéneo.  
4. **Mantenimiento**: En el **modelo cliente** cada usuario debe actualizar su aplicación manualmente, mientras que en **servidor** las actualizaciones se realizan de forma centralizada, simplificando el mantenimiento.  
5. **Acceso a Datos**: En el **modelo cliente** las operaciones que requieren acceso a bases de datos pueden ser limitadas, mientras que en **servidor** se tiene acceso completo a bases de datos y lógica de negocio, lo que facilita la gestión de datos complejos.

   #### **Ejemplos de Tecnologías de Ejecución en Cliente:**

* **JavaScript**: Lenguaje de programación ejecutado en el navegador. Ejemplos: aplicaciones web como juegos en línea, visualizadores de gráficos, etc.  
* **Frameworks y Librerías**: React, Angular, Vue.js (para la construcción de interfaces dinámicas del lado del cliente).  
* **HTML5 y CSS3**: Usados para la estructura y estilo del contenido en el lado del cliente.  
* **Aplicaciones de Escritorio**: Software como Microsoft Word o Photoshop, que se ejecuta completamente en la máquina del usuario.

  #### **Ejemplos de Tecnologías de Ejecución en Servidor:**

* **PHP, Python, Ruby, Java, Node.js**: Lenguajes de programación que permiten la ejecución del lado del servidor.  
* **Servidores Web**: Apache, Nginx, IIS, que gestionan las solicitudes HTTP y despachan los resultados.  
* **Bases de Datos**: Las operaciones que involucran bases de datos, como consultas SQL o MongoDB, se ejecutan en el servidor.  
* **Aplicaciones Web**: Redes sociales (Facebook, Twitter), sistemas de gestión (ERP, CRM), aplicaciones SaaS (Software as a Service).

## Lenguajes de programación web

   ### **JavaScript**

   **Ventajas:**  
1. **Ubicuidad:** Es el lenguaje estándar para el desarrollo web, soportado por todos los navegadores.  
2. **Facilidad de aprendizaje:** Su sintaxis es relativamente sencilla, lo que lo hace accesible para principiantes.  
3. **Gran ecosistema:** Amplia variedad de bibliotecas y frameworks (como React, Angular y Vue) que facilitan el desarrollo.  
4. **Interactividad:** Permite crear experiencias interactivas y dinámicas en la web de manera efectiva.  
   **Desventajas:**  
1. **Tipado dinámico:** Puede llevar a errores difíciles de detectar, ya que las variables no tienen un tipo fijo.  
2. **Falta de herramientas de desarrollo:** Aunque ha mejorado, el soporte para autocompletado y análisis estático puede ser limitado en comparación con lenguajes tipados.  
3. **Dificultades con la escalabilidad:** En proyectos grandes, la falta de estructura y tipado puede complicar el mantenimiento y la comprensión del código.

   ### **TypeScript**

   **Ventajas:**

1. **Tipado estático:** Permite definir tipos para variables y funciones, lo que ayuda a detectar errores en tiempo de compilación, mejorando la calidad del código.  
2. **Mejoras en la productividad:** Las herramientas de desarrollo (como autocompletado y refactorización) son más potentes gracias al tipado, lo que acelera el proceso de desarrollo.  
3. **Compatibilidad con JavaScript:** TypeScript se compila a JavaScript, lo que permite usar bibliotecas y frameworks existentes.  
4. **Características modernas:** Soporta características de ECMAScript más avanzadas, como decoradores y interfaces, antes de que estén completamente implementadas en JavaScript.  
   **Desventajas:**  
1. **Curva de aprendizaje:** Puede ser más complejo para quienes están acostumbrados a la flexibilidad de JavaScript, especialmente al principio.  
2. **Configuración adicional:** Requiere un paso de compilación adicional y, en algunos casos, una configuración más compleja.  
3. **Sobrecarga de código:** Puede resultar en un código más extenso debido a las anotaciones de tipos y las interfaces, lo que puede ser visto como un inconveniente en proyectos pequeños.

## Tecnologías a utilizar

**HTML**:

* **Justificación**: HTML es el lenguaje de marcado estándar para crear la estructura de las páginas web. Es fundamental para cualquier desarrollo web, ya que permite organizar el contenido y definir su jerarquía.  
  **JavaScript**:  
* **Justificación**: JavaScript es el lenguaje de programación que permite la interactividad en el frontend. Es esencial para desarrollar una experiencia de usuario dinámica, como la manipulación de elementos en la página, la gestión de eventos y la comunicación con el servidor a través de AJAX.

	**PHP (con Laravel)**:

* **Justificación**: PHP es un lenguaje de programación ampliamente utilizado para el desarrollo web del lado del servidor. Laravel es un framework PHP que facilita el desarrollo mediante la implementación de patrones arquitectónicos modernos, como MVC (Modelo-Vista-Controlador), así como herramientas para la autenticación, la validación y la gestión de bases de datos. Su sintaxis elegante y sus funcionalidades robustas lo hacen ideal para construir aplicaciones web complejas de forma eficiente.

	**MySQL**:

* **Justificación**: MySQL es un sistema de gestión de bases de datos relacional muy popular y eficiente. Se integra bien con PHP y Laravel, ofreciendo robustez y flexibilidad para manejar datos estructurados, ideal para almacenar información sobre usuarios, empleos, perfiles y calificaciones.  

### Evaluación de los mecanismos de integración de lenguajes de marcas con lenguajes de programación de clientes

HTML y JavaScript se integran de las siguientes maneras:

1. **Estructura y Comportamiento**: HTML proporciona la estructura de la página web (etiquetas, encabezados, párrafos, formularios, etc.), mientras que JavaScript se utiliza para añadir comportamiento a esa estructura. Por ejemplo, un formulario HTML puede ser validado usando JavaScript antes de enviarlo al servidor.  
2. **Manipulación del DOM**: JavaScript permite acceder y modificar dinámicamente el Document Object Model (DOM), que es la representación en memoria del documento HTML. Esto significa que los desarrolladores pueden agregar, eliminar o modificar elementos HTML en respuesta a acciones del usuario (como clics o desplazamiento).  
3. **Eventos**: JavaScript puede agregar manejadores de eventos a elementos HTML, lo que permite que el contenido responda a interacciones del usuario, como hacer clic en botones o enviar formularios.

### Evaluación de herramientas de programación para clientes web

**Editores de Código**:

* **Visual Studio Code**:  
  * **Justificación**: Este editor es ligero, personalizable y cuenta con extensiones para múltiples lenguajes, incluido HTML y JavaScript. Su soporte para control de versiones, terminal integrada y funciones de depuración lo hacen ideal para el desarrollo web.  
    * **Funciones**: Autocompletado, integración con Git, terminal incorporada, soporte para múltiples lenguajes.  
      * **Ventajas**: Mejora la productividad del desarrollador al ofrecer un entorno amigable y personalizable.

    **Frameworks y Bibliotecas**:

* **Bootstrap**:  
  * **Justificación**: Esta biblioteca CSS proporciona componentes y un sistema de cuadrícula que permite desarrollar un diseño responsive de manera rápida y fácil. Facilita la creación de una interfaz atractiva y accesible.  
    * **Funciones**: Componentes predefinidos, sistema de cuadrícula, diseño responsive.  
      * **Ventajas**: Facilita el desarrollo de interfaces atractivas y funcionales sin necesidad de diseñar desde cero.  
* **Axios**:  
  * **Justificación**: Una biblioteca para hacer solicitudes HTTP desde el navegador, ideal para interactuar con el backend de Laravel de manera sencilla y efectiva. Permite gestionar fácilmente la comunicación asincrónica con el servidor.  
    * **Funciones**: Realiza solicitudes HTTP, maneja respuestas de forma sencilla.  
      * **Ventajas**: Permite interacciones rápidas y efectivas con el backend, mejorando la experiencia del usuario.  

## Compatibilidad en navegadores

	 **Google Chrome**

* **Manejo**: Chrome tiene un motor JavaScript muy avanzado (V8) que ofrece un excelente rendimiento y compatibilidad con las últimas características del lenguaje.  
* **Problemas de Compatibilidad**: Pocos problemas, aunque algunas características más nuevas de ECMAScript pueden no estar disponibles en versiones antiguas.  
  **Mozilla Firefox**  
* **Manejo**: Firefox utiliza el motor SpiderMonkey, que también tiene buen soporte para JavaScript moderno y funcionalidades avanzadas.  
* **Problemas de Compatibilidad**: Aunque es generalmente compatible, algunas APIs pueden comportarse de manera diferente en Firefox en comparación con Chrome.  
  **Microsoft Edge**  
* **Manejo**: La versión basada en Chromium de Edge ofrece una compatibilidad similar a Chrome, utilizando el motor V8.  
* **Problemas de Compatibilidad**: Principalmente relacionados con versiones anteriores de Edge (no Chromium), que pueden no soportar características modernas.  
  **Safari**  
* **Manejo**: Safari usa el motor JavaScriptCore (Nitro), que ofrece buena velocidad pero puede tener problemas de compatibilidad con ciertas funciones modernas de JavaScript.  
* **Problemas de Compatibilidad**: A menudo, hay discrepancias con funciones como `Promise` y APIs nuevas que pueden no estar completamente implementadas.

  ### **Identificación de Problemas de Compatibilidad y Soluciones**

1. **Uso de Polyfills**:  
   * **Descripción**: Los polyfills son scripts que permiten que los navegadores antiguos implementen funciones modernas que no soportan. Usar polyfills puede ayudar a garantizar que las características de JavaScript funcionen de manera consistente en todos los navegadores.  
   * **Ejemplo**: Polyfills para `Promise` y `fetch` pueden utilizarse para asegurar que estas funciones estén disponibles incluso en navegadores más antiguos.  
2. **Transpilación**:  
   * **Descripción**: Herramientas como Babel permiten escribir código JavaScript moderno que se transpila a una versión más antigua compatible con más navegadores. Esto ayuda a mantener la sintaxis moderna mientras se asegura la compatibilidad.  
   * **Ejemplo**: Al usar Babel, se puede escribir código con características de ECMAScript 6+ y convertirlo para que funcione en navegadores más antiguos.  
3. **Pruebas en Múltiples Navegadores**:  
   * **Descripción**: Es esencial probar la aplicación en diferentes navegadores y dispositivos para identificar problemas específicos de compatibilidad.  
   * **Solución**: Usar herramientas como BrowserStack o Sauce Labs para realizar pruebas cross-browser.

