# Enviando dados para porta serial 

A porta serial pode ser usada para exibir o estatuto das entradas da placa Arduino. Neste Código , ao pressionar o botão liga o LED integrado no pino 13 da placa Arduino. 

## Esquema de Montagem

* O botão é conectado ao pino 2 (ou qualquer outra entrada digital) por um conector 10kΩ resistor de pull-up. 
* O resistor pull-up está conectado à terra. O outro pino do botão está conectado a uma fonte de alimentação de 5V.
* Abra o Monitor Serial da IDE do arduino para testar o projeto
## Explicação do código 
No programa, na função setup(), primeiro você precisa inicializar a porta serial a 9600 bps entre a placa Arduino e o computador: 
Em seguida, inicialize o pino digital 2, que lerá a saída do botão, como entrada: pinMode(2, INPUT); Quando o botão for pressionado,
a entrada será de 5 V (sinal HIGH), e quando não for pressionado, o pino de entrada será conectado à terra por um resistor (sinal LOW). O estado do botão é enviado para a porta serial.
