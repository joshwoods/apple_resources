

- Foundation
- HTTPCookiePropertyKey
-  path 

Type Property

# path

An `NSString` object containing the path for the cookie.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let path: HTTPCookiePropertyKey
```

## Discussion

This cookie attribute is required.

## See Also

### Cookie property keys

static let comment: HTTPCookiePropertyKey

An `NSString` object containing the comment for the cookie.

static let commentURL: HTTPCookiePropertyKey

An `NSURL` object or `NSString` object containing the comment URL for the cookie.

static let discard: HTTPCookiePropertyKey

An `NSString` object stating whether the cookie should be discarded at the end of the session.

static let domain: HTTPCookiePropertyKey

An `NSString` object containing the domain for the cookie.

static let expires: HTTPCookiePropertyKey

An `NSDate` object or `NSString` object specifying the expiration date for the cookie.

static let maximumAge: HTTPCookiePropertyKey

An `NSString` object containing an integer value stating how long in seconds the cookie should be kept, at most.

static let name: HTTPCookiePropertyKey

An `NSString` object containing the name of the cookie (required).

static let originURL: HTTPCookiePropertyKey

An NSURL or `NSString` object containing the URL that set this cookie.

static let port: HTTPCookiePropertyKey

An `NSString` object containing comma-separated integer values specifying the ports for the cookie.

static let sameSitePolicy: HTTPCookiePropertyKey

A string indicating the same-site policy for the cookie.

static let secure: HTTPCookiePropertyKey

An `NSString` object indicating that the cookie should be transmitted only over secure channels.

static let value: HTTPCookiePropertyKey

An `NSString` object containing the value of the cookie.

static let version: HTTPCookiePropertyKey

An `NSString` object that specifies the version of the cookie.

