

- Foundation
- HTTPCookie
-  path 

Instance Property

# path

The cookie’s path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var path: String { get }
```

## Discussion

The cookie will be sent with requests for this path in the cookie’s domain, and all paths that have this prefix. A path of `"/"` means the cookie will be sent for all URLs in the domain.

## See Also

### Getting cookie host properties

var domain: String

The domain of the cookie.

var portList: [NSNumber]?

The cookie’s port list.

