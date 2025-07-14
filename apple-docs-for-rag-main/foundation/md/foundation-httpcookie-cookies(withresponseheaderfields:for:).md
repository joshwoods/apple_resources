

- Foundation
- HTTPCookie
-  cookies(withResponseHeaderFields:for:) 

Type Method

# cookies(withResponseHeaderFields:for:)

Creates an array of HTTP cookies that corresponds to the provided response header fields for the provided URL.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func cookies(
    withResponseHeaderFields headerFields: [String : String],
    for URL: URL
) -> [HTTPCookie]
```

## Parameters 

`headerFields`  

The header fields used to create the HTTPCookie objects.

`URL`  

The URL associated with the created cookies.

## Return Value

The array of created cookies.

## Discussion

This method ignores irrelevant header fields in `headerFields`, allowing dictionaries to contain additional data.

If `headerFields` doesn’t specify a domain for a given cookie, the cookie is created with a default domain value of `URL`.

If `headerFields` doesn’t specify a path for a given cookie, the cookie is created with a default path value of `"/"`.

## See Also

### Creating cookies

init?(properties: [HTTPCookiePropertyKey : Any])

Initializes an HTTP cookie object with the given cookie properties.

