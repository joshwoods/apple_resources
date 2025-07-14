

- IOBluetooth
- IOBluetoothDevicePair
-  init(device:) 

Initializer

# init(device:)

Creates an autorelease IOBluetoothDevicePair object with a device as the pairing target.

macOS

``` source
convenience init!(device: IOBluetoothDevice!)
```

## Parameters 

`device`  

An IOBluetoothDevice to attept to pair with. The device is retained.

## Return Value

Returns an IOReturn or Bluetooth error code, if the pairing could not be started.

