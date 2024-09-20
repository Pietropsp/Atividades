# Ligar e desligar o LED com o botão


Ao pressionar o botão liga o LED integrado no pino 13 da placa Arduino. O botão é conectado ao pino 2 (ou qualquer outra entrada digital) por um resistor pull-up de 10 kΩ. O resistor pull-up está conectado à terra. O outro contato do botão está conectado a uma fonte de alimentação de 5 V.

Quando o botão não é pressionado, o pino 2 da placa Arduino é conectado à terra por um resistor pull-up, e a entrada será LOW. Quando o botão é pressionado, a entrada digital será de 5V - nível HIGH.

É possível conectar este circuito ao contrário, com um resistor pull-up segurando a entrada HIGH e indo para o nível LOW quando o botão é pressionado. Nesse caso, o comportamento do esboço será invertido: o LED acende e apaga quando o botão é pressionado.

Se você desconectar a entrada digital do resistor, o LED poderá piscar aleatoriamente. Isso ocorre porque a entrada é "flutuante", o que significa que ela retorna aleatoriamente um nível HIGH ou LOW. É por isso que você precisa de um resistor pull-up.

## Peças necessárias :
  *  1 Pushbutton
  *  1 resistor de 10k Ohms
  *  1 resistor de 220 ohms
  *  Led
  *  Fios de conexôes
 ## Esquema de montagem

 * coloque o pushbutton de forma a formar uma ponte etre os dois lados da protoboard
 * conecte o resistor de 10k ohms a um lado do pushbutton e ligue esse resistor ao GND
 * o outro lado deste pushbutton conecte ao pino 2 do arduino
 *  ligue o pushbutton ao VCC usando um pino que está no mesmo lado da protoboard do resistor.
 *  pegue um LED e coloque na protoboard
 *  ligue um resistor de 220 ohms no LED
 *  ligue o LED ao pino 13 do Arduino
 *  ligue o resistor de 220 ohms no GND
