

- Foundation
-  HTTPCookieStringPolicy 

Structure

# HTTPCookieStringPolicy

Values that indicate whether to restrict the cookie to requests sent back to the same site that created it.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct HTTPCookieStringPolicy
```

## Discussion

RFC 6265 defines “same site” as the registerable domain of a URI.

## Topics

### Creating a policy

init(rawValue: String)

### Policies

static let sameSiteStrict: HTTPCookieStringPolicy

A policy that prohibits a cross-site request from including the cookie.

static let sameSiteLax: HTTPCookieStringPolicy

A policy that allows certain cross-site requests to include the cookie.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Securing cookies

var isHTTPOnly: Bool

A Boolean value that indicates whether the cookie should only be sent to HTTP servers.

var isSecure: Bool

A Boolean value that indicates whether the cookie may only be sent over secure channels.

var sameSitePolicy: HTTPCookieStringPolicy?

A Boolean value that indicates whether to restrict the cookie to requests sent back to the same site that created it.

