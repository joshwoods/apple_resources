

- Network
-  NWPath 

Structure

# NWPath

An object that contains information about the properties of the network that a connection uses, or that are available to your app.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
struct NWPath
```

## Topics

### Checking Path Availability

let status: NWPath.Status

A status indicating whether a path can be used by connections.

enum Status

Status values indicating whether a path can be used by connections.

### Inspecting Interfaces

func usesInterfaceType(NWInterface.InterfaceType) -> Bool

Checks if connections using the path may send traffic over a specific interface type.

let availableInterfaces: [NWInterface]

A list of all interfaces available to the path, in order of preference.

var gateways: [NWEndpoint]

A list of gateways configured on the interfaces available to a path.

### Checking Path Capabilities

let supportsIPv4: Bool

A Boolean indicating whether the path can route IPv4 traffic.

let supportsIPv6: Bool

A Boolean indicating whether the path can route IPv6 traffic.

let supportsDNS: Bool

A Boolean indicating whether the path has a DNS server configured.

var isConstrained: Bool

A Boolean indicating whether the path uses an interface in Low Data Mode.

let isExpensive: Bool

A Boolean indicating whether the path uses an interface that is considered expensive, such as Cellular or a Personal Hotspot.

### Inspecting Connected Paths

let localEndpoint: NWEndpoint?

The local endpoint in use by a connection’s network path.

let remoteEndpoint: NWEndpoint?

The remote endpoint in use by a connection’s network path.

### Instance Properties

var unsatisfiedReason: NWPath.UnsatisfiedReason

### Enumerations

enum UnsatisfiedReason

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Equatable
- Sendable

## See Also

### Paths and Interfaces

class NWPathMonitor

An observer that you use to monitor and react to network changes.

struct NWInterface

An interface that a network connection uses to send and receive data.

