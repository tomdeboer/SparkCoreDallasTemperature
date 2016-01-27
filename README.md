# Particle Dallas Temperature Sensor Library <img src="http://i.imgur.com/BwfHCrI.png" width="180px" align="right" />
>This library is a port of the Arduino Dallas Temperature Sensor library. Some includes have been fixed, but the libary is otherwise untouched.
> Original repository by Miles Burton: [Arduino-Temperature-Control-Library](https://github.com/milesburton/Arduino-Temperature-Control-Library).
> Forked from Tom Deboer: [SparkCoreDallasTemperature](https://github.com/tomdeboer/SparkCoreDallasTemperature).

## Supported Sensors
> This library supports the following devices:
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

## Libraries
- [OneWireSpark](https://github.com/Hotaman/OneWireSpark)

## Example Code

	// Init Dallas on pin digital pin 3
	DallasTemperature dallas(new OneWire(D3));

	void setup(){
		Serial.begin(9600);
		dallas.begin();
	}

	void loop(){
		dallas.requestTemperatures();
	    float celsius = dallas.getTempCByIndex( 0 );
	    Serial.print("Temperature: "); Serial.println(celsius) ;
	}
