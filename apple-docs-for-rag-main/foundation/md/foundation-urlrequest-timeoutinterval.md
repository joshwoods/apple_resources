

- Foundation
- URLRequest
-  timeoutInterval 

Instance Property

# timeoutInterval

The timeout interval of the request.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var timeoutInterval: TimeInterval { get set }
```

## Discussion

If during a connection attempt the request remains idle for longer than the timeout interval, the request is considered to have timed out. The default timeout interval is 60 seconds.

As a general rule, you should not use short timeout intervals. Instead, you should provide an easy way for the user to cancel a long-running operation. For more information, read Designing for Real-World Networks in Networking Overview.

## See Also

### Controlling request behavior

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

var requiresDNSSECValidation: Bool

