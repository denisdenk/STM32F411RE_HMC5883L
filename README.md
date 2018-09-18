STM32F411RE + HMC5883L
===================

This example includes the code to connect the *HMC5883L* chip to the **STM32F411** microcontroller. The  data is output via the UART interface at 115200 baud.

The code for the microcontroller is written in C using the HAL library from ST in AC6 System Workbench 

The chip is connected as follows:

| HMC5883L PIN  | STM32 PIN 
| :----------- | ----: | 
| VCC          | 3V3   |    
| GND          | GND   |  
| SDA          | PB7   |  
| SCL		       | PB6   |



I used a Nucleo board with this microcontroller, and on this board, the UART interface is connected as follows:

| STM32F411 PIN| UART PIN 
| :----------- | ----: | 
| PA10         | RX    |    
| PA9          | TX    | 

When connecting the microcontroller to the USB-UART (like cp2102 ch340 ft232 etc.) adapter, you should connect the RX of the microcontroller to the TX of the adapter board.
