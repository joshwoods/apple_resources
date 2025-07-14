

- Objective-C Runtime
- NSObject
-  readRSSI(forDeviceComplete:device:info:error:) 

Instance Method

# readRSSI(forDeviceComplete:device:info:error:)

macOS

``` source
func readRSSI(
    forDeviceComplete controller: Any!,
    device: IOBluetoothDevice!,
    info: UnsafeMutablePointer!,
    error: IOReturn
)
```

## Parameters 

`controller`  

Controller object that sent this delegate message.

`device`  

The `IOBluetooth` device.

`info`  

A pointer to the info.

## Discussion

This delegate gets invoked when an RSSI command complete event occurs. This could occur because you invoked it by issuing a `-readRSSIForDevice:` command, or someone else did from another app on the same controller.

