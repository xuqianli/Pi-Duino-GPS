# Pi-Duino-GPS
The Pi-Duino-GPS is a C++ project that controls a robot to follow a specific GPS coordinates. It also calculates the distance between the robot and the destination to notify the user of the current progress. This project was also implemented with node.js and you can check it out at [0xb0t](https://github.com/xuqianli/0xb0t.git).

The robot is composed of:  

* a Raspberry Pi modle B
* a GPS module 
* a camera module
* an Arduino UNO
* an Arduino Motor Shield
* 2 motors

## Raspberry Pi Hotspot

Since we wish to monitor the status of the robot, we need a way to communicate with the robot to get updated.

Inorder to get a wifi access point working on the raspberry pi, we have borrowed the following script from [Paul](http://blog.sip2serve.com/post/48899893167/rtl8188-access-point-install-script)

```
cd raspi-hotspot
sudo chown root:root  install-rtl8188cus.sh
sudo chmod 755 install-rtl8188cus.sh
sudo ./install-rtl8188cus.sh to run the script.
```

After running the script, you should be able to detect the raspberry pi wifi from another device.


