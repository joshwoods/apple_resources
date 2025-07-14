

- Foundation
- HTTPURLResponse
-  localizedString(forStatusCode:) 

Type Method

# localizedString(forStatusCode:)

Returns a localized string corresponding to a specified HTTP status code.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func localizedString(forStatusCode statusCode: Int) -> String
```

## Parameters 

`statusCode`  

The HTTP status code. See RFC 2616 for details.

## Return Value

A localized string suitable for displaying to users that describes the specified status code.

## See Also

### Getting response status codes

var statusCode: Int

The response’s HTTP status code.

