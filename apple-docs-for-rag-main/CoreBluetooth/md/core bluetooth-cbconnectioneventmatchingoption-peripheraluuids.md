

- Core Bluetooth
- CBConnectionEventMatchingOption
-  peripheralUUIDs 

Type Property

# peripheralUUIDs

An array of UUID objects that represents peripherals to match.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static let peripheralUUIDs: CBConnectionEventMatchingOption
```

## Discussion

A connected peer with any matching peripheral UUIDs results in a call to centralManager(_:connectionEventDidOccur:for:).

## See Also

### Matching Options

static let serviceUUIDs: CBConnectionEventMatchingOption

An array that represents service identifiers to match.

