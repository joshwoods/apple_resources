

- Foundation
- NSMutableURLRequest
-  addValue(\_:forHTTPHeaderField:) 

Instance Method

# addValue(\_:forHTTPHeaderField:)

Adds a value to the header field.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addValue(
    _ value: String,
    forHTTPHeaderField field: String
)
```

## Parameters 

`value`  

The value for the header field.

`field`  

The name of the header field. In keeping with the HTTP RFC, HTTP header field names are case insensitive.

## Discussion

This method provides the ability to add values to header fields incrementally. If a value was previously set for the specified field, the supplied value is appended to the existing value using the appropriate field delimiter (a comma).

Certain header fields are reserved (see Reserved HTTP headers). Do not use this method to change such headers.

## See Also

### Related Documentation

func value(forHTTPHeaderField: String) -> String?

Returns the value of the specified HTTP header field.

### Accessing header fields

var allHTTPHeaderFields: [String : String]?

A dictionary containing all of the HTTP header fields for a request.

func setValue(String?, forHTTPHeaderField: String)

Sets a value for the header field.

