# leds_externos_gateway

<b>Para indicador de power</b><br>
1. Conectar Led a resistencia de 330 ohms a 500ohms.<br>
2. En raspberry
    Pin 6 - positivo de led<br>
    Pin 8 u otro Pin a Posicion Tierra disponible<br>
5. Agregar en /boot/config.txt<br>
      enable_uart=1<br>

<b>Para indicador de PI corriendo</b><br>
1. Agregar este codigo a /boot/config.txt<br>
  dtoverlay=pi3-act-led,gpio=21<br>
  dtparam=act_led_trigger=heartbeat<br>
2. Conectar Pin a GPIO 21<br>
3. Conectar otro pin a tierra (deberia estar justo al lado)
