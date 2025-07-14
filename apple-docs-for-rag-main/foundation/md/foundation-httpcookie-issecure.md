

- Foundation
- HTTPCookie
-  isSecure 

Instance Property

# isSecure

A Boolean value that indicates whether the cookie may only be sent over secure channels.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isSecure: Bool { get }
```

## Discussion

This value is true if this cookie should only be sent over secure channels, otherwise false.

## See Also

### Securing cookies

var isHTTPOnly: Bool

A Boolean value that indicates whether the cookie should only be sent to HTTP servers.

var sameSitePolicy: HTTPCookieStringPolicy?

A Boolean value that indicates whether to restrict the cookie to requests sent back to the same site that created it.

struct HTTPCookieStringPolicy

Values that indicate whether to restrict the cookie to requests sent back to the same site that created it.

