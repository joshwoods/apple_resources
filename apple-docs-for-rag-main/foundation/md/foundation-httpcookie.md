

- Foundation
-  HTTPCookie 

Class

# HTTPCookie

A representation of an HTTP cookie.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class HTTPCookie
```

## Overview

An HTTPCookie object is immutable, initialized from a dictionary that contains the attributes of the cookie. This class supports two different cookie versions:

- Version 0: The original cookie format defined by Netscape. Most cookies are in this format.

- Version 1: The cookie format defined in RFC 6265, HTTP State Management Mechanism.

## Topics

### Creating cookies

class func cookies(withResponseHeaderFields: [String : String], for: URL) -> [HTTPCookie]

Creates an array of HTTP cookies that corresponds to the provided response header fields for the provided URL.

init?(properties: [HTTPCookiePropertyKey : Any])

Initializes an HTTP cookie object with the given cookie properties.

### Converting cookies to request headers

class func requestHeaderFields(with: [HTTPCookie]) -> [String : String]

Converts an array of cookies to a dictionary of header fields.

### Getting cookie host properties

var domain: String

The domain of the cookie.

var path: String

The cookie’s path.

var portList: [NSNumber]?

The cookie’s port list.

### Getting cookie metadata

var name: String

The cookie’s name.

var value: String

The cookie’s string value.

var version: Int

The cookie’s version.

### Determining cookie lifespan

var expiresDate: Date?

The cookie’s expiration date.

var isSessionOnly: Bool

A Boolean value that indicates whether the cookie should be discarded at the end of the session (regardless of expiration date).

### Securing cookies

var isHTTPOnly: Bool

A Boolean value that indicates whether the cookie should only be sent to HTTP servers.

var isSecure: Bool

A Boolean value that indicates whether the cookie may only be sent over secure channels.

var sameSitePolicy: HTTPCookieStringPolicy?

A Boolean value that indicates whether to restrict the cookie to requests sent back to the same site that created it.

struct HTTPCookieStringPolicy

Values that indicate whether to restrict the cookie to requests sent back to the same site that created it.

### Accessing cookie properties as key-value pairs

var properties: [HTTPCookiePropertyKey : Any]?

The cookie’s properties.

struct HTTPCookiePropertyKey

Constants that define the supported keys in a cookie attributes dictionary.

### Getting user-readable cookie metadata

var comment: String?

The cookie’s comment string.

var commentURL: URL?

The cookie’s comment URL.

### Accepting cookies

enum AcceptPolicy

Cookie acceptance policies implemented by the HTTPCookieStorage class.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Cookies

class HTTPCookieStorage

A container that manages the storage of cookies.

