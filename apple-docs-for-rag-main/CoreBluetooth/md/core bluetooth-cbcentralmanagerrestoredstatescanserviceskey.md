

- Core Bluetooth
-  CBCentralManagerRestoredStateScanServicesKey 

Global Variable

# CBCentralManagerRestoredStateScanServicesKey

An array of service IDs for use when restoring state.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.13+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let CBCentralManagerRestoredStateScanServicesKey: String
```

## Discussion

The value associated with this key is an NSArray of service UUIDs (represented by CBUUID objects) containing all the services the central manager was scanning for at the time the system terminated the app.

## See Also

### State Restoration Options

let CBCentralManagerRestoredStatePeripheralsKey: String

An array of peripherals for use when restoring the state of a central manager.

let CBCentralManagerRestoredStateScanOptionsKey: String

A dictionary of peripheral scan options for use when restoring state.

