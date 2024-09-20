# Contagem de pressionamentos de botão.
Para contar o número de pressionamentos de botão, você precisa descobrir quantas vezes o estado do botão muda de desligado para ligado.

## Esquema de Montagem

* O botão é conectado ao pino 2 (ou qualquer outra entrada digital) por um conector 10kΩ resistor de pull-up. 
* O resistor pull-up está conectado à terra. O outro pino do botão está conectado a uma fonte de alimentação de 5V.
* Abra o Monitor Serial da IDE do arduino para testar o projeto
  ## Explicação do programa
O programa compara o estado atual do botão com o seu estado da última vez no loop principal. Se o estado atual do botão diferir do último estado e for igual a HIGH, a contagem de cliques do botão será incrementada e as informações serão enviadas ao Serial Monitor.
