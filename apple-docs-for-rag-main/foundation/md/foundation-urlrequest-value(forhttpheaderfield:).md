

- Foundation
- URLRequest
-  value(forHTTPHeaderField:) 

Instance Method

# value(forHTTPHeaderField:)

Retrieves a header value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func value(forHTTPHeaderField field: String) -> String?
```

## Parameters 

`field`  

The header field name to use for the lookup (case-insensitive).

## Return Value

The value associated with the header field field, or `nil` if there is no corresponding header field.

## Discussion

Note that, in keeping with the HTTP RFC, HTTP header field names are case-insensitive.

## See Also

### Accessing header fields

var allHTTPHeaderFields: [String : String]?

A dictionary containing all of the HTTP header fields for a request.

func addValue(String, forHTTPHeaderField: String)

Adds a value to the header field.

func setValue(String?, forHTTPHeaderField: String)

Sets a value for the header field.

