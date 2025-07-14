

- IOBluetooth
- IOBluetoothHandsFree
-  isSMSEnabled 

Instance Property

# isSMSEnabled

Return YES if the device has SMS enabled.

macOS 10.7+

``` source
var isSMSEnabled: Bool { get }
```

## Discussion

Returns YES if the device has SMS enabled (by responding to a CMGF command). NO if the device has not set an SMS mode or doesn’t support SMS.

