Spark Core compatible Dallas Temperature sensor library
===

This library is a port of the original Arduino compatible Dallas Sensor library. Some includes have been fixed, but the libary is otherwise untouched.

_**Note:** This library depends on the OneWire library._

Original repository by Miles Burton: [Arduino-Temperature-Control-Library](https://github.com/milesburton/Arduino-Temperature-Control-Library).
  
## Getting Started
> This library supports the following devices :
> 
> 
> * DS18B20
> * DS18S20 - Please note there appears to be an issue with this series.
> * DS1822
> * DS1820
>
>
> You will need a pull-up resistor of about 5 KOhm between the 1-Wire data line
> and your 5V power. If you are using the DS18B20, ground pins 1 and 3. The
> centre pin is the data line '1-wire'.