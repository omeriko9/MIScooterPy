# MIScooterPy

Python code for communicating with Xiaomi M365 Scooter over GATT using bluepy.
Based on the [profound reversing work of Camilo Ruiz](https://github.com/CamiAlfa/M365-BLE-PROTOCOL/blob/master/protocolo)

## Installation
Make sure [bluepy](https://github.com/IanHarvey/bluepy) is installed
(Note: code was tested on RPi3 w/ BLE)

## Usage

```python
com=CommManager('AA:AA:AA:AA:AA:AA') # Use real MAC address
com.connect()
com.send('GetSerial')
com.send('GetFirmware')
com.send('GetPincode')
```

