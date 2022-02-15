# leds_externos_gateway

<b>Para indicador de power</b>
1.Conectar Led a resistencia de 330 ohms a 500ohms.
2.Pin a Posicion 2 de PI
3.Otro Pin a Posicion Tierra disponible

<b>Para indicador de PI corriendo</b>
Agregar este codigo a /boot/config.txt
  dtoverlay=pi3-act-led,gpio=21
  dtparam=act_led_trigger=heartbeat
Conectar Pin a GPIO 21
Conectar otro pin a tierra (deberia estar justo al lado)
