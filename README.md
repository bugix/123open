# 123open
An effort to reverse engineer the 123ignition tune serial protocol and provide open tools to the community of vintage car enthusiasts.

So far we know that the [123ignition](https://123ignition.com) Tune distributor submits its sensor data via a USB-to-Serial chip from [FTDI](https://www.ftdichip.com). This byte stream may contain values for RPM, ignition timing, coil current, vacuum and temperature as they are displayed by gauges in the Windows application.

By turning the distributor with a cordless screwdriver, we received the following byte sequences from the serial port:

## 850 RPM
63 53 3c 47 86 82 63 73 2c 47 86 82 63 73 2c 47 86 82 63 73 2c 47 86 82 63 73 2c 47 86 82 63 73 2c 47 86 82 63 73 2c 47 86 82 63 73 2c 47 86 82 63 73 2c 47 86 82 63 73 2c 47 86 82 63 73 2c 47 86 82 63 73 2c 47 86 82 63 73 2c 47 86 82 63 73 2c 47 86 82 63 73 2c 47 86 82 63 73 2c 47 86 82 63 73 2c 47 86 82 63 73 2c 47 86 82 63 73 2c 47 86 82 63 73 2c 47 86 82 63 73 2c 47 86 82 63 73 ...

## 2900 RPM
63 73 2c 47 86 82 63 73 3c 47 86 82 63 63 1e 57 86 82 63 73 1e 57 86 82 63 73 0e 57 86 82 63 63 1e 47 86 82 63 73 0e 57 86 82 63 53 2e 57 86 82 63 73 0e 57 86 82 63 53 2e 47 86 82 63 73 0e 57 86 82 63 53 2e 47 86 82 63 73 0e 57 86 82 63 43 2e 57 86 82 63 73 0e 57 86 82 63 53 2e 47 86 82 63 63 1e 57 86 82 63 53 2e 47 86 82 63 63 1e 57 86 82 63 53 2e 57 86 82 63 63 1e 57 86 82 63 73 ...

**If you have any idea on how to interpret this data, please let us know!**
