# CFI-Tema-1-Redes
En esta imagen se muestra la red del sistema de videoconferencia que tendría un edificio modelo de la empresa, ajustable para cualquiera de sus tres sedes.  
Las sedes se conectan a través de Internet con el protocolo MPLS. En esta red, la entrada a Internet llega por un primer router Cisco ISR 4331, se filtra por un firewall perimetral Cisco Firepower 2140 que filtrar la mayor parte de los datos, después llega a un switch que conecta con los servidores de correo, proxy, DNS, DHCP, VoIP y web, todos estos servidores están la zona desmilitarizada (DMZ), obteniendo una mayor seguridad.
Inmediatamente de la zona desmilitarizada, se encuentra un firewall interno de la misma marca que filtra los servidores https y otro firewall en paralelo de una marca diferente SonicWall TZ270 menos potente para utilizar en caso puntuales por si una actualización de la marca Cisco u otra cosa vulnerabiliza el firewall.
Seguido de estos firewalls se encuentra la red interna, en la cual se encontrará un switch central que se distribuye la conexión a cada segmento de la sede, como el switch de los servidores archivo, administración, videoconferencia y monitoreo o los switches que conectan con los ordenadores, cámaras, proyectores, altavoces e impresora. En cuanto a la estructura de cableado todo está compuesto de fibra hasta los switches, después a partir de cada switch de cada apartado y sus componentes está compuesto de cable recto ethernet, Cat 6a debido a que el Cat 7 es parecido, pero más costoso.
Dispositivos Utilizados
A continuación, se describe los componentes de la red en detalle, como los routers, firewalls, switches, servidores y el cableado, así como los protocolos de seguridad implementados para proteger y optimizar la transmisión de datos entre las sedes.
Router: Cisco ISR 4331
Se ha seleccionado este modelo ya que gestiona múltiples sucursales, actúa como router de borde MPLS de tal forma que inicia y finaliza las etiquetas MPLS de los paquetes que entran y salen de la red. Además, permite la optimización de tráfico y firewall integrado.
Con precio aproximado entre $2,500 - $3,500 USD, cuenta con las siguientes especificaciones:
o	Mejora la conectividad entres redes y optimiza el tráfico mediante QoS.
o	Facilita una comunicación segura y eficiente con filtrado de tráfico.
o	Se evitan pérdidas de paquetes y latencia.
o	Se facilita la administración y escalabilidad al permitir módulos de expansión.
Switch: Cisco 3650-24PS
Este modelo de swicth se ha seleccionado por su capacidad para manejar altos volúmenes de tráfico, compatibilidad con VLANs y soporte para alimentación PoE+, permitiendo la conexión de dispositivos como teléfonos IP y puntos de acceso Wi-Fi.
Con precio aproximado entre $2,000 - $3,000 USD, cuenta con las siguientes especificaciones:
o	Evita la congestión mejorando la segmentación de tráfico con VLANs. 
o	Permite una mejor gestión del ancho de banda mediante QoS.
o	Evita cuellos de botella en la transmisión de datos.
o	Impide interferencia y latencia de red.
Firewall: Cisco Firepower 2140
Se ha elegido este firewall debido a su alto rendimiento en la inspección de tráfico, su capacidad para detectar amenazas y herramientas de ciberseguridad avanzada. Sumado a esto disponemos del Firewall FortiGate 200F que complementa al Cisco Firepower 2140 brindando una seguridad multicapa, seguridad avanzada, inspección de tráfico y control de amenazas en redes empresariales.
Con precio aproximado entre $41.200 - $48,000 USD para el Cisco Firepower 2140 y $5.000 - $6.300 USD para el Firewall FortiGate 200F, cuenta con las siguientes especificaciones:
•	Proporciona una capa de seguridad perimetral, filtrando tráfico malicioso antes de que llegue a la red interna.
•	Mejora la protección contra ataques de denegación de servicio (DDoS).
•	Protege contra Intrusiones y ataques cibernéticos dirigidos a la infraestructura de la empresa.
•	Se evitan problemas de fuga de información o ataques de malware en las comunicaciones.
Cableado: Cat 6A y Fibra Óptica
El cableado Cat 6A se usa dentro de cada edificio para conectar dispositivos finales a los switches, mientras que la fibra óptica se emplea en enlaces troncales entre pisos y sedes debido a su alta capacidad y baja latencia.
Con precio aproximado entre $0.25 - $1.00 USD por metro para el cableado Cat 6A y $1.00 - $2.00 USD por metro para el cableado de Fibra Óptica, cuenta con:
•	Mejora la velocidad y estabilidad de la red.
•	Reduce la latencia en la transmisión de datos, fundamental para la videoconferencia.
•	Se protege en caso de interferencias electromagnéticas en redes de cobre tradicionales.
•	Se evita pérdida de señal en largas distancias, solucionado con fibra óptica.

