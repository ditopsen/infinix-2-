DOCUMENTACIÓN: The Space In Yours 

The Space Is Yours sitúa al jugador en la piel de [Nombre del Protagonista], un piloto e ingeniero de carga civil que cruza el  Zeta-9 transportando suministros estandarizados. Sin previo aviso, una descomunal tormenta de radiación cósmica desactiva los escudos y colapsa el núcleo de navegación de su nave, la Astraea-7. Sin control de los propulsores, la nave se precipita en picada hacia la atmósfera de Uranus-4, un planeta remoto, salvaje y completamente fuera de las rutas comerciales conocidas.
[Nombre del Protagonista] logra eyectarse en una cápsula de emergencia segundos antes de la colisión. Al despertar, se encuentra aislado en un entorno hostil donde el aire apenas es respirable, los restos de su nave están esparcidos a kilómetros de distancia y la fauna local no se asemeja a nada registrado en los manuales de la Federación.


Módulo 1: Sistema de Supervivencia (Alimento y Vida)
  	Funcionalidad: Gestión de hambre, salud y recolección de recursos comestibles en el planeta desconocido.

Requisitos:
El jugador debe contar con una barra de salud y una barra de hambre visibles en la interfaz (UI).
La barra de hambre debe disminuir gradualmente con el tiempo y acelerarse si el jugador corre o realiza acciones de combate.
El mapa debe generar aleatoriamente flora o fauna comestible interactuable que el jugador pueda recolectar al presionar una tecla de acción.
Consumir un alimento debe restaurar una cantidad específica de la barra de salud y/o hambre.
Si la barra de hambre llega a cero, el jugador comenzará a perder salud progresivamente hasta morir.
Objetivo: Mantener al jugador en un estado constante de alerta y gestión de recursos básicos para asegurar su supervivencia en el entorno hostil.
Responsable: Carol (Gameplay Programmer / Systems Programmer)
Prueba: Alejandra (QA / Test Engineer)
Módulo 2: Sistema de Armamento y Combate
Funcionalidad: Recolección, equipamiento y uso de armas para defenderse de los peligros del planeta.
Requisitos:
El jugador debe poder encontrar y equipar armas dispersas por el mapa o en los restos de la nave estrellada.
Debe existir un sistema de inventario básico para cambiar entre armas o munición.
Al hacer clic izquierdo (o botón de ataque), el personaje debe disparar un proyectil o realizar un ataque cuerpo a cuerpo que inflinja daño a los enemigos.
Los monstruos deben tener una barra de vida propia y reaccionar al recibir daño (por ejemplo, reproduciendo una animación de impacto o muriendo al llegar a 0).
Objetivo: Proveer al jugador de los medios necesarios para defenderse, enfrentar las amenazas del planeta y despejar zonas de exploración.
Responsable: Carol (Gameplay Programmer / Systems Programmer)
Prueba: Alejandra (QA / Test Engineer)
Módulo 3: Investigación y Resolución de Escape
Funcionalidad: Búsqueda de pistas, escaneo de tecnología alienígena y ensamblaje de piezas para reparar la nave o construir un método de salida.
Requisitos:
El jugador debe poder interactuar con restos tecnológicos de su nave o ruinas alienígenas para obtener "datos de investigación" o componentes clave.
Se debe incluir un diario o registro de misiones en el menú que indique el progreso de la investigación y las piezas faltantes.
Al recolectar todos los elementos necesarios (por ejemplo: motor cuántico, combustible alienígena, circuito de navegación), se habilitará una estación de crafteo o la consola principal de la nave para activar la secuencia final.
Objetivo: Darle un propósito narrativo y una condición de victoria clara al equipo y al jugador, guiando la exploración del planeta.
Responsable: Carol (Systems Programmer) y Alejandra (Technical Documentation)
Prueba: Alejandra (QA / Test Engineer)
Módulo 4: Inteligencia Artificial de Enemigos (Monstruos)
Funcionalidad: Comportamiento de patrullaje, detección, persecución y ataque de las criaturas hostiles del planeta.
Requisitos:
Los monstruos deben patrullar una zona asignada o mantenerse en reposo hasta que el jugador entre en su radio de visión/audición (Agro Range).
Al detectar al jugador, el monstruo debe cambiar su estado a "Persecución" y moverse hacia la posición del personaje.
Si el monstruo entra en rango cuerpo a cuerpo, debe ejecutar una animación de ataque que reduzca la salud del jugador.
Objetivo: Crear una amenaza dinámica y desafiante que obligue al jugador a decidir entre el combate directo o el sigilo.
Responsable: Ximena (AI Programmer)
Prueba: Alejandra (QA / Test Engineer)
Módulo 5: Infraestructura, Herramientas y Compilación (Soporte Técnico)
Funcionalidad: Automatización de procesos de compilación, gestión del flujo de trabajo y creación de herramientas internas de desarrollo.
Requisitos:
Configurar pipelines o procesos para empaquetar versiones ejecutables del juego estables (Builds).
Proveer herramientas internas de apoyo para que el equipo pueda testear mecánicas rápidamente (por ejemplo, comandos de consola para spawnear ítems o curar al personaje).
Objetivo: Asegurar que el equipo tenga un entorno técnico optimizado y que las versiones del juego se integren sin errores críticos.
Responsable: Ximena (Tools Programmer / Build & Integration Programmer)
Prueba: Alejandra (QA / Test Engineer)
Fases de la Historia
El Despertar y la Supervivencia Inmediata: El protagonista emerge de los escombros de su cápsula en medio de una densa selva alienígena cubierta por neblina y vegetación bioluminiscente. Sin comunicación ni soporte vital estable, su prioridad es subsistir identificando flora y fauna comestible, y recolectando chatarra para fabricar herramientas rudimentarias mientras detecta las primeras señales de fauna hostil.
La Investigación y el Descubrimiento: Rastrea los restos de la Astraea-7, encontrando el fuselaje destrozado con una computadora central aún operativa para escaneos. Al investigar ruinas alienígenas semisepultadas, descubre que el planeta albergó tecnología capaz de manipular el espacio-tiempo. Conforme se adentra en el territorio por componentes tecnológicos, los monstruos se vuelven más peligrosos, obligándolo a mejorar su arsenal.
El Clímax y el Escape: Con los datos decodificados y las piezas alienígenas recolectadas, repara y modifica la consola de comunicaciones para construir un núcleo de salto provisional. La sobrecarga de energía generada atrae a depredadores alfa en una horda masiva. Después de resistir el ataque utilizando todo su armamento y trampas, la cápsula se dispara hacia la órbita, permitiéndole escapar con los secretos de una civilización olvidada.
Jugabilidad Especificada a Detalle
Bucle de Juego (Core Gameplay Loop): El juego combina la exploración de un entorno hostil bidimensional o tridimensional ligero con la gestión constante de recursos críticos (hambre y salud). El jugador explora el mapa de Akelarre-4, recolecta materiales, combate contra monstruos alienígenas para asegurar su supervivencia, y reúne pistas tecnológicas que le permiten avanzar en la misión de reparación de la nave.
Gestión de Estadísticas y Supervivencia: El jugador monitorea constantemente una interfaz en pantalla que muestra la salud y el hambre. El movimiento activo incrementa el metabolismo del personaje, vaciando más rápido el medidor de hambre y exigiendo el consumo estratégico de alimentos recolectados.
Control y Combate Activo: El sistema de control permite el desplazamiento fluido con el teclado y el ratón, con opciones de movimiento, salto, interacción con objetos del entorno mediante colisiones y selección rápida de armas. Los ataques requieren puntería y sincronización para evitar el daño de los enemigos dotados de inteligencia artificial reactiva.
Progresión y Criterio de Victoria: La jugabilidad transiciona desde una etapa de vulnerabilidad extrema (huir y sobrevivir con herramientas básicas) hasta una fase de enfrentamiento táctico y defensa de posición durante el clímax de activación de la consola de escape.
Plataforma, Lenguaje, Motor y Entorno
Plataforma: PC / Escritorio (Windows / Multiplataforma).
Lenguaje de Programación: Python.
Motor / Framework de Programación: Pygame (ideal para desarrollo en 2D con control total de bucles de juego, físicas, renderizado y colisiones) o Ursina Engine (en caso de optar por un entorno 3D simplificado basado en Python).
Entorno Específico: Entorno de desarrollo como Visual Studio Code o PyCharm, intérprete de Python instalado, control de versiones con Git/GitHub para la integración continua de los módulos de Carol, Ximena y Alejandra, y librerías complementarias (como NumPy para cálculos vectoriales de la IA si es necesario).
