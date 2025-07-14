

- Core Bluetooth
-  CBCentralManagerOptionShowPowerAlertKey 

Global Variable

# CBCentralManagerOptionShowPowerAlertKey

A Boolean value that specifies whether the system warns the user if the app instantiates the central manager when Bluetooth service isn’t available.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let CBCentralManagerOptionShowPowerAlertKey: String
```

## Discussion

The value for this key is an NSNumber object. If the key isn’t specified, the default value is true.

## See Also

### Constants

let CBCentralManagerOptionRestoreIdentifierKey: String

A string containing a unique identifier (UID) for the central manager to instantiate.

