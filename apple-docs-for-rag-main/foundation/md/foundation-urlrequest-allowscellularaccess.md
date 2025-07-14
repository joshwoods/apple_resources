

- Foundation
- URLRequest
-  allowsCellularAccess 

Instance Property

# allowsCellularAccess

A Boolean value indicating whether the request is allowed to use the built-in cellular radios to satisfy the request.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var allowsCellularAccess: Bool { get set }
```

## Discussion

Setting this property to `true` makes the request eligible to run over cellular, subject to other considerations (including, but not limited to, the URLSessionConfiguration’s allowsCellularAccess property). Setting this value to `false` ensures that the request will never run over cellular.

## See Also

### Related Documentation

var waitsForConnectivity: Bool

A Boolean value that indicates whether the session should wait for connectivity to become available, or fail immediately.

### Controlling request behavior

var timeoutInterval: TimeInterval

The timeout interval of the request.

var httpShouldHandleCookies: Bool

A Boolean value indicating whether cookies will be sent with and set for this request.

var httpShouldUsePipelining: Bool

A Boolean value indicating whether the request should transmit before the previous response is received.

Deprecated

var allowsPersistentDNS: Bool

var assumesHTTP3Capable: Bool

var cookiePartitionIdentifier: String?

var requiresDNSSECValidation: Bool

