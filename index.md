Bienvenido al Internet de las Cosas.

Para comenzar a utilizar tu ESP32-CAM y encontrar toda la información técnica, te recomendamos las siguientes ligas:

Grupo de Facebook en español sobre Internet de las Cosas:  
[https://www.facebook.com/groups/724628401049648/](https://www.facebook.com/groups/724628401049648/)

*   Información específica sobre el ESP32 CAM:

Cómo instalar la cámara en el módulo:  
Dependiendo del lote, puede venir separada la cámara en el módulo. La instalación es un proceso muy simple, la cámara usa un conector "tipo bisagra". El siguiente video muestra cómo conectarla.  
[https://www.youtube.com/watch?v=olSRkJEkUCU&ab\_channel=CosismoIoT](https://www.youtube.com/watch?v=olSRkJEkUCU&ab_channel=CosismoIoT)

*   **Información para convertidor/programador ESP32-CAM-MB**
![ESP32 CAM MB](https://raw.githubusercontent.com/cosismo/esp32-cam/master/ESP32-CAM-MB.png)

Tutorial para usar la cámara con el programador ESP32-CAM-MB (Inglés):  
[https://randomnerdtutorials.com/upload-code-esp32-cam-mb-usb/](https://randomnerdtutorials.com/upload-code-esp32-cam-mb-usb/)

*   **Información para convertidor convencional USB a TTL**

Video de cómo configurar la cámara con un convertidor USB a TTL convencional(Inglés):  
ESP32-CAM Video Streaming and Face Recognition with Arduino IDE  
[https://www.youtube.com/watch?v=MicAM\_A0\_lU](https://www.youtube.com/watch?v=MicAM_A0_lU)

Tutorial escrito del video anterior:  
[https://randomnerdtutorials.com/esp32-cam-video-streaming-face-recognition-arduino-ide/](https://randomnerdtutorials.com/esp32-cam-video-streaming-face-recognition-arduino-ide/)

Esta placa no cuenta con un LED de energía, por lo que cuando lo conectes no verás que encienda ninguna luz para indicar que está energizada. Tiene dos LEDs, ambos programables por software. Uno es de uso general y el otro hace las veces de "Flash" para la cámara.

Cuando se está programando, es necesario conectar IO0 a tierra, antes de energizar, para entrar en modo boot.

El voltaje de los puertos ( y de los pines TX, RX de la UART) es de 3.3v, aunque la tarjeta tiene un pin para alimentarse con 5V. ASEGÚRATE QUE TU CONVERTIDOR USB-TTL ESTÉ CONFIGURADO CON 3.3V EN LOS PUERTOS DE COMUNICACIÓN (LÓGICA 3.3V). En muchos convertidores se cambia el voltaje a la lógica de 3.3v con un jumper. En caso que uses el convertidor usb-ttl ch340, sigue exactamente el diagrama de la parte de abajo con el jumper amarillo colocado como se indica y quedará configurado en 3.3v. Para otros convertidores consulta el manual del fabricante para saber cómo configurar a lógica 3.3v (generalmente con un jumper o a veces a través de soldadura). BAJO NINGUNA CIRCUNSTANCIA USES UN CONVERTIDOR CON SALIDAS 5V FIJAS (COMO ALGUNOS PL2303, QUE NO TIENEN FORMA DE SELECCIONAR EL VOLTAJE). SI USAS LÓGICA 5V, PROBABLEMENTE TE MARCARÁ UN ERROR O ALGUNA VEZ FUNCIONARÁ, PERO EL MÓDULO NO ESTÁ DISEÑADA PARA TOLERAR ESTO Y **EVENTUALMENTE DAÑARÁS IRREVERSIBLEMENTE LA PLACA**

Diagrama de conexiones: ![esp32camCh340g](https://raw.githubusercontent.com/cosismo/esp32-cam/master/esp32ToCh340gv2.png)

Hoja de especificaciones técnicas:  
[https://drive.google.com/file/d/11m5DbaZ4C7bbMHccGwkEZLNfd2bzMjy7/view?usp=sharing](https://drive.google.com/file/d/11m5DbaZ4C7bbMHccGwkEZLNfd2bzMjy7/view?usp=sharing)

Ejemplos de cientos de proyectos para la ESP32-CAM en Github  
[https://github.com/search?o=desc&q=esp32-cam&s=stars&type=Repositories](https://github.com/search?o=desc&q=esp32-cam&s=stars&type=Repositories)

*   Información general sobre el ESP32:

Libro electrónico sobre el ESP32:  
[https://drive.google.com/file/d/11-IH-38VJOXbFJ1ybB1i2Cvcl9n3pSTU/view](https://drive.google.com/file/d/11-IH-38VJOXbFJ1ybB1i2Cvcl9n3pSTU/view)

Listas con decenas de videos con ejemplos y código de proyectos con ESP32:  
Tutoriales básicos en español:  
[https://www.youtube.com/playlist?list=PL2xmtLUbEugnUoLiRTqwCm5wi2MSzsw3D](https://www.youtube.com/playlist?list=PL2xmtLUbEugnUoLiRTqwCm5wi2MSzsw3D)  
Inglés:  
[https://www.youtube.com/watch?v=rP9p0MzxSos&list=PLxJ8\_KSR8bp5-F4HVG4QOm4Kt6wQhzsjU](https://www.youtube.com/watch?v=rP9p0MzxSos&list=PLxJ8_KSR8bp5-F4HVG4QOm4Kt6wQhzsjU)  
[https://www.youtube.com/watch?v=jhjZZkKupk8&list=PL3XBzmAj53RnZPeWe799F-uoXERBldhn9](https://www.youtube.com/watch?v=jhjZZkKupk8&list=PL3XBzmAj53RnZPeWe799F-uoXERBldhn9)

Información oficial del fabricante del chip:  
[https://espressif.com/en/producttype/esp-wroom-32](https://espressif.com/en/producttype/esp-wroom-32)

Librerías oficiales Arduino:  
[https://github.com/espressif/arduino-esp32](https://github.com/espressif/arduino-esp32)

Foro y mucha información:  
[https://esp32.com/](https://esp32.com/)

Quedamos a tus órdenes por esta vía.

¡Suerte!  
Equipo Cosismo
