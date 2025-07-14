

- Foundation
- URLRequest
-  httpShouldHandleCookies 

Instance Property

# httpShouldHandleCookies

A Boolean value indicating whether cookies will be sent with and set for this request.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var httpShouldHandleCookies: Bool { get set }
```

## Discussion

`true` if the default cookie handling will be used for this request, `false` otherwise. The default is `true`.

## See Also

### Controlling request behavior

var timeoutInterval: TimeInterval

The timeout interval of the request.

var httpShouldUsePipelining: Bool

A Boolean value indicating whether the request should transmit before the previous response is received.

Deprecated

var allowsCellularAccess: Bool

A Boolean value indicating whether the request is allowed to use the built-in cellular radios to satisfy the request.

var allowsPersistentDNS: Bool

var assumesHTTP3Capable: Bool

var cookiePartitionIdentifier: String?

var requiresDNSSECValidation: Bool

