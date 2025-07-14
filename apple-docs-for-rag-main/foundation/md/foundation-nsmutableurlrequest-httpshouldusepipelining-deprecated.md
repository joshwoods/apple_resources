

- Foundation
- NSMutableURLRequest
-  httpShouldUsePipelining Deprecated

Instance Property

# httpShouldUsePipelining

A Boolean value that indicates whether the request can continue transmitting data before receiving a response from an earlier transmission.

iOS 4.0–18.4DeprecatediPadOS 4.0–18.4DeprecatedMac Catalyst 13.1–18.4DeprecatedmacOS 10.7–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–11.4Deprecated

``` source
var httpShouldUsePipelining: Bool { get set }
```

Deprecated

Only supported in the classic loader, please adopt HTTP/2 and HTTP/3 instead

## Discussion

true if the request should continue transmitting data, false if the request should wait for a response. The default value is false.

Setting this property to true value does not guarantee HTTP pipelining behavior. This may have no effect if an HTTP proxy is configured, or if the HTTP request uses an unsafe request method—for example, POST requests will not pipeline. Pipelining behavior may not begin until the second request on a given TCP connection. There may be other situations where pipelining does not occur even though this property is set to true. HTTP 1.1 allows the client to send multiple requests to the server without waiting for a response. Though HTTP 1.1 requires support for pipelining, some servers report themselves as being HTTP 1.1 but do not support pipelining (disconnecting, sending resources in the wrong order, omitting part of a resource, etc.).

## See Also

### Controlling request behavior

var timeoutInterval: TimeInterval

The request’s timeout interval, in seconds.

var httpShouldHandleCookies: Bool

A Boolean value that indicates whether the request should use the default cookie handling for the request.

var allowsCellularAccess: Bool

A Boolean value that indicates whether a connection can use the device’s cellular network (if present).

