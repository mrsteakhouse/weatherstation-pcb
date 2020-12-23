# Weather station PCB Schematics 

These are the PCB schematics for the weatherstation project.
It is designed to work with an ESP-01 tuned for deep sleep.
The circuit is powered by any 9V power source (6xAA works best).
A linear voltage regulator ([MCP1755S](http://ww1.microchip.com/downloads/en/devicedoc/25160a.pdf)) breaks that 9V down to 3.3V.
The MCU communicates through I2C with the on board voltage sensor ([MCP3421](https://www.microchip.com/wwwproducts/en/en520011)) and an air quality sensor like the [BME-280](https://www.bosch-sensortec.com/products/environmental-sensors/humidity-sensors-bme280/).
Additionaly any other I2C device that runs on 3.3V may be connected through an extra pair of VCC, GND, SCL and SDA.

The implementation can be found [here](https://github.com/mrsteakhouse/weatherstation/tree/main).
