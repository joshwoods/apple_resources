

- Core MIDI
-  MIDINetworkConnection 

Class

# MIDINetworkConnection

An object that connects a session to a host.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class MIDINetworkConnection
```

## Topics

### Creating Connections

convenience init(host: MIDINetworkHost)

Creates a connection to the specified host.

### Accessing Connections

var host: MIDINetworkHost

The host connection.

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

### Networking

class MIDINetworkHost

An object that represents the host’s network address.

class MIDINetworkSession

An object that represents a pairing of a source and destination.

