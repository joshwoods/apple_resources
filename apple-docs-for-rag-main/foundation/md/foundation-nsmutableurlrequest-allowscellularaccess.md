

- Foundation
- NSMutableURLRequest
-  allowsCellularAccess 

Instance Property

# allowsCellularAccess

A Boolean value that indicates whether a connection can use the device’s cellular network (if present).

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var allowsCellularAccess: Bool { get set }
```

## Discussion

Setting this property to true (the default) makes the request eligible to run over cellular, subject to other considerations (including, but not limited to, the allowsCellularAccess property of the URLSessionConfiguration). Setting this value to false ensures that the request will never run over cellular.

## See Also

### Related Documentation

var waitsForConnectivity: Bool

A Boolean value that indicates whether the session should wait for connectivity to become available, or fail immediately.

### Controlling request behavior

var timeoutInterval: TimeInterval

The request’s timeout interval, in seconds.

var httpShouldHandleCookies: Bool

A Boolean value that indicates whether the request should use the default cookie handling for the request.

var httpShouldUsePipelining: Bool

A Boolean value that indicates whether the request can continue transmitting data before receiving a response from an earlier transmission.

Deprecated

