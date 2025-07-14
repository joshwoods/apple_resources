

- Foundation
- NSMutableURLRequest
-  allHTTPHeaderFields 

Instance Property

# allHTTPHeaderFields

A dictionary containing all of the HTTP header fields for a request.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var allHTTPHeaderFields: [String : String]? { get set }
```

## Discussion

Certain header fields are reserved (see Reserved HTTP headers). Do not use this property to set such headers.

## See Also

### Accessing header fields

func addValue(String, forHTTPHeaderField: String)

Adds a value to the header field.

func setValue(String?, forHTTPHeaderField: String)

Sets a value for the header field.

