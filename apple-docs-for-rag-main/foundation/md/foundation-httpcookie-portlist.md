

- Foundation
- HTTPCookie
-  portList 

Instance Property

# portList

The cookie’s port list.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var portList: [NSNumber]? { get }
```

## Discussion

The list of ports for the cookie, returned as an array of `NSNumber` objects containing integers. If the cookie has no port list, the value of this property is `nil` and the cookie will be sent to any port. Otherwise, the cookie is only sent to ports specified in the port list.

## See Also

### Getting cookie host properties

var domain: String

The domain of the cookie.

var path: String

The cookie’s path.

