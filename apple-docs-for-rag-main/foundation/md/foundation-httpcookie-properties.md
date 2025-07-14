

- Foundation
- HTTPCookie
-  properties 

Instance Property

# properties

The cookie’s properties.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var properties: [HTTPCookiePropertyKey : Any]? { get }
```

## Discussion

This dictionary can be used with init(properties:) (or cookieWithProperties: in Objective-C) to create an equivalent HTTPCookie object.

See init(properties:) for more information on the constraints imposed on the `properties` dictionary.

## See Also

### Accessing cookie properties as key-value pairs

struct HTTPCookiePropertyKey

Constants that define the supported keys in a cookie attributes dictionary.

