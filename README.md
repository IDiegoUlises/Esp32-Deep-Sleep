# Esp32 Deep Sleep Con Activacion Externa

<img src="https://github.com/IDiegoUlises/Esp32-Deep-Sleep/blob/main/Images/ESP32-DOIT-DEVKIT.jpg" width="1000" height="400" />

* Todos los puertos que sean RTC pueden ser utilizados como activacion externa (ext0)

### Codigo
```c++
void setup()
{
  //Configura el modo sueño y para despertarlo con un high en pin el indicado
  esp_sleep_enable_ext0_wakeup(GPIO_NUM_13, HIGH); //High o Low

  //Inicia el modo sueño
  esp_deep_sleep_start();
}

void loop()
{

}
```

![](https://github.com/IDiegoUlises/Esp32-Deep-Sleep/blob/main/Images/Esp32-Deep-Sleep.gif)
