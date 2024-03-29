![ESP32 CAM](https://raw.githubusercontent.com/cosismo/esp32-cam/master/ESP32-CAM-versions.png)  
  
  
Bienvenido al Internet de las Cosas.

Para comenzar a utilizar tu ESP32-CAM y encontrar toda la información técnica, te recomendamos las siguientes ligas:

Grupo de Facebook en español sobre Internet de las Cosas:  
[https://www.facebook.com/groups/724628401049648/](https://www.facebook.com/groups/724628401049648/)

**Información específica sobre el ESP32 CAM:**

*  Cómo instalar la cámara en el módulo:  
Dependiendo del lote, puede venir separada la cámara en el módulo. La instalación es un proceso muy simple, la cámara usa un conector "tipo bisagra". El siguiente video muestra cómo conectarla.  
[https://www.youtube.com/watch?v=olSRkJEkUCU&ab\_channel=CosismoIoT](https://www.youtube.com/watch?v=olSRkJEkUCU&ab_channel=CosismoIoT)

*   Protip: para cargar el sketch / bin a tu ESP32:  
1) Presiona y deja presionado el botón "boot" (también conocido como "load" o "download").  
2) Sin soltar el botón "boot", presiona y suelta el botón "reset".  
3) Sube el sketch desde el Arduino IDE, siempre dejando presionado el botón "boot".  
  
Si no sigues el procedimiento probablemente no puedas cargar el sketch y se te presentarán errores de timeout o como los que se describen en este post:  
[https://github.com/espressif/arduino-esp32/issues/1253](https://github.com/espressif/arduino-esp32/issues/1253) 

*   Programación básica
Existen dos modelos de la esp32cam, con convertidor incluído y con convertidor separado. Dependiendo del modelo, la apariencia física es diferente, pero las instrucciones son básicamente las mismas.  
En el Arduino IDE:  
1) Instala las librerías de ESP32 Arduino con el método de json en preferencias. [Instalar ESP32 en Arduino IDE](https://randomnerdtutorials.com/installing-the-esp32-board-in-arduino-ide-windows-instructions/)  
2) Selecciona el modelo AI-Thinker ESP32-CAM.  
3) Modifica el código agregando las credenciales de tu red WiFi al ejemplo.  
4) Sube el ejemplo: ESP32 > Camera > CameraWebServer.  

*   Esta placa no cuenta con un LED de energía, por lo que cuando lo conectes no verás que encienda ninguna luz para indicar que está energizada. Tiene dos LEDs, ambos programables por software. Uno es de uso general y el otro hace las veces de "Flash" para la cámara.

*   Puedes seguir cualquier tutorial del modelo viejo en el que se tenía que cablear el convertidor usb a la cámara, sólo ignora los pasos de puentear los cables y usa el método de presionar "boot" y "reset" para subir el sketch que se menciona arriba.

[Tutorial en inglés (página + video)](https://randomnerdtutorials.com/esp32-cam-video-streaming-face-recognition-arduino-ide/)  

[Tutorial en español (video)](https://www.youtube.com/watch?v=WBJrXUy2HEw)  

*   Drivers USB
[Drivers Windows, Mac, Linux CH340G](https://www.geekfactory.mx/tutoriales-arduino/driver-ch340-para-arduino-chinos-o-genericos/)

*   Hoja de especificaciones técnicas:  
[https://drive.google.com/file/d/11m5DbaZ4C7bbMHccGwkEZLNfd2bzMjy7/view?usp=sharing](https://drive.google.com/file/d/11m5DbaZ4C7bbMHccGwkEZLNfd2bzMjy7/view?usp=sharing)

*   Ejemplos de cientos de proyectos para la ESP32-CAM en Github  
[https://github.com/search?o=desc&q=esp32-cam&s=stars&type=Repositories](https://github.com/search?o=desc&q=esp32-cam&s=stars&type=Repositories)

**Información general sobre el ESP32:**

* **LIBRO ELECTRÓNICO**.
### Descargar libro electrónico PDF
[Libro electrónico sobre el ESP32](https://drive.google.com/file/d/11-IH-38VJOXbFJ1ybB1i2Cvcl9n3pSTU/view)  
[Otro Libro](https://archive.org/details/foo_20210223)

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

**Problemas conocidos**
*   "Basura" en el serial.  Si bien un error en el baudrate puede ocasionar que recibas caracteres erróneos en el monitor serial del Arduino IDE, si estás seguro de que está configurado correctamente, quizá tengas un problema de energía. Esto es causado porque el voltaje del serial cae a niveles bajos y no puede ser leído por la laptop. Puedes hacer una prueba de cargar un sketch que consuma menos energía como el ejemplo esp32 / chipID para verificar que si funciona el serial a bajo consumo de corriente.  
Este modelo consume más energía que los anteriores por usar el chip ESP32 + CH340G + Cámara, y puede ser que no funcione con la corriente de tu puerto USB, por lo que tendrás que alimentarlo externamente. 
Puedes alimentar la placa a través de sus pines (5v + GND) con una fuente externa mientras está conectado a tu laptop, puedes usar un hub usb alimentado externamente o puedes conectarlo directamente a un cargador USB de celular. 
Para encontrar su IP, puedes buscarla en tu router o usar un escáner de red. 


Quedamos a tus órdenes por esta vía.

¡Suerte!  
Equipo Cosismo
