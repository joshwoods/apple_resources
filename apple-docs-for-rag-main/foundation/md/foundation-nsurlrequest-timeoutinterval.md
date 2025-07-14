

- Foundation
- NSURLRequest
-  timeoutInterval 

Instance Property

# timeoutInterval

The request’s timeout interval, in seconds.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var timeoutInterval: TimeInterval { get }
```

## Discussion

If during a connection attempt the request remains idle for longer than the timeout interval, the request is considered to have timed out.

## See Also

### Related Documentation

var timeoutInterval: TimeInterval

The request’s timeout interval, in seconds.

### Controlling request behavior

var httpShouldHandleCookies: Bool

A Boolean value that indicates whether the default cookie handling will be used for this request.

var httpShouldUsePipelining: Bool

A Boolean value that indicates whether the request should continue transmitting data before receiving a response from an earlier transmission.

Deprecated

var allowsCellularAccess: Bool

A Boolean value that indicates whether the request is allowed to use the cellular radio (if present).

