4G HAT para Raspberry Pi, Diseño completo de un HAT compatible con Raspberry Pi que integra comunicaciones celulares 4G/LTE. Hecho especialmente para usar como companion computer en y comunicarse con un PixHawk en un UAV (unmanned aerial vehicle).
Desarrollado como proyecto final para la materia Diseño Avanzado de Circuitos Impresos en la Universidad Nacional de Rosario.
![photo_2026-01-16 08 11 04](https://github.com/user-attachments/assets/b04e4a6f-a7db-4371-9845-dae724024507)
![photo_2026-01-16 08 11 04](https://github.com/user-attachments/assets/92a3a402-e783-482d-ba9c-33df29802437)
Dentro del repositorio se van a encontrar 3 versiones del layout apenas diferentes entre si. Estas iteraciones se hicieron en busqueda de optimizar el espacio y la comodidad de los conectores para el usuario (tener en cuenta que una vez estar montado sobre una Raspberry Pi la cara inferior del HAT no es accesible).

Características

Compatible con estándar Raspberry Pi HAT
Cumple especificaciones mecánicas (65x56mm, mounting holes)
EEPROM de identificación según estándar HAT
Conectores GPIO de 40 pines

Comunicacion UART PixHawk:
Conector JST GH 6 pines para conectar con cable cruzado a GPS2 o TELEM2 del PixHawk Cube Orange. 115200 baudios.

Comunicaciones 4G/LTE:

Módulo celular: SIM7600
Bandas soportadas: [especificar]
Interfaz USB para comandos AT
Conectores SMA/U.FL para antenas externas


Diseño RF de Alta Frecuencia

PCB multicapa: 2 capas (esto fue eleccion adrede como ejercicio academico, porque es mas dificil lograr impedancia controlada con esta distancia entre capas).
Control de impedancia de 50Ω en líneas de RF
Control de impedancia de 90Ω en lineas USB 2.0
Stackup optimizado para señales high-speed
Matching de impedancia en conexiones de antena


Alimentación
Pack de baterias 2S a 9S (de 7V a 35V). Regulador switching para alimentar la Raspberry Pi, segundo regulador switching alimenta el modulo SIM7600.

Tecnologías Utilizadas

Diseño PCB: KiCAD 9
Capas: 2 layers (Ground plane en ambas capas)
Comunicación: USB, UART, SPI, GPIO
Impedancia controlada: 50Ω para trazas RF, 90Ω diferencial para USB

Esquematico principal
<img width="1097" height="761" alt="Captura de pantalla 2026-01-17 a la(s) 10 48 18" src="https://github.com/user-attachments/assets/f137575b-41bd-48ab-bec0-61d080d8c270" />
El esquematico completo puede encontrarse en la carpeta del proyecto.

Estado del Proyecto

-Diseño esquemático completo
-Layout PCB con control de impedancia
-Diseño validado en simulación

Estado actual: Proyecto académico completado (2025). Diseño validado, pendiente fabricación y testing.

Licencia
Proyecto académico - Todos los derechos reservados

Contacto
Rodrigo Maero - r.maero@gmail.com
