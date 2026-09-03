# Los-completitos
Propuesta N.° 1
Nombre del proyecto: Park Aviso (Sistema de proximidad para estacionamiento del personal)

Problema o necesidad: Los vehículos del personal e inspectores tienen problemas de visibilidad al estacionarse cerca de muros bajos o zonas peatonales del liceo, arriesgando colisiones menores.

Aplicación: Estacionamiento o zona de carga y descarga del liceo.

Funcionamiento: El sensor ultrasónico mide continuamente la distancia al vehículo entrante. Si la distancia es segura, activa un LED verde; si el auto se acerca demasiado a la pared, interrumpe la luz verde, enciende un LED rojo y activa un zumbador con pitidos intermitentes para alertar al conductor.

Arduino: Arduino UNO.

Sensores: Sensor ultrasónico HC-SR04.

Actuadores: 1 LED verde, 1 LED rojo y 1 Zumbador (buzzer).

Otros componentes: 2 Resistencias de 220 ohms, Placa de pruebas (breadboard), Cables Jumper.

Materiales: Caja plástica de protección, soporte para fijar a la pared del estacionamiento.

Programación: Lectura digital y cálculo de tiempo del eco en el HC-SR04 para convertirlo a centímetros. Estructura if/else para evaluar los rangos de distancia y activar los pines de los LEDs y el zumbador mediante señales PWM o digitales.

Viabilidad: Muy alta. Los componentes son de bajo costo, fácil acceso y rápida simulación en Tinkercad.

Propuesta N.° 2
Nombre del proyecto: BioClima Liceo (Monitor ambiental para laboratorio)

Problema o necesidad: La falta de control de temperatura y humedad en el laboratorio de ciencias o huerto escolar provoca el deterioro de cultivos o reactivos.

Aplicación: Invernadero escolar, huerto o laboratorio de ciencias.

Funcionamiento: El sensor lee las condiciones ambientales en tiempo real y las despliega en la pantalla LCD. Si la temperatura supera el límite recomendado para las plantas, el sistema enciende un LED de advertencia y activa un zumbador de alerta.

Arduino: Arduino UNO.

Sensores: Sensor de temperatura y humedad DHT11.

Actuadores: Pantalla LCD 16x2 (I2C), 1 LED de alerta, Zumbador.

Otros componentes: Potenciómetro (para contraste de pantalla si no usa I2C), Resistencia de 220 ohms, Cables Jumper, Breadboard.

Materiales: Maqueta pequeña de invernadero o base para fijación en pared.

Programación: Uso de librería para el sensor DHT11 e inclusión de condicionales if/else para comprobar si la temperatura rebasa el límite fijado, enviando señales a la pantalla y activando la alarma sonora/luminosa.

Viabilidad: Alta. Requiere verificar librerías de temperatura en la simulación.

Propuesta N.° 3
Nombre del proyecto: EcoLuz Aula (Luz de seguridad y ahorro energético)

Problema o necesidad: Alto consumo eléctrico por luces que quedan encendidas en pasillos o salas cuando hay suficiente luz natural o cuando oscurece de golpe.

Aplicación: Pasillos, salas de clases o bodega de materiales del liceo.

Funcionamiento: Una fotorresistencia (LDR) detecta los niveles de luz natural. Al bajar la luminosidad ambiental, el sistema enciende un LED RGB en un tono cálido para iluminar la zona y activa una pantalla que muestra el estado ("Luz Encendida"). Un potenciómetro permite ajustar manualmente el umbral de oscurecimiento.

Arduino: Arduino UNO.

Sensores: Fotorresistencia (LDR).

Actuadores: 1 LED RGB, Pantalla LCD 16x2.

Otros componentes: 2 Potenciómetro de 10 kilo ohms, (para divisor de tensión LDR), 3 Resistencias de 220 ohms (para el LED RGB), Breadboard, Cables Jumper.

Materiales: Soporte de cartón piedra o acrílico para simular una maqueta de aula.

Programación: Lectura analógica del pin del LDR y del potenciómetro (analogRead()). Comparación mediante if/else para activar las salidas PWM del LED RGB según el nivel de oscuridad.

Viabilidad: Alta. Ideal para demostrar conceptos de automatización y ahorro energético.

Propuesta N.° 4
Nombre del proyecto: RetoReflejos (Plataforma de pausas activas para el recreo)

Problema o necesidad: Falta de actividades recreativas, dinámicas y de estimulación psicomotriz para los estudiantes durante los recreos.

Aplicación: Patio del liceo, zona de juegos o sala de estar de estudiantes.

Funcionamiento: Un LED principal se enciende de manera aleatoria. Dos estudiantes compiten por presionar su respectivo pulsador primero. El sistema detecta quién fue más rápido, enciende el LED asignado al ganador y emite un tono musical festivo mediante un zumbador.

Arduino: Arduino UNO.

Sensores / Entradas: 2 Pulsadores (Push buttons).

Actuadores: 1 LED central, 2 LEDs de victoria (verde y azul), 1 Zumbador.

Otros componentes: 2 Resistencias de 10 kilo ohms (Pull-down), 3 Resistencias de 220 ohms, Breadboard, Cables Jumper.

Materiales: Tablero de madera o cartón prensado para montar los pulsadores y LEDs de forma resistente.

Programación: Uso de funciones de tiempo (millis() o delay()) y generación de tiempo aleatorio con random(). Evaluación de cuál pulsador cambia de estado lógico primero utilizando estructuras if/else.

Viabilidad: Alta. Es un proyecto interactivo y divertido muy fácil de probar en Tinkercad.

Propuesta N.° 5
Nombre del proyecto: MorseKey (Sistema de control de acceso por código para el laboratorio)

Problema o necesidad: Ingreso no autorizado a salas especiales (laboratorio de computación, bodegas o pañol) que requiere un control sencillo sin llaves físicas.

Aplicación: Puertas de acceso a laboratorios, pañol o sala de profesores.

Funcionamiento: El usuario introduce una clave mediante 2 pulsadores (uno para "puntos" y otro para "rayas"). El sistema da retroalimentación sonora con un zumbador al presionar cada botón. Si la secuencia ingresada es correcta, se activa un LED verde (simulando apertura de puerta); si es errónea, se enciende un LED rojo de rechazo.

Arduino: Arduino UNO.

Sensores / Entradas: 2 Pulsadores.

Actuadores: 1 LED verde, 1 LED rojo, 1 Zumbador.

Otros componentes: 2 Resistencias de 10 kilo ohms, 2 Resistencias de 220 ohms, Breadboard, Cables Jumper.

Materiales: Maqueta de puerta pequeña o marco decorativo para la demostración.

Programación: Registro de lecturas digitales en variables o arreglos (arrays). Uso de bucles for o estructuras if/else anidadas para verificar la secuencia ingresada frente a la clave almacenada.

Viabilidad: Muy alta. Permite demostrar un alto nivel de lógica de programación con componentes sencillos y accesibles.

