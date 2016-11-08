# smartmeter.py: extract data from "smart" power-meters

This tool can read the values contained inside Landis+Gyr
power-meters and sends the output to Influxdb. It has been 
tested with the E230 model but I guess that it should work 
with IEC 62056 compliant devices too.

# install

1. Install few dependencies using pip

* pyserial
* influxdb

# configure

You'll have to statically set the Influxdb server IP address +
database settings inside the code for now.

# run

``$ ./smartmeter.py -d /dev/ttyUSB0`` 

* ``-D``:  daemonize

# credits

Joost Baltissen is the author of the inital code

