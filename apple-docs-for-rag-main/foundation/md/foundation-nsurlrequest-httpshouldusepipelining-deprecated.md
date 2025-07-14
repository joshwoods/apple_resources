

- Foundation
- NSURLRequest
-  httpShouldUsePipelining Deprecated

Instance Property

# httpShouldUsePipelining

A Boolean value that indicates whether the request should continue transmitting data before receiving a response from an earlier transmission.

iOS 4.0–18.4DeprecatediPadOS 4.0–18.4DeprecatedMac Catalyst 13.1–18.4DeprecatedmacOS 10.7–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–11.4Deprecated

``` source
var httpShouldUsePipelining: Bool { get }
```

Deprecated

Only supported in the classic loader, please adopt HTTP/2 and HTTP/3 instead

## Discussion

true if the request should continue transmitting data; otherwise, false.

## See Also

### Related Documentation

var httpShouldUsePipelining: Bool

A Boolean value that indicates whether the request can continue transmitting data before receiving a response from an earlier transmission.

Deprecated

### Controlling request behavior

var timeoutInterval: TimeInterval

The request’s timeout interval, in seconds.

var httpShouldHandleCookies: Bool

A Boolean value that indicates whether the default cookie handling will be used for this request.

var allowsCellularAccess: Bool

A Boolean value that indicates whether the request is allowed to use the cellular radio (if present).

