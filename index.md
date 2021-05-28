<p>Bienvenido al Internet de las Cosas.</p>
<p>Para comenzar a utilizar tu ESP32-CAM y encontrar toda la información técnica, te recomendamos las siguientes ligas:</p>
<p>Grupo de Facebook en español sobre Internet de las Cosas:<br>
<a href="https://www.facebook.com/groups/724628401049648/">https://www.facebook.com/groups/724628401049648/</a></p>
<ul>
<li>Información específica sobre el ESP32 CAM:</li>
</ul>
<p>Cómo instalar la cámara en el módulo:<br>
Dependiendo del lote, puede venir separada la cámara en el módulo. La instalación es un proceso muy simple, la cámara usa un conector "tipo bisagra".  El siguiente video muestra cómo conectarla.<br>
<a href="https://www.youtube.com/watch?v=olSRkJEkUCU&ab_channel=CosismoIoT">https://www.youtube.com/watch?v=olSRkJEkUCU&ab_channel=CosismoIoT</a></p>
<p>Video de cómo configurar la cámara (Inglés):<br>
ESP32-CAM Video Streaming and Face Recognition with Arduino IDE<br>
<a href="https://www.youtube.com/watch?v=MicAM_A0_lU">https://www.youtube.com/watch?v=MicAM_A0_lU</a></p>
<p>Tutorial escrito del video anterior:<br>
<a href="https://randomnerdtutorials.com/esp32-cam-video-streaming-face-recognition-arduino-ide/">https://randomnerdtutorials.com/esp32-cam-video-streaming-face-recognition-arduino-ide/</a></p>
<p>Esta placa no cuenta con un LED de energía, por lo que cuando lo conectes no verás que encienda ninguna luz para indicar que está energizada. Tiene dos LEDs, ambos programables por software. Uno es de uso general y el otro hace las veces de "Flash" para la cámara.</p>
<p>Cuando se está programando, es necesario conectar IO0 a tierra, antes de energizar,  para entrar en modo boot.</p>
<p>El voltaje de los puertos ( y de los pines TX, RX de la UART) es de 3.3v, aunque la tarjeta tiene un pin para alimentarse con 5V. 
ASEGÚRATE QUE TU CONVERTIDOR USB-TTL ESTÉ CONFIGURADO CON 3.3V EN LOS PUERTOS DE COMUNICACIÓN (LÓGICA 3.3V). En muchos convertidores se cambia el voltaje a la lógica de 3.3v con un jumper. En caso que uses el convertidor usb-ttl ch340, sigue exactamente el diagrama de la parte de abajo con el jumper amarillo colocado como se indica y quedará configurado en 3.3v. Para otros convertidores consulta el manual del fabricante para saber cómo configurar a lógica 3.3v (generalmente con un jumper o a veces a través de soldadura). BAJO NINGUNA CIRCUNSTANCIA USES UN CONVERTIDOR CON SALIDAS 5V FIJAS (COMO ALGUNOS PL2303, QUE NO TIENEN FORMA DE SELECCIONAR EL VOLTAJE). SI USAS LÓGICA  5V, PROBABLEMENTE TE MARCARÁ UN ERROR O ALGUNA VEZ FUNCIONARÁ, PERO EL MÓDULO NO ESTÁ DISEÑADA PARA TOLERAR ESTO Y <strong>EVENTUALMENTE DAÑARÁS IRREVERSIBLEMENTE LA PLACA</strong></p>

Diagrama de conexiones:  

![esp32camCh340g](https://raw.githubusercontent.com/cosismo/esp32-cam/master/esp32ToCh340g.png)  

<p>Hoja de especificaciones técnicas:<br>
<a href="https://drive.google.com/file/d/11m5DbaZ4C7bbMHccGwkEZLNfd2bzMjy7/view?usp=sharing">https://drive.google.com/file/d/11m5DbaZ4C7bbMHccGwkEZLNfd2bzMjy7/view?usp=sharing</a></p>
<p>Ejemplos de cientos de proyectos para la ESP32-CAM en Github<br>
<a href="https://github.com/search?o=desc&q=esp32-cam&s=stars&type=Repositories">  https://github.com/search?o=desc&q=esp32-cam&s=stars&type=Repositories
</a>

<ul>
<li>Información general sobre el ESP32:</li>
</ul>
<p>Libro electrónico sobre el ESP32:<br>
<a href="https://drive.google.com/file/d/11-IH-38VJOXbFJ1ybB1i2Cvcl9n3pSTU/view">https://drive.google.com/file/d/11-IH-38VJOXbFJ1ybB1i2Cvcl9n3pSTU/view</a></p>
<p>Listas con decenas de videos con ejemplos y código de proyectos con ESP32:<br>
Tutoriales básicos en español:<br>
<a href="https://www.youtube.com/playlist?list=PL2xmtLUbEugnUoLiRTqwCm5wi2MSzsw3D">https://www.youtube.com/playlist?list=PL2xmtLUbEugnUoLiRTqwCm5wi2MSzsw3D</a><br>
Inglés:<br>
<a href="https://www.youtube.com/watch?v=rP9p0MzxSos&amp;list=PLxJ8_KSR8bp5-F4HVG4QOm4Kt6wQhzsjU">https://www.youtube.com/watch?v=rP9p0MzxSos&amp;list=PLxJ8_KSR8bp5-F4HVG4QOm4Kt6wQhzsjU</a><br>
<a href="https://www.youtube.com/watch?v=jhjZZkKupk8&amp;list=PL3XBzmAj53RnZPeWe799F-uoXERBldhn9">https://www.youtube.com/watch?v=jhjZZkKupk8&amp;list=PL3XBzmAj53RnZPeWe799F-uoXERBldhn9</a></p>
<p>Información oficial del fabricante del chip:<br>
<a href="https://espressif.com/en/producttype/esp-wroom-32">https://espressif.com/en/producttype/esp-wroom-32</a></p>
<p>Librerías oficiales Arduino:<br>
<a href="https://github.com/espressif/arduino-esp32">https://github.com/espressif/arduino-esp32</a></p>
<p>Foro y mucha información:<br>
<a href="https://esp32.com/">https://esp32.com/</a></p>
<p>Quedamos a tus órdenes por esta vía.</p>
<p>¡Suerte!<br>
Equipo Cosismo</p>
