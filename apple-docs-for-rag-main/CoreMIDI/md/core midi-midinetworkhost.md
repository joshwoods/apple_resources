

- Core MIDI
-  MIDINetworkHost 

Class

# MIDINetworkHost

An object that represents the host’s network address.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class MIDINetworkHost
```

## Topics

### Creating Network Hosts

convenience init(name: String, address: String, port: Int)

Creates a host with the specified name, adress, and port.

convenience init(name: String, netService: NetService)

Creates a host with the specified name and net service.

convenience init(name: String, netServiceName: String, netServiceDomain: String)

Creates a host with the specified name, net service name, and domain.

let MIDINetworkBonjourServiceType: String

The Bonjour service type.

### Inspecting Host Properties

var name: String

The host name.

var netServiceName: String?

The net service name.

var netServiceDomain: String?

The net service domain.

var address: String

The host address.

var port: Int

The host port.

### Comparing Hosts

func hasSameAddress(as: MIDINetworkHost) -> Bool

Compares this host instance with another to see if they share the same address value.

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

class MIDINetworkConnection

An object that connects a session to a host.

class MIDINetworkSession

An object that represents a pairing of a source and destination.

