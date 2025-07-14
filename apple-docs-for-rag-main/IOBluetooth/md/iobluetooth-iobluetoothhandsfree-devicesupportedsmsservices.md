

- IOBluetooth
- IOBluetoothHandsFree
-  deviceSupportedSMSServices 

Instance Property

# deviceSupportedSMSServices

Return the device’s supported SMS services.

macOS 10.7+

``` source
var deviceSupportedSMSServices: UInt32 { get }
```

## Return Value

The SMS services supported

## Discussion

Returns the device’s supported SMS services bitmap. The values are described in “IOBluetoothHandsFreeSMSSupport.”

