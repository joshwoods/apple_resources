

- Network Extension
- NERelay
-  additionalHTTPHeaderFields 

Instance Property

# additionalHTTPHeaderFields

A dictionary of additional HTTP headers to send as part of `CONNECT` requests to the relay.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var additionalHTTPHeaderFields: [String : String] { get set }
```

## See Also

### Configuring client properties

var identityData: Data?

The PKCS12 data for the relay client authentication.

var identityDataPassword: String?

The password the relay uses to decrypt the PKCS12 identity data.

var syntheticDNSAnswerIPv4Prefix: String?

An IPv4 address prefix the relay uses to handle address info requests.

var syntheticDNSAnswerIPv6Prefix: String?

An IPv6 address prefix the relay uses to handle address info requests.

