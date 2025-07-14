

- Foundation
- NSURLRequest
-  value(forHTTPHeaderField:) 

Instance Method

# value(forHTTPHeaderField:)

Returns the value of the specified HTTP header field.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func value(forHTTPHeaderField field: String) -> String?
```

## Parameters 

`field`  

The name of the header field whose value is to be returned. In keeping with the HTTP RFC, HTTP header field names are case-insensitive.

## Return Value

The value associated with the header field `field`, or `nil` if there is no corresponding header field.

## See Also

### Related Documentation

func addValue(String, forHTTPHeaderField: String)

Adds a value to the header field.

func setValue(String?, forHTTPHeaderField: String)

Sets a value for the header field.

### Getting header fields

var allHTTPHeaderFields: [String : String]?

A dictionary containing all of the HTTP header fields for a request.

