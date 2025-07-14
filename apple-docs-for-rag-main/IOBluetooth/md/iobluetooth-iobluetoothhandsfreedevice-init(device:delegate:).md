

- IOBluetooth
- IOBluetoothHandsFreeDevice
-  init(device:delegate:) 

Initializer

# init(device:delegate:)

Creates an object to manage phone calls on a hands-free Bluetooth device.

macOS 10.7+

``` source
init!(
    device: IOBluetoothDevice!,
    delegate: Any!
)
```

## Parameters 

`device`  

A Bluetooth device.

`delegate`  

A delegate that conforms to the IOBluetoothHandsFreeDeviceDelegate protocol.

