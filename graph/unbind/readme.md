# Prevent USB from being used locally!
# Guide:
- https://stackoverflow.com/questions/59755514/unbinded-usb-device-get-automatically-bind-on-linux
- https://stackoverflow.com/questions/18765725/turning-off-a-single-usb-device-again

# sch:
https://www.google.com/search?q=ubuntu+usb+unbind+driver

# Code:
```
echo -n usb1 | sudo tee /sys/bus/usb/drivers/usb/unbind
ls /sys/bus/usb/devices
```
