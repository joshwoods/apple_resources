

- Foundation
- URLRequest
-  allowsPersistentDNS 

Instance Property

# allowsPersistentDNS

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var allowsPersistentDNS: Bool { get set }
```

## See Also

### Controlling request behavior

var timeoutInterval: TimeInterval

The timeout interval of the request.

var httpShouldHandleCookies: Bool

A Boolean value indicating whether cookies will be sent with and set for this request.

var httpShouldUsePipelining: Bool

A Boolean value indicating whether the request should transmit before the previous response is received.

Deprecated

var allowsCellularAccess: Bool

A Boolean value indicating whether the request is allowed to use the built-in cellular radios to satisfy the request.

var assumesHTTP3Capable: Bool

var cookiePartitionIdentifier: String?

var requiresDNSSECValidation: Bool

