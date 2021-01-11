# My-voron-config
Config for my voron 2.4 with fluidd and prusaslicers



Update MCUS:

cd ~/klipper/
make menuconfig
make clean
make
ls /dev/serial/by-id/*
sudo service klipper stop
make flash FLASH_DEVICE=/dev/serial/by-id/usb-Klipper_lpc1768_055000138280F7AE35139457C42000F5-if00
make flash FLASH_DEVICE=/dev/serial/by-id/usb-Klipper_lpc1768_0E10011402094AAF72B05E5DC12000F5-if00
sudo service klipper start
