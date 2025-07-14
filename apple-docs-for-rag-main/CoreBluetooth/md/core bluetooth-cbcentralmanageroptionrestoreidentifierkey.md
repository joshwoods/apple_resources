

- Core Bluetooth
-  CBCentralManagerOptionRestoreIdentifierKey 

Global Variable

# CBCentralManagerOptionRestoreIdentifierKey

A string containing a unique identifier (UID) for the central manager to instantiate.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.13+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let CBCentralManagerOptionRestoreIdentifierKey: String
```

## Discussion

The value for this key is an NSString. The system uses this UID to identify a specific central manager. As a result, the UID must remain the same for subsequent executions of the app to restore the central manager.

## See Also

### Constants

let CBCentralManagerOptionShowPowerAlertKey: String

A Boolean value that specifies whether the system warns the user if the app instantiates the central manager when Bluetooth service isn’t available.

