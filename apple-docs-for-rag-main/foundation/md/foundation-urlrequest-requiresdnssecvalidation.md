

- Foundation
- URLRequest
-  requiresDNSSECValidation 

Instance Property

# requiresDNSSECValidation

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
var requiresDNSSECValidation: Bool { get set }
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

var allowsPersistentDNS: Bool

var assumesHTTP3Capable: Bool

var cookiePartitionIdentifier: String?

