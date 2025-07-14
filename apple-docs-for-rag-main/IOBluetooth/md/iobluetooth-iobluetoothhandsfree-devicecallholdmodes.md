

- IOBluetooth
- IOBluetoothHandsFree
-  deviceCallHoldModes 

Instance Property

# deviceCallHoldModes

Return the device’s supported call hold modes.

macOS 10.7+

``` source
var deviceCallHoldModes: UInt32 { get }
```

## Return Value

The SMS services supported

## Discussion

Returns the device’s supported call hold modes bitmap. The values are described in “IOBluetoothHandsFreeCallHoldModes.”

