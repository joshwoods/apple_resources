

- Foundation
- NSURLRequest
-  allowsCellularAccess 

Instance Property

# allowsCellularAccess

A Boolean value that indicates whether the request is allowed to use the cellular radio (if present).

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var allowsCellularAccess: Bool { get }
```

## Discussion

true if the cellular radio can be used; false otherwise.

## See Also

### Related Documentation

var allowsCellularAccess: Bool

A Boolean value that indicates whether a connection can use the device’s cellular network (if present).

### Controlling request behavior

var timeoutInterval: TimeInterval

The request’s timeout interval, in seconds.

var httpShouldHandleCookies: Bool

A Boolean value that indicates whether the default cookie handling will be used for this request.

var httpShouldUsePipelining: Bool

A Boolean value that indicates whether the request should continue transmitting data before receiving a response from an earlier transmission.

Deprecated

