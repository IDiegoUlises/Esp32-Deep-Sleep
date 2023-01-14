# Esp32-Deep-Sleep


```c++
void setup()
{
  //Configura el modo sueño y para despertarlo con un high
  esp_sleep_enable_ext0_wakeup(GPIO_NUM_13, HIGH); //High o Low

  //Inicia el modo sueño
  esp_deep_sleep_start();
}

void loop()
{

}
```
