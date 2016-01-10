############# 
wahhkyahhoverlay
#############

:DEMO URL: https://youtu.be/fMjwVNXyXuQ :

Arduino setup
------------

use arduino/mpu6050.ino

Raspberry Pi 2 setup
---------------------

#. Connect Arduino via USB cable
#. Attach Camera

Fuji setup
~~~~~~~~~~~

to receive MPU-6050 data from Arduino, Fuji is setup using raspi2/mpu.toml

::

	$ fuji-gw -c mpu.toml

Momo start
~~~~~~~~~

Use Anzu account to get client-id and access token.

::

	$ momo-gw -C CLIENT_ID -A ACCESS_TOKEN -H wss://anzu.shiguredo.jp:443/signaling

Browser setup
-------------

Access Anzu site 
~~~~~~~~~~~~~~

:URL: https://anzu.shiguredo.jp/:

Kick Electron application
~~~~~~~~~~~~~~~~~~~~

::

	$ electron .
