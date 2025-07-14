

- Foundation
- HTTPCookie
-  init(properties:) 

Initializer

# init(properties:)

Initializes an HTTP cookie object with the given cookie properties.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(properties: [HTTPCookiePropertyKey : Any])
```

## Parameters 

`properties`  

The properties for the new cookie object, expressed as key-value pairs.

## Return Value

A new cookie object, with the given properies.

## Discussion

This initializer returns `nil` if the provided properties are invalid. To successfully create a cookie, you must provide values for (at least) the path, name, and value keys, and either the originURL key or the domain key.

See Accepting cookies for more information on the available cookie attribute constants and the constraints imposed on the values in the dictionary.

## See Also

### Creating cookies

class func cookies(withResponseHeaderFields: [String : String], for: URL) -> [HTTPCookie]

Creates an array of HTTP cookies that corresponds to the provided response header fields for the provided URL.

