

- Network Extension
- NERelay
-  syntheticDNSAnswerIPv6Prefix 

Instance Property

# syntheticDNSAnswerIPv6Prefix

An IPv6 address prefix the relay uses to handle address info requests.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var syntheticDNSAnswerIPv6Prefix: String? { get set }
```

## Discussion

The value of this property is an address prefix, such as `2001:DB8::/32`. The relay manager uses this prefix to synthesize DNS answers for apps that use `getaddrinfo()` to resolve domains included in matchDomains.

## See Also

### Configuring client properties

var additionalHTTPHeaderFields: [String : String]

A dictionary of additional HTTP headers to send as part of `CONNECT` requests to the relay.

var identityData: Data?

The PKCS12 data for the relay client authentication.

var identityDataPassword: String?

The password the relay uses to decrypt the PKCS12 identity data.

var syntheticDNSAnswerIPv4Prefix: String?

An IPv4 address prefix the relay uses to handle address info requests.

