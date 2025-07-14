

- IOBluetooth
- IOBluetoothDevice
-  recentDevices(\_:) 

Type Method

# recentDevices(\_:)

Gets an array of recently used Bluetooth devices.

macOS

``` source
class func recentDevices(_ numDevices: UInt) -> [Any]!
```

## Parameters 

`numDevices`  

The number of devices to return.

## Return Value

Returns an array of device objects recently used by the system. If no devices have been accessed, nil is returned.

## Discussion

The resulting array contains IOBluetoothDevice objects sorted in reverse chronological order. The most recently accessed devices are first. If the numDevices parameter is 0, all devices accessed by the system are returned. If numDevices is non-zero, only the most recent devices are returned.

NOTE: This method is only available in macOS 10.2.4 (Bluetooth v1.1) or later.

