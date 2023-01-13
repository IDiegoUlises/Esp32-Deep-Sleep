# Esp32-Deep-Sleep

code

void setup() {
  Serial.begin(9600);

  Serial.println("Estoy despierto");
  esp_sleep_enable_ext0_wakeup(GPIO_NUM_15, 1); //1 = High, 0 = Low

  Serial.println("A dormir........................ ");
  esp_deep_sleep_start();
  Serial.println("Esto nunca se imprime");
}

void loop() {
  // put your main code here, to run repeatedly:

}
