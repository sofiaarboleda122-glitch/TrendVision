# 09 · Matriz de gestión de riesgos

En este documento, el equipo Trendvision identifica y valora los riesgos de implementar en la floricultura un panel de monitoreo que recibe lecturas de sensores de temperatura, humedad ambiente y humedad del suelo por bloque de cultivo, las muestra en tiempo real y envía alertas cuando un valor sale del rango óptimo. La solución se iniciará como un piloto en un solo invernadero, con sensores de bajo costo y herramientas gratuitas. La usarán la administradora, que recibirá alertas y reportes en su celular, y los operarios, que registrarán y consultarán datos durante sus rondas de inspección.

El nivel de cada riesgo es el producto de la probabilidad (P, de 1 a 5) por el impacto (I, de 1 a 5): 1-4 bajo, 5-9 medio, 10-16 alto y 20-25 crítico.

## Matriz de riesgos

| ID | Riesgo | Categoría | P | I | Nivel | Tratamiento | Acción | Responsable | Fecha |
| :-- | :-- | :-- | :-: | :-: | :-: | :-- | :-- | :-: | :-: |
| R1 | Falla de sensores y conectividad: la humedad del invernadero, la señal débil o la caída de energía dejan sin lecturas a uno o más bloques. | Tecnológico | 4 | 4 | 16 (Alto) | Mitigar | Proteger los sensores con carcasas, medir la cobertura de red antes de instalarlos, guardar lecturas en el microcontrolador mientras no haya conexión y avisar cuando un sensor deje de reportar. | PR | 5 de noviembre |
| R2 | Acceso indebido o pérdida de datos del cultivo y de los registros de producción. | Datos y ciberseguridad | 3 | 4 | 12 (Alto) | Mitigar | Usar contraseñas robustas y roles diferenciados (administradora y operarios), conexión cifrada, copias de seguridad automáticas semanales y una prueba de restauración. | PR | 7 de noviembre |
| R3 | Resistencia de los operarios a pasar del papel y el Excel al registro digital. | Personas y adopción | 4 | 3 | 12 (Alto) | Mitigar | Diseñar una pantalla de registro corta y legible desde el celular, hacer una capacitación práctica en el invernadero y acompañar las primeras rondas, con retroalimentación de los operarios. | UX | 10 de noviembre |
| R4 | Sobrecosto frente al presupuesto limitado (sensores, hosting y reposición de equipos). | Financiero | 2 | 2 | 4 (Bajo) | Aceptar | Limitar el piloto a un invernadero, usar sensores de bajo costo y servicios gratuitos, y llevar un registro simple de gastos con un tope definido por el equipo. | LP | 12 de noviembre |
| R5 | Tratamiento de datos personales sin autorización (Ley 1581 de 2012): el sistema guarda nombre, celular o correo de la administradora y los operarios para enviar alertas. | Legal | 2 | 2 | 4 (Bajo) | Evitar | Recoger solo los datos de contacto necesarios, obtener autorización informada de cada usuario, redactar una política de tratamiento breve y no almacenar datos de clientes. | LP | 6 de noviembre |
| R6 | Alertas mal calibradas o ignoradas: umbrales inadecuados generan falsas alarmas o no avisan a tiempo ante plagas, hongos o estrés hídrico. | Operativo | 3 | 4 | 12 (Alto) | Mitigar | Definir los rangos óptimos por tipo de flor con el jefe de cultivo, probarlos con datos reales del piloto, ajustarlos tras la primera semana y establecer quién responde a cada alerta. | AP | 13 de noviembre |

## Riesgos altos y críticos: plan de respuesta

Por ahora no hay riesgos críticos. Los cuatro riesgos altos son los siguientes.

### R1 · Falla de sensores y conectividad (nivel 16)
Es el riesgo más importante, porque sin lecturas confiables el panel pierde su razón de ser y la detección tardía de anomalías sigue ocurriendo. El plan es:
- Revisar la cobertura de red en el invernadero piloto antes de comprar o instalar equipos.
- Instalar los sensores con protección contra la humedad.
- Programar el microcontrolador para guardar las lecturas localmente y enviarlas al recuperar la conexión.
- Configurar una alerta de "sensor sin reportar" para que una falla no pase inadvertida.

### R2 · Acceso indebido o pérdida de datos (nivel 12)
Los datos de temperatura, humedad, riego y producción sustentan las decisiones del cultivo, y perderlos o alterarlos afectaría la trazabilidad. El plan es:
- Asignar permisos por rol, de modo que solo la administradora modifique configuraciones y los operarios registren y consulten.
- Cifrar la comunicación.
- Programar copias de seguridad semanales y verificar que se pueden restaurar.

### R3 · Resistencia de operarios al registro digital (nivel 12)
Hoy los operarios anotan en papel o Excel, y una herramienta que perciban como lenta o complicada terminaría abandonada. El plan es:
- Mantener el registro en pocos pasos y con botones grandes.
- Capacitar en el propio invernadero durante una ronda real.
- Recoger sus comentarios en las primeras semanas del piloto y ajustar la interfaz.

### R6 · Alertas mal calibradas o ignoradas (nivel 12)
Un exceso de falsas alarmas lleva a ignorarlas, y un umbral demasiado amplio deja pasar hongos, plagas o estrés hídrico que dañan la flor de exportación. El plan es:
- Acordar con el jefe de cultivo los rangos óptimos para rosas, claveles y crisantemos.
- Revisar las alertas generadas en la primera semana y recalibrar los umbrales.
- Dejar definido quién atiende cada tipo de alerta.

![Mapa de calor de riesgos](../assets/matriz-riesgos.png)

### Cómo leer el mapa de calor

Cada riesgo aparece en la casilla donde se cruzan dos cosas: qué tan probable es que ocurra, que sube de abajo hacia arriba, y cuánto daño haría si ocurre, que crece de izquierda a derecha. El color acompaña esa lectura y va del verde, donde basta con vigilar, al rojo, donde hay que actuar ya. En nuestro proyecto, lo que queda más arriba y a la derecha es la **Falla de sensores y conectividad**, porque en un invernadero húmedo y con señal irregular es muy probable que fallen lecturas, y sin ellas seguiríamos detectando tarde las plagas y el estrés hídrico. Por eso lo primero que haremos es medir la cobertura de red y proteger los sensores antes de instalarlos. Un escalón más abajo, en la zona naranja, están **Acceso indebido o pérdida de datos**, **Resistencia de operarios al registro digital** y **Alertas mal calibradas o ignoradas**, que atenderemos con roles de acceso, capacitación en el invernadero y ajuste de umbrales con el jefe de cultivo. En verde quedaron **Sobrecosto frente al presupuesto limitado**, porque el piloto de un solo invernadero con equipos económicos acota el gasto, y **Tratamiento de datos sin autorización**, porque solo guardamos datos de contacto de los usuarios y ninguno de clientes; basta con revisarlos en cada avance del proyecto.

## Conclusión

Los mayores riesgos de la solución están en la parte técnica y en el uso diario (sensores, datos, adopción y calibración de alertas), y el piloto en un solo invernadero nos permite controlarlos antes de ampliar.
Los riesgos financiero y legal son bajos gracias al alcance reducido y a que solo se tratan datos de contacto con autorización, y los revisaremos en cada entrega.
