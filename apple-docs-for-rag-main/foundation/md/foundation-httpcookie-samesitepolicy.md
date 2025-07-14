

- Foundation
- HTTPCookie
-  sameSitePolicy 

Instance Property

# sameSitePolicy

A Boolean value that indicates whether to restrict the cookie to requests sent back to the same site that created it.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var sameSitePolicy: HTTPCookieStringPolicy? { get }
```

## Discussion

Along with the policy values defined by HTTPCookieStringPolicy, this property may also be `nil`. In this case, cross-site requests include the cookie.

## See Also

### Securing cookies

var isHTTPOnly: Bool

A Boolean value that indicates whether the cookie should only be sent to HTTP servers.

var isSecure: Bool

A Boolean value that indicates whether the cookie may only be sent over secure channels.

struct HTTPCookieStringPolicy

Values that indicate whether to restrict the cookie to requests sent back to the same site that created it.

