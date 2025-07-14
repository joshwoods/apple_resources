

- Core Bluetooth
-  CBPeripheralManagerOptionRestoreIdentifierKey 

Global Variable

# CBPeripheralManagerOptionRestoreIdentifierKey

A unique identifier (UID) with which to instantiate the peripheral manager.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let CBPeripheralManagerOptionRestoreIdentifierKey: String
```

## Discussion

The value associated with this key is an NSString.

The system uses this UID to identify a specific peripheral manager. As a result, the UID must remain the same for subsequent executions of the app for successful restoration of the peripheral manager.

## See Also

### Initialization Options

let CBPeripheralManagerOptionShowPowerAlertKey: String

A Boolean value specifying whether the system should warn if Bluetooth is in the powered-off state when instantiating the peripheral manager.

