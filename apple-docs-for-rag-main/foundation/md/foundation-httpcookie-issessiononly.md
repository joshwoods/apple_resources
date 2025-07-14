

- Foundation
- HTTPCookie
-  isSessionOnly 

Instance Property

# isSessionOnly

A Boolean value that indicates whether the cookie should be discarded at the end of the session (regardless of expiration date).

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isSessionOnly: Bool { get }
```

## Discussion

This value is true if the cookie should be discarded at the end of the session (regardless of expiration date), otherwise false.

## See Also

### Determining cookie lifespan

var expiresDate: Date?

The cookie’s expiration date.

