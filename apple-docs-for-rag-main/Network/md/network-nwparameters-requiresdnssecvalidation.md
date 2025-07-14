

- Network
- NWParameters
-  requiresDNSSECValidation 

Instance Property

# requiresDNSSECValidation

A Boolean value that determines whether a connection requires DNSSEC validation when resolving endpoints.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
final var requiresDNSSECValidation: Bool { get set }
```

## See Also

### Customizing Connection Options

var multipathServiceType: NWParameters.MultipathServiceType

An option to allow connections to use multipath protocols.

enum MultipathServiceType

Modes in which a connection can support multipath protocols.

var serviceClass: NWParameters.ServiceClass

A level of service quality for connections to use for Cellular Network Slicing.

enum ServiceClass

Indicates the traffic characteristics of the network connections used by Cellular Network Slicing.

var allowFastOpen: Bool

A Boolean that enables sending application data with protocol handshakes.

var expiredDNSBehavior: NWParameters.ExpiredDNSBehavior

A behavior that defines how expired DNS answers will be used.

enum ExpiredDNSBehavior

Options for configuring how expired DNS answers should be used.

var preferNoProxies: Bool

A Boolean that indicates that connections should ignore proxies when they are enabled on the system.

var includePeerToPeer: Bool

A Boolean that enables peer-to-peer link technologies for connections and listeners.

var allowLocalEndpointReuse: Bool

A Boolean that allows reusing local addresses and ports across connections.

var acceptLocalOnly: Bool

A Boolean that restricts listeners to only accepting connections from the local link.

