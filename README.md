# Raspberry 4b Adafruit DHT Patch
Patch with Adafruit_DHT libray in Python 3.7 with Raspberry pi 4 model b. Adafruit_DHT by default is not supporting Raspberry Pi 4 model b in his installation packages. 

## Installing

To install the solution program into your Raspb Python Library, you have to install first the library for Adafruit_DHT:

```bash
sudo apt-get update
sudo apt-get install python3-pip
sudo python3 -m pip install --upgrade pip setuptools wheel
sudo pip3 install Adafruit_DHT
```
Second step, go to the Python3.7 packages by using the following command: 
```bash
cd /usr/local/lib/python3.7/dist-packages/Adafruit_DHT
````
Finally, you have to git the python program from this repository:
```bash
sudo rm -r platform_detect.py
sudo wget -L https://raw.githubusercontent.com/ferburri/Raspb_4b_Adafruit_DHT/master/platform_detect.py
```

Last step, check if your python3 file is obtaining the information from the sensors
```bash 
python3 "example.py"
```

