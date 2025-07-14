

- Foundation
- HTTPCookie
-  commentURL 

Instance Property

# commentURL

The cookie’s comment URL.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var commentURL: URL? { get }
```

## Discussion

This value is `nil` if the cookie has no comment URL. This value specifies a URL that can be presented to the user as a link for further information about this cookie.

## See Also

### Getting user-readable cookie metadata

var comment: String?

The cookie’s comment string.

