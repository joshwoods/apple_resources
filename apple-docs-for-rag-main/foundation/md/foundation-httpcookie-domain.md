

- Foundation
- HTTPCookie
-  domain 

Instance Property

# domain

The domain of the cookie.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var domain: String { get }
```

## Discussion

If the domain does not start with a dot, then the cookie is only sent to the exact host specified by the domain. If the domain does start with a dot, then the cookie is sent to other hosts in that domain as well, subject to certain restrictions. See RFC 6265 for more detail.

## See Also

### Getting cookie host properties

var path: String

The cookie’s path.

var portList: [NSNumber]?

The cookie’s port list.

