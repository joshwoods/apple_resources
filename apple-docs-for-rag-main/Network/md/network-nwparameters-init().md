

- Network
- NWParameters
-  init() 

Initializer

# init()

Initializes parameters for connections, listeners, and browsers with no protocols specified.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
init()
```

## See Also

### Creating Parameters

class var tls: NWParameters

A set of default parameters for connections and listeners that use TLS and TCP.

class var tcp: NWParameters

A set of default parameters for connections and listeners that use TCP.

class var dtls: NWParameters

A set of default parameters for connections and listeners that use DTLS and UDP.

class var udp: NWParameters

A set of default parameters for connections and listeners that use UDP.

class func quic(alpn: [String]) -> NWParameters

Returns a set of default parameters for connections and listeners that use QUIC, with a set of supported Application-Layer Protocol Negotiation values.

class func quicDatagram(alpn: [String]) -> NWParameters

Returns a set of default parameters for connections and listeners that use QUIC datagrams, with a set of supported Application-Layer Protocol Negotiation values.

convenience init(tls: NWProtocolTLS.Options?, tcp: NWProtocolTCP.Options)

Initializes parameters for TLS connections and listeners with custom TLS and TCP options.

convenience init(dtls: NWProtocolTLS.Options?, udp: NWProtocolUDP.Options)

Initializes parameters for DTLS connections and listeners with custom DTLS and UDP options.

convenience init(quic: NWProtocolQUIC.Options)

Initializes parameters for QUIC connections and listeners with custom QUIC options.

init(customIPProtocolNumber: UInt8)

Initializes parameters for connections and listeners using a custom IP protocol.

func copy() -> NWParameters

Performs a deep copy of a parameters object.

