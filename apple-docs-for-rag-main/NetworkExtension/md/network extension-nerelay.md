

- Network Extension
-  NERelay 

Class

# NERelay

A single relay server configuration that you can chain together with other relays.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class NERelay
```

## Overview

Relay servers are secure HTTP proxies that allow proxying TCP traffic using the `CONNECT` method and UDP traffic using the `connect-udp` protocol defined in RFC 9298.

## Topics

### Configuring server properties

var http3RelayURL: URL?

A URL identifying the relay server accessible using HTTP/3.

var http2RelayURL: URL?

A URL identifying the relay server accessible using HTTP/2.

var dnsOverHTTPSURL: URL?

The URL of a DNS-over-HTTPS (DoH) resolver accessible from the relay.

var rawPublicKeys: [Data]?

An array of TLS raw public keys that the relay server can present during the TLS handshake.

### Configuring client properties

var additionalHTTPHeaderFields: [String : String]

A dictionary of additional HTTP headers to send as part of `CONNECT` requests to the relay.

var identityData: Data?

The PKCS12 data for the relay client authentication.

var identityDataPassword: String?

The password the relay uses to decrypt the PKCS12 identity data.

var syntheticDNSAnswerIPv4Prefix: String?

An IPv4 address prefix the relay uses to handle address info requests.

var syntheticDNSAnswerIPv6Prefix: String?

An IPv6 address prefix the relay uses to handle address info requests.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Relay configuration

class NERelayManager

An object you use to create and manage a network relay configuration.

