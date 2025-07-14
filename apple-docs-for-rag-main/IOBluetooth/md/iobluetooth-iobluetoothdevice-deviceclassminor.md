

- IOBluetooth
- IOBluetoothDevice
-  deviceClassMinor 

Instance Property

# deviceClassMinor

Get the minor service class of the device.

macOS

``` source
var deviceClassMinor: BluetoothDeviceClassMinor { get }
```

## Discussion

This value is only meaningful if the target device has been seen during an inquiry. This can be by checking the result of -getLastInquiryUpdate. If nil is returned, then the device hasn’t been seen.

