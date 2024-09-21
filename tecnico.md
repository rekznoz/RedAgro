# Informe técnico

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
