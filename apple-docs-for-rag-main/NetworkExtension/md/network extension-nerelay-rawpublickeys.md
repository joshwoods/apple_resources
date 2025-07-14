

- Network Extension
- NERelay
-  rawPublicKeys 

Instance Property

# rawPublicKeys

An array of TLS raw public keys that the relay server can present during the TLS handshake.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var rawPublicKeys: [Data]? { get set }
```

## Discussion

If you set one or more keys, the raw public keys are used to authenticate the relay server. If no keys are set, or if the array is `nil`, default TLS server certificate evaluation is used.

## See Also

### Configuring server properties

var http3RelayURL: URL?

A URL identifying the relay server accessible using HTTP/3.

var http2RelayURL: URL?

A URL identifying the relay server accessible using HTTP/2.

var dnsOverHTTPSURL: URL?

The URL of a DNS-over-HTTPS (DoH) resolver accessible from the relay.

