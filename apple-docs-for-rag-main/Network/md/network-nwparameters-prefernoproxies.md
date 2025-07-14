

- Network
- NWParameters
-  preferNoProxies 

Instance Property

# preferNoProxies

A Boolean that indicates that connections should ignore proxies when they are enabled on the system.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
final var preferNoProxies: Bool { get set }
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

var requiresDNSSECValidation: Bool

A Boolean value that determines whether a connection requires DNSSEC validation when resolving endpoints.

var includePeerToPeer: Bool

A Boolean that enables peer-to-peer link technologies for connections and listeners.

var allowLocalEndpointReuse: Bool

A Boolean that allows reusing local addresses and ports across connections.

var acceptLocalOnly: Bool

A Boolean that restricts listeners to only accepting connections from the local link.

