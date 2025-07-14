

- Network Extension
- NERelay
-  http3RelayURL 

Instance Property

# http3RelayURL

A URL identifying the relay server accessible using HTTP/3.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var http3RelayURL: URL? { get set }
```

## See Also

### Configuring server properties

var http2RelayURL: URL?

A URL identifying the relay server accessible using HTTP/2.

var dnsOverHTTPSURL: URL?

The URL of a DNS-over-HTTPS (DoH) resolver accessible from the relay.

var rawPublicKeys: [Data]?

An array of TLS raw public keys that the relay server can present during the TLS handshake.

