

- Foundation
- URLSessionConfiguration
-  httpCookieAcceptPolicy 

Instance Property

# httpCookieAcceptPolicy

A policy constant that determines when cookies should be accepted.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var httpCookieAcceptPolicy: HTTPCookie.AcceptPolicy { get set }
```

## Discussion

This property determines the cookie accept policy for all tasks within sessions based on this configuration.

The default value is HTTPCookie.AcceptPolicy.onlyFromMainDocumentDomain. You can change it to any of the constants defined in the HTTPCookie.AcceptPolicy enumerated type.

If you want more direct control over what cookies are accepted, set this value to HTTPCookie.AcceptPolicy.never and then use the allHeaderFields and cookies(withResponseHeaderFields:for:) methods to extract cookies from the URL response object yourself.

## See Also

### Setting cookie policies

var httpShouldSetCookies: Bool

A Boolean value that determines whether requests should contain cookies from the cookie store.

var httpCookieStorage: HTTPCookieStorage?

The cookie store for storing cookies within this session.

class HTTPCookie

A representation of an HTTP cookie.

