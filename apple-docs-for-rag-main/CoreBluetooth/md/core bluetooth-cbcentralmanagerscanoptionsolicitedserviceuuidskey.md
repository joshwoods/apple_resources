

- Core Bluetooth
-  CBCentralManagerScanOptionSolicitedServiceUUIDsKey 

Global Variable

# CBCentralManagerScanOptionSolicitedServiceUUIDsKey

An array of service UUIDs that you want to scan for.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let CBCentralManagerScanOptionSolicitedServiceUUIDsKey: String
```

## Discussion

The array is an instance of NSArray, and uses CBUUID objects to represent the UUIDs to scan for.

Specifying this scan option causes the central manager to also scan for peripherals soliciting any of the services contained in the array.

## See Also

### Constants

let CBCentralManagerScanOptionAllowDuplicatesKey: String

A Boolean value that specifies whether the scan should run without duplicate filtering.

