# MIScooterPy

Python code for communicating with Xiaomi M365 Scooter over GATT using bluepy.
Based on the [profound reversing work of Camilo Ruiz](https://github.com/CamiAlfa/M365-BLE-PROTOCOL/blob/master/protocolo).

Final goal is to have Firmware(s) update using other than the currently available Android apps, from devices such as PC, RPi and perhaps Arduino. The project is WIP and currently supports a few 'get' commands, but is being updated with more commands progressively.

Feel free to contribute :)


## Installation
No installation is required except for the BluePy python library. Installation instructions can be found [on bluepy's github page](https://github.com/IanHarvey/bluepy)

Code is targeting Python 3 
Tested on Raspberry Pi 3 Model B

## Usage

```python
myMAC='AA:AA:AA:AA:AA:AA'
com=CommManager(myMAC)
com.connect()
com.send('GetSerial')
# Response will be printed to console
com.send('GetFirmware')
com.send('GetPincode')
```

