dcc-05v2-britetank
------------------

Firmware for temperature and pressure sensor.


Pressure Sensor
---------------

The pressure sensor is a 1/8" NPT stainless sensor:

 * Input: 5V
 * Range: 0-60 psi.
 * Output: 0.5V – 4.5V linear voltage output. 0 psi outputs 0.5V, 30 psi outputs 2.5V, 60 psi outputs 4.5V.

Since the ESP8266 has a 0-1V ADC, I've added a 2:1 voltage divider using two 4.7K resistors, so the effective range is:

```
 0.0psi = 0.25V
 7.5psi = 0.50V
15.0psi = 0.75V
22.5psi = 1.00V
```
