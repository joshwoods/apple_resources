

- Network
- NWParameters
-  init(customIPProtocolNumber:) 

Initializer

# init(customIPProtocolNumber:)

Initializes parameters for connections and listeners using a custom IP protocol.

macOS 10.15+

``` source
init(customIPProtocolNumber: UInt8)
```

## Discussion

Creating custom IP protocol connections requires the “com.apple.developer.networking.custom-protocol” entitlement.

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

init()

Initializes parameters for connections, listeners, and browsers with no protocols specified.

func copy() -> NWParameters

Performs a deep copy of a parameters object.

