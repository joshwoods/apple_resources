

- Foundation
- HTTPCookie
-  comment 

Instance Property

# comment

The cookie’s comment string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var comment: String? { get }
```

## Discussion

This value is `nil` if the cookie has no comment. You can present this string to the user, explaining the contents and purpose of this cookie.

## See Also

### Getting user-readable cookie metadata

var commentURL: URL?

The cookie’s comment URL.

