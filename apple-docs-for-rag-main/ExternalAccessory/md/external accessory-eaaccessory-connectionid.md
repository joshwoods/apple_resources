

- External Accessory
- EAAccessory
-  connectionID 

Instance Property

# connectionID

The accessory’s unique ID for connecting to the iOS-based device.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
var connectionID: Int { get }
```

## Discussion

The connection ID uniquely identifies this accessory to the device. If multiple accessories of the same type are connected to the device, you can use this information to distinguish between them.

The connection ID for an accessory persists only for the duration of the current connection. If the accessory is disconnected and reconnected, a new connection ID is assigned.

## See Also

### Getting Connection Information

var isConnected: Bool

A Boolean value indicating whether the accessory is currently connected to the iOS-based device.

Null Connection ID

The ID for an unconnected accessory.

