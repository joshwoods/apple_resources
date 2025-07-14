

- Foundation
- HTTPCookie
-  isHTTPOnly 

Instance Property

# isHTTPOnly

A Boolean value that indicates whether the cookie should only be sent to HTTP servers.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isHTTPOnly: Bool { get }
```

## Discussion

The value of this property is true if the cookie should only be sent using HTTP headers, false otherwise.

Cookies can be marked as HTTP-only by a server (or by JavaScript code). Cookies marked as such must only be sent via HTTP Headers in HTTP requests for URLs that match both the path and domain of the respective cookies.

Note

RFC 6265 formally defines the `HttpOnly` attribute.

Important

To prevent cross-site scripting vulnerabilities, don’t deliver cookies marked as HTTP-only to JavaScript code.

## See Also

### Securing cookies

var isSecure: Bool

A Boolean value that indicates whether the cookie may only be sent over secure channels.

var sameSitePolicy: HTTPCookieStringPolicy?

A Boolean value that indicates whether to restrict the cookie to requests sent back to the same site that created it.

struct HTTPCookieStringPolicy

Values that indicate whether to restrict the cookie to requests sent back to the same site that created it.

