# Informe técnico

### Menu de Navegacion
1. [Documento de propuesta](propuesta.md)
2. [Bibliografia](bibliografica.md)

### Indice
1. [Compatibilidad en navegadores](#compatibilidad-en-navegadores)
2. [Modelos de ejecución](#modelos-de-ejecucion)
3. [Lenguajes de programacion web](#lenguajes-de-programacion-web)
4. [Analisis de mercado](#analisis-de-mercado)

## Compatibilidad en navegadores

#### Google Chrome

* **Manejo**: Chrome tiene un motor JavaScript que ofrece un excelente rendimiento y compatibilidad sus últimas características.  

* **Problemas de Compatibilidad**: Pocos problemas, aunque algunas características más nuevas pueden no estar disponibles en versiones antiguas.  

#### Mozilla Firefox 

* **Manejo**: Firefox utiliza el motor SpiderMonkey, que también tiene buen soporte para JavaScript moderno y funcionalidades avanzadas.  

* **Problemas de Compatibilidad**: Aunque es generalmente compatible, algunas APIs pueden comportarse de manera diferente en Firefox en comparación con Chrome.  

#### Microsoft Edge

* **Manejo**: La versión basada en Chromium de Edge ofrece una compatibilidad similar a Chrome.

* **Problemas de Compatibilidad**: Principalmente relacionados con versiones anteriores de Edge (no Chromium), que pueden no soportar características modernas. 

#### Safari

* **Manejo**: Safari usa el motor JavaScriptCore, que ofrece buena velocidad pero puede tener problemas de compatibilidad con ciertas funciones modernas de JavaScript.  

* **Problemas de Compatibilidad**: A menudo, hay discrepancias con APIs nuevas que pueden no estar completamente implementadas.

### Identificación de Problemas de Compatibilidad y Soluciones

#### Polyfills

* **Descripción**: Los polyfills son scripts que permiten que los navegadores antiguos implementen funciones modernas que no soportan. Usar polyfills puede ayudar a garantizar que las características de JavaScript funcionen de manera consistente en todos los navegadores.  

* **Ejemplo**: Polyfills para `fetch` pueden utilizarse para asegurar que estas funciones estén disponibles incluso en navegadores más antiguos.  

#### Transpilación

* **Descripción**: Herramientas como Babel permiten escribir código JavaScript moderno que se transpila a una versión más antigua compatible con más navegadores. Esto ayuda a mantener la sintaxis moderna mientras se asegura la compatibilidad.  

* **Ejemplo**: Al usar Babel, se puede escribir código con características de ECMAScript y convertirlo para que funcione en navegadores más antiguos.  

#### Pruebas en Múltiples Navegadores

* **Descripción**: Es esencial probar la aplicación en diferentes navegadores y dispositivos para identificar problemas específicos de compatibilidad.  

* **Solución**: Usar herramientas como BrowserStack o Sauce Labs para realizar pruebas cross-browser.

## Modelos de ejecucion

En el modelo cliente la aplicación se ejecuta en el dispositivo del usuario con lo cual es necesario   
descargar el código y procesarlo en su máquina, en el modelo servidor el codigo se ejecuta en un  
servidor ajeno al cliente y el cliente solo recibe los resultados, el cliente vendría a ser un intermediario entre usuario y servidor.

### Caracteristicas

- En el modelo cliente el código se ejecuta en un navegador o una aplicación instalada mientras que en servidor todo el procesamiento de datos ocurre en un sistema aparte.  
- En el modelo cliente los recursos utilizados son los del dispositivos del usuario, mientras que en el servidor el procesamiento lo realiza un sistema que esta dedicado a ello.  
- En el modelo cliente las respuestas a las acciones del usuario deberian ser inmediatas, sin necesidad de necesitar una respuesta de un tercero, mientras que en el servidor tiene que estar en continuo contacto el cliente con el servidor, y el cliente debe esperar la respuesta del servidor  
- En el modelo cliente, el código es totalmente accesible por cualquier usuario para ser manipulado a su gusto en buena o mala manera, en el modelo servidor el codigo esta oculto en el servidor y no puede ser editado por personas ajenas a el.  
- El modelo cliente esta limitado a la capacidad del dispositivo del usuario no puede escalar por sí solo, en el modelo servidor, el servidor esta abierto a cambios y siempre puede escalar su potencia.

#### Ventajas e Inconvenientes

1. **Interactividad**: En el **modelo cliente** las respuestas son rápidas y fluidas, permitiendo una experiencia de usuario más dinámica, mientras que en **servidor** la interacción puede ser más lenta debido a la latencia de la comunicación.

2. **Carga en el Servidor**: En el **modelo cliente** se reduce la carga del servidor, ya que el procesamiento se realiza en el dispositivo del usuario, mientras que en **servidor** el servidor asume todo el procesamiento, lo que puede provocar cuellos de botella si hay muchos usuarios.

3. **Desarrollo Offline**: En el **modelo cliente** es posible trabajar con ciertas funcionalidades sin conexión a Internet, mientras que en **servidor** se necesita conexión constante para acceder a la aplicación.

4. **Uso de Recursos Locales**: En el **modelo cliente** se aprovechan los recursos del dispositivo del usuario (como GPU para procesado), mientras que en **servidor** depende de la capacidad del servidor para realizar tareas pesadas.

5. **Menos Costos de Servidor**: En el **modelo cliente** puede reducirse el costo de infraestructura de servidores, mientras que en **servidor** los costos pueden aumentar a medida que se escala para atender más usuarios.

6. **Dependencia del Cliente**: En el **modelo cliente** la experiencia del usuario puede verse afectada por las limitaciones del dispositivo, mientras que en **servidor** se garantiza una experiencia 'optima' ya que todo el procesamiento es centralizado.

7. **Seguridad**: En el **modelo cliente** el código puede ser examinado y manipulado por cualquier usuario, lo que puede crear riesgo en la seguridad, mientras que en **servidor** el código y los datos sensibles están protegidos en el servidor y solo son manipulados por las personas con acceso al mismo.

8. **Compatibilidad**: En el **modelo cliente** el desarrollo debe considerar diferentes dispositivos y navegadores, lo que puede aumentar la complejidad, mientras que en **servidor** se trabaja en un entorno controlado.

9. **Mantenimiento**: En el **modelo cliente** cada usuario debe actualizar su aplicación manualmente, mientras que en **servidor** las actualizaciones se realizan de forma centralizada, simplificando el mantenimiento.

10. **Acceso a Datos**: En el **modelo cliente** las operaciones que requieren acceso a bases de datos deben ser limitadas y pueden exponer informacion delicada al usuario si se hace de mala forma, mientras que en **servidor** se tiene acceso completo a bases de datos, ademas se puede tener un acceso local si la base de datos se encuentra dentro del mismo servidor, ofreciendo una velocidad de acceso a datos inmediata.

### Ejemplos de Tecnologías de Ejecución en Cliente

* **JavaScript**: Lenguaje de programación ejecutado en el navegador. 
    - Aplicaciones web como juegos en línea, visualizadores de gráficos, etc.

* **Frameworks y Librerías**: React, Angular, Vue.js (para la construcción de interfaces dinámicas)

* **HTML y CSS**: Usados para la estructura y estilo del contenido.

### Ejemplos de Tecnologías de Ejecución en Servidor

* **PHP, Python, Ruby, Java, Node.js**: Lenguajes de programación que permiten la ejecución del lado del servidor.

* **Servidores Web**: Apache y Nginx gestionan las solicitudes HTTP y entregan los resultados.

* **Bases de Datos**: Las operaciones de bases de datos, como consultas, se ejecutan en el servidor.

## Lenguajes de programacion web

### **JavaScript**

**Ventajas:**  

1. **Compatibilidad:** Es el lenguaje estándar para el desarrollo web, soportado por todos los navegadores.

2. **Facilidad de aprendizaje:** Su sintaxis es relativamente sencilla, lo que lo hace accesible para principiantes.

3. **Ecosistema:** Amplia variedad de bibliotecas y frameworks (como React, Angular y Vue) que facilitan el desarrollo.

4. **Interactividad:** Permite crear experiencias interactivas y dinámicas en la web de manera efectiva.

**Desventajas:**  

1. **Tipado dinámico:** Puede llevar a errores difíciles de detectar, ya que las variables no tienen un tipo fijo.

2. **Falta de herramientas de desarrollo:** El soporte para autocompletado y análisis estático puede ser limitado.

3. **Dificultades con la escalabilidad:** En proyectos grandes, la falta de estructura y tipado puede complicar el mantenimiento.


### **TypeScript**

**Ventajas:**

1. **Tipado estático:** Permite definir tipos para variables y funciones, lo que ayuda a detectar errores en tiempo de compilación.

2. **Mejoras en la productividad:** Las herramientas de desarrollo (como autocompletado y refactorización) son más potentes gracias al tipado.

3. **Compatibilidad con JavaScript:** TypeScript se compila a JavaScript, lo que permite usar bibliotecas y frameworks existentes.

4. **Características modernas:** Soporta características de ECMAScript más avanzadas, como decoradores e interfaces, antes de que estén implementadas en JavaScript.

**Desventajas:**

1. **Curva de aprendizaje:** Puede ser más complejo para quienes están acostumbrados a la flexibilidad de JavaScript.

2. **Configuración adicional:** Requiere un paso de compilación adicional y, en algunos casos, una configuración más compleja.

3. **Sobrecarga de código:** Puede resultar en un código más extenso debido a las anotaciones de tipos y las interfaces, lo que puede ser visto como un inconveniente en proyectos pequeños.

## Analisis de mercado

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
