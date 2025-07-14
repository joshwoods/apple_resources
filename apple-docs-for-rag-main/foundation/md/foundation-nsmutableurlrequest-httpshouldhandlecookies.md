

- Foundation
- NSMutableURLRequest
-  httpShouldHandleCookies 

Instance Property

# httpShouldHandleCookies

A Boolean value that indicates whether the request should use the default cookie handling for the request.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var httpShouldHandleCookies: Bool { get set }
```

## Discussion

true if the request should use the default cookie handling for the request, false otherwise. The default is true.

If your app sets the `Cookie` header on an NSMutableURLRequest object, then this method has no effect, and the cookie data you set in the header overrides all cookies from the cookie store.

### Special considerations

In OS X v10.2 with Safari 1.0 the value set by this method is not respected by the framework.

## See Also

### Related Documentation

var httpShouldHandleCookies: Bool

A Boolean value that indicates whether the default cookie handling will be used for this request.

### Controlling request behavior

var timeoutInterval: TimeInterval

The request’s timeout interval, in seconds.

var httpShouldUsePipelining: Bool

A Boolean value that indicates whether the request can continue transmitting data before receiving a response from an earlier transmission.

Deprecated

var allowsCellularAccess: Bool

A Boolean value that indicates whether a connection can use the device’s cellular network (if present).

