# ESP32-and-LAMBDA62-LoRA-Module

I struggled to get the LAMBDA62 LoRA module from RF Solutions working with the ESP32. Mostly a skill issue. Below is how I did it.

This will work for Platform.io, likely also work Arduino IDE.

---

I'm not sure where the code was originally from, if you find it, let me know and I'll add a reference.

Connect pins as follows:
~~~
// ESP32 - SX126x pin configuration
PIN_LORA_RESET = 27;	 // LORA RESET
PIN_LORA_NSS = 5;	 // LORA SPI CS
PIN_LORA_SCLK = 18;	 // LORA SPI CLK
PIN_LORA_MISO = 23;	 // LORA SPI MISO > SDO
PIN_LORA_MOSI = 19;	 // LORA SPI MOSI > SDI
PIN_LORA_BUSY = 32;	 // LORA SPI BUSY 
PIN_LORA_DIO_1 = 33; // LORA DIO_1
RADIO_RXEN = 17;	 // LORA ANTENNA RX ENABLE
RADIO_TXEN = 16;	 // LORA ANTENNA TX ENABLE
~~~
