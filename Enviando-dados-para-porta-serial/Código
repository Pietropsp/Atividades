int pushButton = 2;  // Defina o pino onde o botão está conectado

void setup() {
  Serial.begin(9600);  // Inicialize a comunicação serial
  pinMode(pushButton, INPUT);  // Configure o pino do botão como entrada
}

void loop() {
  int buttonState = digitalRead(pushButton);  // Leia o estado do botão
  Serial.println(buttonState);  // Imprima o estado do botão no monitor serial
  delay(500);  // Aguarde meio segundo
}
