Follow the steps in the below link:
https://github.com/plerup/makeEspArduino

Follow the steps in the below link:
https://github.com/plerup/makeEspArduino

cd to esp32-ex
make upload -> should work but sometime fails.
use below
/home/sms/esp32/arduino-esp32/tools/esptool.py --port /dev/ttyUSB0 write_flash 0x0000 ./build/Enode1001_v1.0.2_esp32/Enode1001_v1.0.2.bin

/home/sms/esp32/arduino-esp32/tools/esptool.py --chip esp32 --port /dev/ttyUSB0 write_flash 0x1000 ./build/Enode1001_v1.0.2_esp32/Enode1001_v1.0.2.bin

Also look at the below links if need be:
https://github.com/sudar/Arduino-Makefile
https://github.com/sudar/Arduino-Makefile/tree/master/examples
