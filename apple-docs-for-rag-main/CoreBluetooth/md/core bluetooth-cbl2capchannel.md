

- Core Bluetooth
-  CBL2CAPChannel 

Class

# CBL2CAPChannel

A live L2CAP connection to a remote device.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class CBL2CAPChannel
```

## Topics

### Accessing Streams

var inputStream: InputStream!

The stream used for reading data from the remote peer.

var outputStream: OutputStream!

The stream used for writing data to the peer.

### Accessing the Peer

var peer: CBPeer!

The peer connected to the channel.

### Accessing the Protocol/Service Multiplexer

var psm: CBL2CAPPSM

The PSM of the channel.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Working with L2CAP Channels

func openL2CAPChannel(CBL2CAPPSM)

Attempts to open an L2CAP channel to the peripheral using the supplied Protocol/Service Multiplexer (PSM).

typealias CBL2CAPPSM

The type of PSM identifiers.

