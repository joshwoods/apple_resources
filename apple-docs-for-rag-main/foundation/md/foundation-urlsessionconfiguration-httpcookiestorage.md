

- Foundation
- URLSessionConfiguration
-  httpCookieStorage 

Instance Property

# httpCookieStorage

The cookie store for storing cookies within this session.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var httpCookieStorage: HTTPCookieStorage? { get set }
```

## Discussion

This property determines the cookie storage object used by all tasks within sessions based on this configuration.

To disable cookie storage, set this property to `nil`.

For default and background sessions, the default value is the shared cookie storage object.

For ephemeral sessions, the default value is a private cookie storage object that stores data in memory only, and is destroyed when you invalidate the session.

## See Also

### Setting cookie policies

var httpCookieAcceptPolicy: HTTPCookie.AcceptPolicy

A policy constant that determines when cookies should be accepted.

var httpShouldSetCookies: Bool

A Boolean value that determines whether requests should contain cookies from the cookie store.

class HTTPCookie

A representation of an HTTP cookie.

