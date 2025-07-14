

- Core Bluetooth
- CBPeripheral
-  openL2CAPChannel(\_:) 

Instance Method

# openL2CAPChannel(\_:)

Attempts to open an L2CAP channel to the peripheral using the supplied Protocol/Service Multiplexer (PSM).

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.14+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func openL2CAPChannel(_ PSM: CBL2CAPPSM)
```

## Parameters 

`PSM`  

The PSM of the channel to open.

## See Also

### Working with L2CAP Channels

class CBL2CAPChannel

A live L2CAP connection to a remote device.

typealias CBL2CAPPSM

The type of PSM identifiers.

