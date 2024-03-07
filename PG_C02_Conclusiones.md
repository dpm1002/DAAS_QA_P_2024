## Conclusiones SonarQube:
SonarQube es una herramienta muy potente de análisis de código y calidad. Permite configurar a medida para cada proyecto las reglas que se desean cumplir, teniendo numerosas posibilidades de configuración, tanto de reglas disponibles como de rangos y valores límite, lo cual la hace enormemente versátil.

Además, soporta una gran cantidad de lenguajes de programación (27) y se integra con los principales repositorios online (GitHub, GitLab, Bitbucket) por lo que da cobertura a casi cualquier tipo de proyecto posible.

Podemos destacar además, que al ofrecer el servicio tanto en aplicación de escritorio como en la nube, puede ayudar a mejorar la calidad en proyectos de diferentes tamaños y tanto en fase de desarrollo como en despliegue, integrándolo en el CI-CD del proyecto. Una vez integrado en el ciclo de CI-CD del proyecto, se usa para como filtro para evitar subir a producción código que no cumpla los criterios y reglas de calidad establecidas, no continuando el ciclo de despliegue si el análisis realizado no es exitoso.

Por último, indicar que sus interfaces de interacción son muy visuales y sencillas de utilizar, incluyéndose gráficos y un visor de código, ofreciendo hasta 11 badges diferentes para visualizar de forma rápida en el repositorio los resultados del análisis. 
Incluso nos muestra posibles soluciones a los problemas detectados basándose en las reglas establecidas. Todo esto facilita mucho la tarea de los desarrolladores a la hora de resolver los problemas de calidad detectados lo que aporta mucho valor al ciclo de desarrollo de los proyectos, pudiendo ahorrar mucho tiempo tanto localizando como resolviendo dichos problemas.

## Conclusiones Codebeat:
Codebeat es una aplicación sencilla que calcula un conjunto universal de métricas para los 10 lenguajes soportados para conseguir una buena calidad de código, modificación y mantenibilidad.

Pese a trabajar con menos lenguajes que otras herramientas disponibles, es flexible en su uso con varios repositorios.
Esta herramienta es open source, por lo que es accesible al público y todos pueden ver, modificar y distribuir el código, y así trabajar de manera colaborativa si fuera necesario.

Únicamente se puede usar On cloud, aunque permite analizar las métricas tanto en web como en dispositivos móviles.

Un punto negativo es que solamente analiza 4 métricas de código, lo cual está bien para un uso más ágil, pero perdemos cierta información que con otro tipo de herramienta si que obtendríamos.

Por sí sola no dispone de gestión de reportes, pero se pueden utilizar los reporters: ruby-test-reporter y javascript-test-reporter, los cuales son de código abierto y la documentación de Codebeat dispone de un tutorial para su uso.

Al igual que con “Java CI” y “codecov” usados anteriormente, esta herramienta dispone de 1 badge que puede ser utilizado en nuestro repositorio para tener más a mano la calificación “GPA” de calidad que realiza Codebeat.

Finalmente, hay que señalar que es una aplicación gratuita, aunque de esta forma solo sirve para repositorios públicos. La opción de pago es de 20$ al mes permite un número ilimitado de repositorios privados y un servicio dedicado.


## Conclusiones Codacy:
Codacy es una herramienta que de forma automatizada nos permite optimizar nuestro código, limpiarlo, corregir errores y hacerlo mas sencillo y legible, de tal modo que mejora la calidad del mismo.

Soporta un alto número de lenguajes, en concreto es capaz de evaluar 44 lenguajes de programación, de las herramientas evaluadas es la que mayor número de lenguajes soporta.

Es capaz de integrarse con 3 repositorios (GitHub Cloud, GitHub Enterprise, GitLab Cloud, GitLab Enterprise, Bitbucket Cloud y Bitbuket Server), por lo que su cobertura es muy amplia. Si comparamos con el resto de las herramientas vemos que integra alguna menos.

Vemos que tiene el mismo número de métricas que Codebeat y un número bastante inferior que SonarQube que tiene 8.
Hemos tenido problemas con la cobertura, ya que no la exporta de nuestro proyecto, tenemos que configurar varias cosas que no hemos conseguido que nos muestre aún así, por lo que no resulta muy útil el tener que andar configurando para que nos muestre dicha cobertura.

El número de características en bastante inferior a Codebeat y a SonarQube.

Dispone de configuración de reglas para el análisis al igual que las otras dos herramientas.

Nos ofrece una prueba de 14 días con acceso completo a los repositorios públicos y privados, mayor prioridad y análisis más rápido, un soporte prioritario y tableros avanzados, pero pasada esta prueba tenemos un plan gratuito de código abierto que sólo nos da acceso a repositorios públicos.

A diferencia de las otras herramientas con Codacy no podemos exportar los resultados.

Finalmente podemos decir que es una herramienta muy sencilla de utilizar, con varias funciones y alta configuración.
