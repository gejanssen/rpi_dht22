Driver for DHT22/AM2302 Temperature and humidity sensors on Raspberry Pi
=======

* Forked from [technion/lol_dht22](https://github.com/technion/lol_dht22)
* Based on [dht11.c](http://ubuntuone.com/6mT9cTREz90BUfvQD1AGNy) (license unknown).
* Requires wiringPi library.

<img src="https://github.com/gejanssen/rpi_dht22/blob/master/dht22.png" align="right" />


Install and Usage
------

    ./configure
    make
    sudo ./rpi_dht22 pin1 [pin2...]
    Pin = 7, Humidity = 55.4 %, Temperature = 16.6 °C


    Or do a :

```
gej@rpi-b ~/rpi_dht22 $ ./read_dht22.sh 
Data not good, skip
Data not good, skip
Pin = 4, Humidity = 43.9 %, Temperature = 19.7 °C
gej@rpi-b ~/rpi_dht22 $
```


License 
-------

Public domain. Do what you want. No warranties.

Options
-------

`./configure` options:
* `--disable-silent-rules` Show the make process (silent by default)
* `--disable-secure` Disable compile with FORTIY_SOURCE and stack-protector (enabled by default)
* `--enable-development` Compile with -g -O0 -Wall. Applies disable-secure automatically

`autogen.sh`: Autoconf boostrap. Development use only.
