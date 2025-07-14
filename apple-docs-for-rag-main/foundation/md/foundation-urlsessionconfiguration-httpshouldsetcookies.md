

- Foundation
- URLSessionConfiguration
-  httpShouldSetCookies 

Instance Property

# httpShouldSetCookies

A Boolean value that determines whether requests should contain cookies from the cookie store.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var httpShouldSetCookies: Bool { get set }
```

## Discussion

This property controls whether tasks within sessions based on this configuration should automatically provide cookies from the shared cookie store when making requests.

If you want to provide cookies yourself, set this value to false and provide a `Cookie` header either through the session’s httpAdditionalHeaders property or on a per-request level using a custom NSURLRequest object.

The default value is true.

## See Also

### Setting cookie policies

var httpCookieAcceptPolicy: HTTPCookie.AcceptPolicy

A policy constant that determines when cookies should be accepted.

var httpCookieStorage: HTTPCookieStorage?

The cookie store for storing cookies within this session.

class HTTPCookie

A representation of an HTTP cookie.

