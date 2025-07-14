

- Core Bluetooth
-  CBPeripheralManagerOptionShowPowerAlertKey 

Global Variable

# CBPeripheralManagerOptionShowPowerAlertKey

A Boolean value specifying whether the system should warn if Bluetooth is in the powered-off state when instantiating the peripheral manager.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let CBPeripheralManagerOptionShowPowerAlertKey: String
```

## Discussion

The value for this key is an NSNumber. If the key isn’t specified, the default value is false.

## See Also

### Initialization Options

let CBPeripheralManagerOptionRestoreIdentifierKey: String

A unique identifier (UID) with which to instantiate the peripheral manager.

