

- Foundation
- NSURLRequest
-  httpShouldHandleCookies 

Instance Property

# httpShouldHandleCookies

A Boolean value that indicates whether the default cookie handling will be used for this request.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var httpShouldHandleCookies: Bool { get }
```

## Discussion

true if the default cookie handling will be used for this request, false otherwise. The default is true.

## See Also

### Related Documentation

var httpShouldHandleCookies: Bool

A Boolean value that indicates whether the request should use the default cookie handling for the request.

### Controlling request behavior

var timeoutInterval: TimeInterval

The request’s timeout interval, in seconds.

var httpShouldUsePipelining: Bool

A Boolean value that indicates whether the request should continue transmitting data before receiving a response from an earlier transmission.

Deprecated

var allowsCellularAccess: Bool

A Boolean value that indicates whether the request is allowed to use the cellular radio (if present).

